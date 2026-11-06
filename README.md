# CyberLab

CyberLab is a local application security learning project built around a practical workflow: reproduce an API authorization flaw, fix it, and verify the fix with a regression test.

**Status** · Design baseline documented. Implementation is planned.

## Foundation

The first milestone is a Spring Boot API, a React dashboard shell, and a reproducible PostgreSQL setup with Docker Compose and Flyway. The safe core will demonstrate server-side role and resource ownership checks.

## First exercise · LAB-001

`LAB-001` will demonstrate broken object-level authorization (BOLA) using two synthetic accounts and their orders. Learners will compare the vulnerable and fixed variants, then run a regression test that verifies the owner can access the order and the other account is denied.

## Authorized use

Intentionally vulnerable exercises are designed for isolated, disposable environments on localhost. Use synthetic data and run exercises only on systems you own or have explicit permission to test. Keep vulnerable services off public interfaces.

## Project documentation

See the [bilingual project overview](docs/CYBERLAB_PROJECT_OVERVIEW.md) for the planned architecture, trust boundaries, module specifications, and roadmap.
