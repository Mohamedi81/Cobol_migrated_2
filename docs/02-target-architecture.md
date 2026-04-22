# Target Java Microservices Architecture

- Services: `customer-service`, `policy-service`, `policy-version-service`, `analytics-service`, `gateway-service`, `common-lib`.
- Tech stack: Java 17, Spring Boot 3, Spring Web, Spring Data JPA, PostgreSQL.
- Communication: REST/JSON between services via the gateway.
- Data: relational schema modeling customers, policies, policy versions, and statistics derived from VSAM/DB2 structures.

More detailed design (entities, endpoints, and COBOL mapping) will be refined in subsequent commits.
