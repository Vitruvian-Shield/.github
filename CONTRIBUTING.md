# Contributing to Vitruvian Shield Repositories

This repository is part of the Vitruvian Shield platform, a regulated Software as a Medical Device system under EU MDR, IEC 62304 and 21 CFR Part 11. Contributions must respect both engineering best practice and the regulatory quality system.

## Before you start

Read three documents first: this CONTRIBUTING guide, the repository SECURITY.md, and the Software Development Plan for this repository stored in the QMS Confluence space under Software Development Plans. If the Software Development Plan does not exist for this repository, raise an issue tagged type-regulatory before contributing.

## Branching model

- main holds production-ready code and is protected.
- develop holds the next release and is protected.
- Feature branches are named feat/short-description, fix/short-description, chore/short-description or docs/short-description.
- Release branches are named release/YYYY.MM.x.

## Commit messages

Follow Conventional Commits:
type(scope): short summary
Types: feat, fix, docs, chore, refactor, test, perf, security, regulatory.
For Class B or Class C changes add a Regulatory-Impact trailer describing the risk class and the affected control.

## Pull requests

Every pull request requires:
- Green CI (lint, test, SAST, dependency scan, secret scan, SBOM generation)
- Review from at least two code owners declared in CODEOWNERS
- A description linking to the issue or requirement it implements
- Updated unit tests and, where relevant, integration tests
- Updated documentation in the repository README or the relevant Confluence page
- For Class B or Class C components, a note explaining the regulatory impact and the traceability link to the risk analysis entry

Pull requests that add or modify authentication, authorisation, audit trail, electronic signature, randomisation, dosing, consent or investigational product accountability logic require explicit CTO approval before merge.

## Code style

JavaScript and TypeScript follow the repository ESLint and Prettier configuration. Python follows Ruff and Black defaults. Go follows gofmt and go vet. Flutter and Dart follow flutter analyze defaults. Do not reformat unrelated files in a functional pull request.

## Tests

Every merged change must either add a test, modify an existing test to match the new behaviour, or carry an explicit Test-Exemption trailer in the commit message explaining why a test is not applicable. Class B and Class C components require unit test coverage of at least 80 percent on changed lines.

## Secrets

Do not commit credentials. Use environment variables loaded from a secret manager. If you believe a secret has been committed, stop and email security@vitruvianshield.com immediately; do not force-push.

## Signing

Commits must be signed (GPG or SSH). Unsigned commits are rejected by branch protection.

## Questions

Ask in the Vitruvian Shield Confluence space Engineering Handbook, or open a discussion in this repository.
