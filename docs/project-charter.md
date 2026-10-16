# Project charter

## Learning objective

Establish a Spring Boot/JPA project foundation and begin modeling a user for a course-based commerce exercise.

## Scope represented today

- Maven and Java 21 project setup.
- Spring Boot application bootstrap.
- H2 in-memory test/development profile.
- Initial user model and a context-load test.

## Explicitly not implemented

- Product catalog, categories, carts, orders, payments, inventory, or customer workflows.
- REST endpoints, service layer, persistence repositories, and database migrations.
- Authentication, authorization, password handling, validation, error API, or audit trail.
- Deployment, CI, monitoring, support, or production-data design.

## Ownership and decision gate

This is a personal learning archive. The owner should either archive it as a checkpoint or approve a new, separately scoped commerce implementation. It must not be represented as a completed DSCommerce project.

## Completion criteria for a future implementation

1. Define a product/domain brief and API contract.
2. Model persistence relationships correctly and add migrations/seeds.
3. Add validation, authentication/authorization, and secure password lifecycle if user accounts remain in scope.
4. Implement tests across domain, repository, and API layers.
5. Add CI, environment configuration, observability, and deployment evidence.
