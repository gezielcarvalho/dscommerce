# Current-state documentation

## Purpose

This repository appears to be the starting point of a DevSuperior DSCommerce learning exercise. It captures initial project setup rather than a functioning e-commerce system.

## Current state

- Runtime: Java 21 with Spring Boot configuration managed by Maven.
- Dependencies: Spring MVC, Spring Data JPA, H2, and test starters.
- Data: one `User` entity; its roles array has not been modeled as a JPA relationship or collection mapping.
- Configuration: active `test` profile uses an in-memory H2 database and enables the H2 console.
- Verification: one Spring context-load test.
- Application surface: no controllers, repositories, services, migrations, fixtures, or commerce features were found.

## Decision

Classify as a formative learning archive. Do not describe it as an e-commerce application, publish it as a portfolio project, or deploy it without an approved product and security redesign.

See the [charter](project-charter.md), [architecture](architecture.md), and [delivery handoff](delivery-and-quality.md).
