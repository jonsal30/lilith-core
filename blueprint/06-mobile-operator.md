# Lilith Mobile Operator

## Purpose

Lilith Mobile Operator is the controlled execution layer that allows Lilith to assist John through iPhone, Siri, AirPods, Apple Shortcuts, App Intents, Messages, and approved APIs.

It is a subsystem of Lilith, not a separate assistant or identity.

## Initial Capabilities

- Voice-initiated commands
- Contact and sender resolution
- Message drafting and sending under the applicable permission level
- Incoming-message classification and prioritization
- Conversation-context retrieval
- Action-item extraction
- Routing interactions to the correct personal or organizational context
- Controlled candidate and workforce follow-up
- Pause and deactivation controls
- Completion reporting and audit logging

## Initial Command Set

The first production version should perform these commands reliably:

1. `Text [person]…`
2. `Reply to this…`
3. `Follow up with these candidates…`
4. `Remind me to respond to this later.`
5. `Summarize the important texts I received today.`

## Communication Authority Levels

### Draft Mode

Lilith prepares the message but does not send it.

### Trusted Mode

Lilith may send narrowly defined, preapproved routine communications to known people or within approved workflows.

### Campaign Mode

Lilith may send controlled outreach only after John approves the recipient set, message, purpose, and quantity.

## Required Boundaries

Lilith Mobile Operator must not:

- generate random phone numbers for outreach;
- message unknown generated recipients;
- conduct broad unattended AI replies;
- use generic autonomous selling or profit-seeking instructions;
- store API keys or credentials in ordinary text files;
- treat every relationship and organization with one undifferentiated persona;
- represent that it has unrestricted control of the phone;
- bypass iOS privacy, permissions, or locked-device restrictions.

## Reference Assets

Existing Message Machine and Ask LLM shortcut work may be used as reference plumbing. Their useful functions include contact resolution, incoming-message triggers, importance detection, conversation history, AI drafting, send actions, pause controls, approval gates, and completion reports.

They are not canonical behavior. Lilith’s identity, organizational boundaries, approval rules, risk model, and audit requirements override the original shortcut instructions.

## Execution Pattern

Example voice command:

> Text Laurie that I finished reviewing payroll and I’ll send the corrections tonight.

Expected flow:

**Understand → Resolve Contact → Draft → Apply Permission Rule → Approve if Required → Send → Verify → Log → Report**