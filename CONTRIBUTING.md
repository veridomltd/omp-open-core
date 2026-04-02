# Contributing to OMP Open Core

Thank you for your interest in contributing to OMP Open Core.

OMP Open Core is the free and open-source reference implementation and verification toolkit for the Operating Model Protocol (OMP™). This repository exists to make OMP-conformant Proof-Points independently verifiable without reliance on Veridom infrastructure.

## Scope of this repository

This repository accepts contributions to the open implementation layer only.

### In scope
- reference validator
- machine-readable schemas
- Watchtower reference framework
- test fixtures and verification examples
- interoperability documentation
- implementation notes tied to published OMP specifications

### Out of scope
- institutional deployment tooling
- commercial consulting artifacts
- production Proof-Point generation infrastructure
- customer-specific domain configurations
- proprietary diagnostic or deployment systems

## Before contributing

Please do three things first:

1. Read the `README.md`
2. Check open issues to see whether the work is already being discussed
3. Open an issue before starting large changes

For bug fixes, schema clarifications, documentation improvements, and tests, you can usually proceed directly.  
For new features, architectural changes, or changes affecting protocol interpretation, open an issue first.

## Types of contributions we welcome

We welcome contributions in the following areas:

- **Validator development**
  - chain integrity verification
  - RFC 3161 timestamp verification
  - schema conformance checks
  - CLI usability and error handling

- **Schemas**
  - Audit Trace schema
  - Interaction schema
  - validation rules
  - schema examples and fixtures

- **Watchtower framework**
  - reference implementation improvements
  - configuration examples
  - test coverage
  - evaluation trace clarity

- **Documentation**
  - interoperability guides
  - developer documentation
  - protocol clarification
  - examples for auditors, insurers, and regulators

- **Testing**
  - conformance tests
  - broken-chain test cases
  - invalid timestamp test cases
  - malformed schema fixtures
  - cross-version compatibility tests

## Contribution principles

### 1. Independent verifiability comes first
Changes must preserve the ability for a third party to verify an OMP-conformant record without access to Veridom systems.

### 2. Keep protocol and product separate
This repository is for the open reference layer, not the commercial implementation layer.

### 3. Determinism over convenience
If a change weakens deterministic interpretation or introduces ambiguity in routing, verification, or schema meaning, it is unlikely to be accepted.

### 4. Explicit is better than implicit
Validation rules, assumptions, and edge-case behavior should be documented clearly.

### 5. Standards alignment matters
Where possible, contributions should remain consistent with the published OMP specification, related Internet-Drafts, and the repository’s stated licensing model.

## How to contribute

### For small changes
- Fork the repository
- Create a branch
- Make the change
- Open a pull request with a clear description

### For larger changes
Open an issue first with:
- the problem being solved
- why the current implementation is insufficient
- the proposed change
- any effect on protocol interpretation, validator behavior, or interoperability

## Pull request guidance

Please keep pull requests focused.

A good pull request should include:
- a clear title
- a short explanation of what changed
- the reason for the change
- tests, examples, or documentation updates where relevant

If your pull request changes behavior, include:
- before/after behavior
- sample inputs and outputs
- any compatibility impact

## Coding and documentation expectations

### Code
- prefer readable, maintainable implementations
- include comments where protocol behavior may be non-obvious
- add or update tests for new logic
- avoid unnecessary dependencies

### Documentation
- write for technically literate readers who may not know OMP in advance
- define terms precisely
- avoid marketing language in technical docs
- keep examples realistic and auditable

## Issues

When opening an issue, please label the problem as clearly as possible, for example:
- bug
- schema clarification
- validator enhancement
- documentation
- interoperability
- standards alignment

If reporting a bug, include:
- expected behavior
- actual behavior
- steps to reproduce
- sample record or fixture if safe to share

## Licensing

By contributing to this repository, you agree that your contributions will be released under the repository’s licenses:

- **Software and machine-readable artifacts:** Apache License 2.0
- **Documentation:** CC BY 4.0 where indicated

See the `LICENSE` file and repository notices for details.

## Security and sensitive disclosures

Do not post:
- private customer data
- confidential deployment details
- live institutional records
- production credentials or secrets

If you believe you have found a security-sensitive issue in the validator or verification workflow, do not open a public issue. Contact the maintainers privately using the repository contact details once published.

## Maintainers

This repository is maintained by Veridom Ltd.

Initial maintainers:
- Oluropo Apalowo
- Tolulope Adebayo

Maintainer information may be updated as the project matures.

## Final note

The goal of OMP Open Core is not just usable code.  
It is trustworthy, inspectable, independently verifiable infrastructure for AI decision accountability.

Contributions that strengthen that goal are welcome.
