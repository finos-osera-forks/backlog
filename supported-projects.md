# Supported projects

Generated 2026-09-24T06:05:27Z. Written by the line manager reconciler.

The latest patch view: every library at the latest upstream patch release, the view the work follows. Every library and version the exchange maintains, ordered by library and then by version. A library that sits on more than one line is one row, with every line it belongs to named. For reporting only.

## Lines

| line_id | ecosystem | anchor | status | CVE_in_scope | CVE_fixed | CVE_fixed_% | CVE_out_of_scope | CVE_in_progress | CVE_left | CVE_not_remediable |
|---|---|---|---|---|---|---|---|---|---|---|
| spring-boot-2.7.x | maven | `org.springframework.boot:spring-boot-dependencies@2.7.18` | in progress | 71 | 1 | 1% | 196 | 0 | 70 | 0 |
| spring-framework-5.3.x | maven | `org.springframework:spring-framework-bom@5.3.39` | not fixed | 19 | 0 | 0% | 24 | 0 | 19 | 0 |
| spring-security-5.7.x | maven | `org.springframework.security:spring-security-bom@5.7.11` | not fixed | 20 | 0 | 0% | 40 | 0 | 20 | 0 |

## Libraries

41 libraries across 3 line(s).

| name | version | lines | why_listed | status | CVE_in_scope | CVE_fixed | CVE_fixed_% | CVE_out_of_scope | CVE_in_progress | CVE_left | CVE_not_remediable | patched_as | consumed | consumption_readiness | chain | files | evidence | signatures | document | producer | verdict | fork | tag | upload | tagger |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| ch.qos.logback:logback-core | 1.2.13 | spring-boot-2.7.x | listed by the BOM at 1.2.12 | open | 1 | 0 | 0% | 5 | 0 | 1 | 0 |  |  | not claimed |  |  |  |  |  |  |  |  |  |  |  |
| com.fasterxml.jackson.core:jackson-core | 2.13.5 | spring-boot-2.7.x, spring-security-5.7.x | listed by the BOM of spring-boot-2.7.x at 2.13.5 (com.fasterxml.jackson:jackson-bom@2.13.5) | open | 2 | 0 | 0% | 0 | 0 | 2 | 0 |  |  | not claimed |  |  |  |  |  |  |  |  |  |  |  |
| com.fasterxml.jackson.core:jackson-databind | 2.13.5 | spring-boot-2.7.x, spring-security-5.7.x | listed by the BOM of spring-boot-2.7.x at 2.13.5 (com.fasterxml.jackson:jackson-bom@2.13.5) | open | 3 | 0 | 0% | 2 | 0 | 3 | 0 |  |  | not claimed |  |  |  |  |  |  |  |  |  |  |  |
| com.fasterxml.jackson.dataformat:jackson-dataformat-toml | 2.13.5 | spring-boot-2.7.x | listed by the BOM at 2.13.5 (com.fasterxml.jackson:jackson-bom@2.13.5) | open | 1 | 0 | 0% | 0 | 0 | 1 | 0 |  |  | not claimed |  |  |  |  |  |  |  |  |  |  |  |
| io.projectreactor.netty:reactor-netty | 1.0.48 | spring-boot-2.7.x | listed by the BOM at 1.0.39 (io.projectreactor:reactor-bom@2020.0.38) | open | 1 | 0 | 0% | 0 | 0 | 1 | 0 |  |  | not claimed |  |  |  |  |  |  |  |  |  |  |  |
| io.projectreactor.netty:reactor-netty-http | 1.0.48 | spring-boot-2.7.x | listed by the BOM at 1.0.39 (io.projectreactor:reactor-bom@2020.0.38) | open | 1 | 0 | 0% | 0 | 0 | 1 | 0 |  |  | not claimed |  |  |  |  |  |  |  |  |  |  |  |
| org.apache.logging.log4j:log4j-1.2-api | 2.17.2 | spring-boot-2.7.x | listed by the BOM at 2.17.2 (org.apache.logging.log4j:log4j-bom@2.17.2) | open | 1 | 0 | 0% | 0 | 0 | 1 | 0 |  |  | not claimed |  |  |  |  |  |  |  |  |  |  |  |
| org.apache.logging.log4j:log4j-core | 2.17.2 | spring-boot-2.7.x | listed by the BOM at 2.17.2 (org.apache.logging.log4j:log4j-bom@2.17.2) | open | 1 | 0 | 0% | 2 | 0 | 1 | 0 |  |  | not claimed |  |  |  |  |  |  |  |  |  |  |  |
| org.apache.logging.log4j:log4j-layout-template-json | 2.17.2 | spring-boot-2.7.x | listed by the BOM at 2.17.2 (org.apache.logging.log4j:log4j-bom@2.17.2) | open | 1 | 0 | 0% | 0 | 0 | 1 | 0 |  |  | not claimed |  |  |  |  |  |  |  |  |  |  |  |
| org.eclipse.jetty:jetty-http | 9.4.58.v20250814 | spring-boot-2.7.x | listed by the BOM at 9.4.53.v20231009 (org.eclipse.jetty:jetty-bom@9.4.53.v20231009) | open | 1 | 0 | 0% | 1 | 0 | 1 | 0 |  |  | not claimed |  |  |  |  |  |  |  |  |  |  |  |
| org.eclipse.jetty:jetty-jaspi | 9.4.58.v20250814 | spring-boot-2.7.x | listed by the BOM at 9.4.53.v20231009 (org.eclipse.jetty:jetty-bom@9.4.53.v20231009) | open | 1 | 0 | 0% | 0 | 0 | 1 | 0 |  |  | not claimed |  |  |  |  |  |  |  |  |  |  |  |
| org.eclipse.jetty:jetty-security | 9.4.58.v20250814 | spring-boot-2.7.x | listed by the BOM at 9.4.53.v20231009 (org.eclipse.jetty:jetty-bom@9.4.53.v20231009) | open | 1 | 0 | 0% | 0 | 0 | 1 | 0 |  |  | not claimed |  |  |  |  |  |  |  |  |  |  |  |
| org.hibernate:hibernate-core | 5.6.15.Final | spring-boot-2.7.x | listed by the BOM at 5.6.15.Final | fixed | 1 | 1 | 100% | 0 | 0 | 0 | 0 | 5.6.15.Final-osera-00001 | 5.6.15.Final-osera-00001 | ready | complete | OK | OK | OK | OK | OK | OK | OK | OK | OK | OK |
| org.springframework.boot:spring-boot | 2.7.18 | spring-boot-2.7.x | own project (the anchor's group) | open | 2 | 0 | 0% | 0 | 0 | 2 | 0 |  |  | not claimed |  |  |  |  |  |  |  |  |  |  |  |
| org.springframework.boot:spring-boot-devtools | 2.7.18 | spring-boot-2.7.x | own project (the anchor's group) | open | 1 | 0 | 0% | 0 | 0 | 1 | 0 |  |  | not claimed |  |  |  |  |  |  |  |  |  |  |  |
| org.springframework.boot:spring-boot-loader | 2.7.18 | spring-boot-2.7.x | own project (the anchor's group) | open | 1 | 0 | 0% | 0 | 0 | 1 | 0 |  |  | not claimed |  |  |  |  |  |  |  |  |  |  |  |
| org.springframework.boot:spring-boot-starter-actuator | 2.7.18 | spring-boot-2.7.x | own project (the anchor's group) | open | 1 | 0 | 0% | 0 | 0 | 1 | 0 |  |  | not claimed |  |  |  |  |  |  |  |  |  |  |  |
| org.springframework.data:spring-data-commons | 2.7.18 | spring-boot-2.7.x, spring-security-5.7.x | listed by the BOM of spring-boot-2.7.x at 2.7.18 (org.springframework.data:spring-data-bom@2021.2.18) | open | 1 | 0 | 0% | 2 | 0 | 1 | 0 |  |  | not claimed |  |  |  |  |  |  |  |  |  |  |  |
| org.springframework.data:spring-data-keyvalue | 2.7.18 | spring-boot-2.7.x | listed by the BOM at 2.7.18 (org.springframework.data:spring-data-bom@2021.2.18) | open | 1 | 0 | 0% | 0 | 0 | 1 | 0 |  |  | not claimed |  |  |  |  |  |  |  |  |  |  |  |
| org.springframework.data:spring-data-mongodb | 3.4.18 | spring-boot-2.7.x | listed by the BOM at 3.4.18 (org.springframework.data:spring-data-bom@2021.2.18) | open | 1 | 0 | 0% | 1 | 0 | 1 | 0 |  |  | not claimed |  |  |  |  |  |  |  |  |  |  |  |
| org.springframework.data:spring-data-rest-core | 3.7.18 | spring-boot-2.7.x | listed by the BOM at 3.7.18 (org.springframework.data:spring-data-bom@2021.2.18) | open | 2 | 0 | 0% | 2 | 0 | 2 | 0 |  |  | not claimed |  |  |  |  |  |  |  |  |  |  |  |
| org.springframework.graphql:spring-graphql | 1.0.6 | spring-boot-2.7.x | listed by the BOM at 1.0.6 | open | 2 | 0 | 0% | 0 | 0 | 2 | 0 |  |  | not claimed |  |  |  |  |  |  |  |  |  |  |  |
| org.springframework.hateoas:spring-hateoas | 1.5.6 | spring-boot-2.7.x | listed by the BOM at 1.5.6 | open | 2 | 0 | 0% | 0 | 0 | 2 | 0 |  |  | not claimed |  |  |  |  |  |  |  |  |  |  |  |
| org.springframework.integration:spring-integration-file | 5.5.20 | spring-boot-2.7.x | listed by the BOM at 5.5.20 (org.springframework.integration:spring-integration-bom@5.5.20) | open | 1 | 0 | 0% | 0 | 0 | 1 | 0 |  |  | not claimed |  |  |  |  |  |  |  |  |  |  |  |
| org.springframework.kafka:spring-kafka | 2.8.11 | spring-boot-2.7.x | listed by the BOM at 2.8.11 | open | 4 | 0 | 0% | 0 | 0 | 4 | 0 |  |  | not claimed |  |  |  |  |  |  |  |  |  |  |  |
| org.springframework.ldap:spring-ldap-core | 2.4.4 | spring-boot-2.7.x, spring-security-5.7.x | listed by the BOM of spring-boot-2.7.x at 2.4.1 | open | 1 | 0 | 0% | 0 | 0 | 1 | 0 |  |  | not claimed |  |  |  |  |  |  |  |  |  |  |  |
| org.springframework.security:spring-security-core | 5.7.11 | spring-boot-2.7.x, spring-security-5.7.x | own project on spring-boot-2.7.x (declared org.springframework.security@5.7.11) | open | 1 | 0 | 0% | 2 | 0 | 1 | 0 |  |  | not claimed |  |  |  |  |  |  |  |  |  |  |  |
| org.springframework.security:spring-security-crypto | 5.7.11 | spring-boot-2.7.x, spring-security-5.7.x | own project on spring-boot-2.7.x (declared org.springframework.security@5.7.11) | open | 1 | 0 | 0% | 0 | 0 | 1 | 0 |  |  | not claimed |  |  |  |  |  |  |  |  |  |  |  |
| org.springframework.security:spring-security-saml2-service-provider | 5.7.11 | spring-boot-2.7.x, spring-security-5.7.x | own project on spring-boot-2.7.x (declared org.springframework.security@5.7.11) | open | 1 | 0 | 0% | 2 | 0 | 1 | 0 |  |  | not claimed |  |  |  |  |  |  |  |  |  |  |  |
| org.springframework.security:spring-security-web | 5.7.11 | spring-boot-2.7.x, spring-security-5.7.x | own project on spring-boot-2.7.x (declared org.springframework.security@5.7.11) | open | 4 | 0 | 0% | 0 | 0 | 4 | 0 |  |  | not claimed |  |  |  |  |  |  |  |  |  |  |  |
| org.springframework.ws:spring-ws-core | 3.1.8 | spring-boot-2.7.x | listed by the BOM at 3.1.8 | open | 1 | 0 | 0% | 0 | 0 | 1 | 0 |  |  | not claimed |  |  |  |  |  |  |  |  |  |  |  |
| org.springframework.ws:spring-ws-security | 3.1.8 | spring-boot-2.7.x | listed by the BOM at 3.1.8 | open | 1 | 0 | 0% | 4 | 0 | 1 | 0 |  |  | not claimed |  |  |  |  |  |  |  |  |  |  |  |
| org.springframework.ws:spring-xml | 3.1.8 | spring-boot-2.7.x | listed by the BOM at 3.1.8 | open | 1 | 0 | 0% | 0 | 0 | 1 | 0 |  |  | not claimed |  |  |  |  |  |  |  |  |  |  |  |
| org.springframework:spring-core | 5.3.39 | spring-boot-2.7.x, spring-framework-5.3.x, spring-security-5.7.x | own project on spring-boot-2.7.x (declared org.springframework@5.3.39) | open | 2 | 0 | 0% | 0 | 0 | 2 | 0 |  |  | not claimed |  |  |  |  |  |  |  |  |  |  |  |
| org.springframework:spring-expression | 5.3.39 | spring-boot-2.7.x, spring-framework-5.3.x, spring-security-5.7.x | own project on spring-boot-2.7.x (declared org.springframework@5.3.39) | open | 3 | 0 | 0% | 1 | 0 | 3 | 0 |  |  | not claimed |  |  |  |  |  |  |  |  |  |  |  |
| org.springframework:spring-jms | 5.3.39 | spring-boot-2.7.x, spring-framework-5.3.x | own project on spring-boot-2.7.x (declared org.springframework@5.3.39) | open | 1 | 0 | 0% | 0 | 0 | 1 | 0 |  |  | not claimed |  |  |  |  |  |  |  |  |  |  |  |
| org.springframework:spring-web | 5.3.39 | spring-boot-2.7.x, spring-framework-5.3.x, spring-security-5.7.x | own project on spring-boot-2.7.x (declared org.springframework@5.3.39) | open | 1 | 0 | 0% | 1 | 0 | 1 | 0 |  |  | not claimed |  |  |  |  |  |  |  |  |  |  |  |
| org.springframework:spring-webflux | 5.3.39 | spring-boot-2.7.x, spring-framework-5.3.x | own project on spring-boot-2.7.x (declared org.springframework@5.3.39) | open | 5 | 0 | 0% | 10 | 0 | 5 | 0 |  |  | not claimed |  |  |  |  |  |  |  |  |  |  |  |
| org.springframework:spring-webmvc | 5.3.39 | spring-boot-2.7.x, spring-framework-5.3.x | own project on spring-boot-2.7.x (declared org.springframework@5.3.39) | open | 6 | 0 | 0% | 9 | 0 | 6 | 0 |  |  | not claimed |  |  |  |  |  |  |  |  |  |  |  |
| org.springframework:spring-websocket | 5.3.39 | spring-boot-2.7.x, spring-framework-5.3.x | own project on spring-boot-2.7.x (declared org.springframework@5.3.39) | open | 1 | 0 | 0% | 1 | 0 | 1 | 0 |  |  | not claimed |  |  |  |  |  |  |  |  |  |  |  |
| org.yaml:snakeyaml | 1.30 | spring-boot-2.7.x | listed by the BOM at 1.30 | open | 6 | 0 | 0% | 1 | 0 | 6 | 0 |  |  | not claimed |  |  |  |  |  |  |  |  |  |  |  |
