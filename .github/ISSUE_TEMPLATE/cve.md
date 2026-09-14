---
name: CVE to fix on a supported line
about: One issue per CVE from the order book. Opened by the backlog workflow, or by hand for a CVE that is not in the book yet.
title: "<P0, P1 or P2> <CVE id> in <library> <version>"
labels: cve
---

## What

- CVE: <CVE id, with the link to the advisory>
- Library: <group:artifact of the jar that holds the affected code>
- Version on the line: <version>
- Lines: <the supported lines this CVE is on>

## Why it is in the book

- Priority: <priority band>
- CVSS: <score and version, as recorded at NVD>
- CISA KEV: <yes or no>
- EPSS percentile: <value>
- Rules that put it here, from https://github.com/finos-osera/risk-navigator/issues/7:
<one rule per line>

## Summary

<the advisory's one line summary>

## Book

- Opened from: <book version tag>
- Entry: <link to the row in cve-backlog.md>
