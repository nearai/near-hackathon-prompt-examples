# 06. AI Security & Defense

**Track id:** `security` · **Tagline:** Trust, but verify

Build spending limits, policy engines, sandboxed wallets, reputation and scam detection. Give AI money without handing it the keys to everything.

**Lean on:** Agent security, function-call keys, TEE attestation

## Start here

- [Access keys](https://docs.near.org/protocol/accounts-contracts/access-keys)
- [OutLayer getting started](https://app.outlayer.ai/docs/getting-started)
- [NEAR AI Cloud verification](https://docs.near.ai/cloud/verification)
- [Agent API policies & limits](https://docs.agentsonintents.com/integration/agent-api/policies-and-limits)

## Prompt

```text
Track: AI Security & Defense (id: security).

Build [a counterparty check for agents that pay]. Before an agent sends funds or calls a contract, it asks this service about the receiver. The service returns allow, warn or block, plus the reasons.

Signals to score (add more if the docs suggest good ones):
- account age and activity history
- whether the receiver is a contract, and whether its code changed recently
- prior interactions between this agent and the receiver
- a shared blocklist that other agents can report to, with evidence attached

Requirements:
- An agent-side wrapper that refuses to sign when the answer is block and asks a human when it's warn.
- The agent signs with a function-call access key scoped to one contract, never a full-access key. Explain the limits of that key in the README.
- An attack demo: a script where a prompt-injected agent tries to pay a known-bad address and gets stopped. Show the log.

List the data sources you'd use for each signal and how you'd get them, then wait for my OK.
```

## Note

Read the caveats on the access keys page. An account that holds only function-call keys can't transfer NEAR or add keys, and it can lock itself out if the gas allowance runs out.
