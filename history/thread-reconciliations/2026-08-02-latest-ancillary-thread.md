# Reconciliation — Latest Ancillary Lilith Thread

**Source thread:** Unsolicited GitHub Spam Warning  
**Last updated:** 2026-08-02  
**Authority:** Supporting evidence; reconciled decisions are recorded separately.

## Relevant Contribution

The thread began with a GitHub issue but produced two durable architectural insights:

1. Lilith should use closed-loop execution rather than stopping at advice.
2. Lilith needs a controlled mobile execution layer for iPhone, voice, messaging, and shortcuts.

## Closed-Loop Execution

The originating example followed this sequence:

**Issue surfaced → Context retrieved → Decision made → John directed closure → GitHub action executed → Closure verified**

This was reconciled into `blueprint/01-operating-doctrine.md`.

## Mobile Operator

The thread proposed adapting prior Message Machine and Ask LLM shortcut work into a governed Lilith subsystem with:

- voice-initiated commands;
- contact resolution;
- incoming-message triage;
- message drafting and sending;
- action extraction and context routing;
- Draft, Trusted, and Campaign permission modes;
- completion verification and logging.

This was reconciled into `blueprint/06-mobile-operator.md` and `DEC-2026-008-mobile-operator.md`.

## Excluded from Canonical Blueprint

The specific unsolicited GitHub issue and its spam details remain operational history. They do not define Lilith’s architecture.

## Reconciliation Classification

- **New doctrine:** closed-loop execution
- **New subsystem:** Lilith Mobile Operator
- **Reused assets:** Message Machine and Ask LLM as reference plumbing
- **Rejected behavior:** random-number messaging, broad unattended replies, plaintext credentials, unrestricted phone-control claims