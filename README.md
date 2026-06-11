# skills

Reusable agent skills (Anthropic `SKILL.md` format) for the SDLC microservice-generation workflow.
Each skill is a folder containing a `SKILL.md` with frontmatter (`name`, `description`, `version`,
`created`, `updated`) and body sections: **When to Use · Procedure · Patterns · Anti-Patterns ·
Tool Selection · Validation Rules · RAG Sources**.

Skills are stack-specific by design; agents stay tech-agnostic and activate the right skill from the
TSA (e.g. `messaging.broker = Kafka` → kafka skill).

## Catalog

### Cross-cutting / framework
- `adr-microservices-blueprint` — architecture decision blueprint (stack resolved from the TSA)
- `java17-springboot3-best-practices` — JVM/Spring Boot coding standards (Java 17 / Spring Boot 3.x)
- `build-toolchain-alignment` — align the build/runtime toolchain to the TSA version
- `domain-service-coreframework-guidelines` — domain-service core-framework rules
- `legacy-sql-to-modern-jpa-transformation` — legacy SQL → JPA migration
- `compilation-error-triage` — build/compile error triage
- `spring-boot-3-test-stabilization` — test stabilization (Spring Boot 3.x / Java 17)
- `microservice-iteration-handoff` — iteration handoff

### Application agent
- `ddd` · `rest-api-design` · `spring-boot` · `event-modeling` · `testing`

### Messaging agent
- `kafka` · `aws-sqs` · `azure-service-bus` · `event-contract` · `outbox-pattern`

### Database agent
- `postgresql` · `oracle` · `mongodb` · `jpa` · `flyway` · `data-modeling`

### Security agent
- `oauth2` · `jwt` · `oidc` · `zero-trust` · `secrets-management`
