# Architecture and data-model boundaries

## Current components

| Component | Current responsibility |
| --- | --- |
| `DscommerceApplication` | Spring Boot application entry point. |
| `entities/User` | Initial JPA entity with basic personal/contact fields. |
| `application*.properties` | Activates an H2-backed test profile and Hibernate diagnostics. |
| `DscommerceApplicationTests` | Verifies that the Spring context loads. |
| `pom.xml` | Maven dependencies and Java target configuration. |

## Current data boundary

The project uses an in-memory H2 database for the test profile. Data disappears when the process ends. There are no migrations, fixtures, repositories, or defined database contract.

The current `User` entity includes a raw string-array roles field. That is not an established relational mapping or authorization model. Any continuation needs to explicitly design roles, password storage, validation, data privacy, and database schema before persisting user data.

## Operational limitations

- No HTTP endpoint has been implemented despite web dependencies.
- The H2 console and SQL logging are useful for local learning, not a production posture.
- No secrets, external services, queues, file storage, or deployment topology are defined.
