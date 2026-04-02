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
