# DEC-2026-009 — Canonical Lilith Repository

**Status:** Accepted  
**Date:** 2026-08-02  
**Authority:** John

## Decision

`jonsal30/lilith-core` is the canonical human-readable repository for Lilith’s identity, architecture, operating doctrine, context map, accepted decisions, workflows, and current state.

`jonsal30/openhands-Lilith-` is not the source of truth. It may remain an experimental or future execution runtime based on OpenHands.

## Operating Model

- ChatGPT Source-of-Truth project: conversation, reasoning, decisions, and commands.
- `lilith-core`: durable canonical truth and version history.
- Connected runtimes and tools: execution.
- Future database: live operational state and transactions.

## Rules

- `main` represents accepted canonical truth.
- Major architectural changes should be proposed through branches and pull requests.
- Ancillary conversations are supporting evidence until reconciled.
- Newer information does not automatically override accepted truth.
- Sensitive raw records and credentials must not be committed.

## Security Requirement

The repository should be made private before sensitive operational context is added, and its history should be audited for secrets or private data.