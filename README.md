# OSERA backlog

The vulnerabilities (CVEs) OSERA fixes on the lines it supports, in priority order, one GitHub issue each. The backlog says what to fix, why, and where each one stands. How a CVE gets fixed is the producer's decision.

## Files

| File | Written by | What it holds |
|---|---|---|
| `supported-lines.csv` | people, then the line manager | One row per supported line. People declare `line_id`, `ecosystem` (maven, pypi, npm), `anchor` (the artifact whose version fixes every package in the line, for Java the Spring Boot dependency list), `components` (the line's projects inside the anchor, one `group@version` each: the group is the scope, the version pins the whole group when the anchor lists it at another; empty when the anchor is the project's own BOM), `scope`, `source`. The line manager fills `status` (not fixed, in progress, fixed), `book_version`, `as_of`, the five counts and `consume`, the OSERA BOM a bank imports |
| `rules/prioritisation.yaml` | people | The Risk Navigator rules the line manager applies: the score bands, the signals, which CVEs are in, which priority each gets, the curated list |
| `cve-backlog.json` | the line manager | The backlog. One entry per CVE and library and line, entry schema 0.6.0, with a `status` per entry. CVSS 3.1 score from NVD, priority and rules from the Risk Navigator |
| `cve-excluded.json` | the line manager | Every CVE the scan found that the rules left out, with the reason |
| `cve-backlog.md` | the line manager | The backlog as a table |
| `graphs/<line_id>/` | the line manager | The dependency graph of the line, CycloneDX, one file per resolver |
| `bom/<line_id>/pom.xml` | the line manager | The OSERA BOM of the line, the same file it publishes in the release repository |
| `status/<line_id>.json` | the line manager | The lists behind the counts of the line row |
| `schema/` | people | What an entry must look like |
| `.github/ISSUE_TEMPLATE/cve.md` | people | The issue template |

## How it works

1. **Members approve the line.** A line is one row in `supported-lines.csv`. Two approvers approve the pull request that adds it. They approve the line, and not each CVE.
2. **The line manager builds the backlog.** From the line's graph, the advisories, the scores and the rules file, it writes `cve-backlog.json` and opens a pull request. The `validate` check confirms every entry matches the schema and names a supported line. The line manager merges its own pull request when the check is green. Nobody approves the backlog.
3. **The line manager tags.** It tags the merge commit, `v2026.09.16` style. Merging alone publishes nothing.
4. **The tag opens the issues.** The `open-issues` workflow opens one issue per CVE and library version, labelled with the priority band and the line. A CVE that already has an issue anywhere in the organisation is left alone, with a comment if its priority changed. The workflow never closes or deletes anything.
5. **Producers fix, the line manager closes.** A producer moves the issue into the patch repository and works there. When the fixed release is promoted into the release repository, the line manager marks the entry fixed, publishes the BOM, and closes the issue with the published coordinates and the BOM version.

6. **A CVE can leave the backlog.** The line manager scans every line again each day. A CVE that two scans in a row no longer find (its score fell under the bar, the rules changed, the library left the line's graph) is removed from `cve-backlog.json` and written to `cve-excluded.json` with the reason and the dates. Its issue is closed with the same words and the label `out of scope`, on the board or in the producer's patch repository. Found again later, it comes back as open and its issue reopens. A CVE leaving the backlog is never a fix.

Never in this repository: how a CVE gets fixed, which member asked for what, anything a member chose not to fix.

## Known limits

- An issue title names the artifact and the version, `snakeyaml 1.33`, not the group. The line manager pairs a CVE with its issue by CVE, artifact and version. Two libraries with the same artifact name in different groups, at the same version, with the same CVE, would share one issue. Rare, known, left as it is.

## Labels

`cve` on every issue, `P0 / Act`, `P1 / Attend`, `P2 / Investigate` for the priority, `kev` for the CISA Known Exploited Vulnerabilities list, one label per line.

## Sources

- Lines and Wave 1 scope: the OSERA Board and https://github.com/finos-osera/risk-navigator/issues/7
- Prioritisation rules: https://github.com/finos-osera/risk-navigator/issues/7
- The flow: https://github.com/finos-osera/operations-taskforce/issues/23
