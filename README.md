# OMP Open Core

Open reference implementation and verification toolkit for deterministic AI decision accountability.

OMP Open Core is the free and open-source implementation layer for the Operating Model Protocol (OMP™). It enables any institution, regulator, insurer, auditor, or researcher to generate, validate, and independently verify OMP-conformant Proof-Points without dependency on Veridom infrastructure.

## What OMP Open Core provides

This repository contains the public, grantable layer of OMP:

- **Reference validator**  
  Verifies OMP Proof-Point chains for:
  - SHA-256 chain integrity
  - RFC 3161 trusted timestamp authenticity
  - schema conformance

- **Audit Trace schema**  
  Machine-readable schema for the OMP Audit Trace record.

- **Interaction schema**  
  Machine-readable schema for the OMP Interaction input record.

- **Watchtower evaluation framework**  
  Reference implementation of OMP pre-routing enforcement gate logic.

- **Interoperability documentation**  
  Open implementation guides mapping OMP to regulated-domain requirements.

## What OMP is

OMP is a deterministic decision-enforcement protocol with an evidentiary layer.

It classifies each AI-mediated interaction into one of three accountable states:

- **AUTONOMOUS** — no human review required
- **ASSISTED** — human review required before dispatch
- **ESCALATED** — mandatory human intervention triggered

For each interaction, OMP produces a sealed accountability record that can be independently verified by a third party.

## Why this exists

Institutions deploying AI in consequential decisions often cannot produce a per-decision evidence record that a regulator, insurer, court, or auditor can independently verify.

Current tools usually record outputs retrospectively. They do not reliably preserve:

- the decision state at the moment of interaction
- the rule path applied
- the accountability path taken
- tamper-evident proof that the record has remained intact

OMP Open Core exists to close that infrastructure gap.

## Design principles

- **Independent verifiability**  
  Verification must not depend on Veridom’s systems or continued operation.

- **Open implementation**  
  Any party should be able to implement and test the protocol.

- **Domain portability**  
  The same protocol should support credit, legal, insurance, agent oversight, and other regulated domains.

- **Standards alignment**  
  OMP is developed through open technical specification and Internet-Draft publication.

## Repository structure

Planned structure:

```text
schemas/
  audit-trace/
  interaction/

validator/
  cli/
  tests/

watchtower-framework/
  core/
  examples/

docs/
  interoperability/
  architecture/
```

## Status

This repository is in initial public setup.

Current work in progress:

* repository bootstrap
* Apache 2.0 licensing
* schema publication
* validator v1.0 planning
* Watchtower reference framework extraction
* interoperability guide preparation

## Prior specification work

The OMP technical specification is already published through:

* **Zenodo DOI:** `10.5281/zenodo.19140948`
* **IETF Internet-Drafts:** core protocol and domain profiles

This repository is the open implementation and verification layer that makes the published specification usable without vendor dependency.

## Open / commercial boundary

### Open in this repository

* reference validator
* machine-readable schemas
* Watchtower reference framework
* interoperability documentation
* public examples and tests

### Commercial and not included here

* diagnostic agent
* institutional deployment tooling
* implementation consulting
* domain-specific production configuration
* production Proof-Point generation infrastructure
* live deployment operations

## Licensing

* **Software and machine-readable schemas:** Apache License 2.0
* **Documentation and interoperability guides:** CC BY 4.0 where indicated

See [`LICENSE`](./LICENSE).

## Contributing

Contribution guidelines will be added as the public implementation stabilizes.

Early contributors interested in:

* schema review
* RFC 3161 validation workflows
* regulated-domain interoperability
* test corpus design
* IETF-aligned implementation feedback

are welcome to open an issue.

## Contact

* **Veridom Ltd**
* Website: `https://veridom.io`
* Repository: `https://github.com/veridomltd/omp-open-core`

For implementation, standards, or research collaboration, open an issue in this repository.

```
