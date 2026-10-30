# 03. Privacy & Private AI

**Track id:** `privacy` · **Tagline:** Private by design

Explore confidential computation, private finance and AI that protects sensitive data. Build intelligence without exposure.

**Lean on:** Private AI, TEE, NEAR AI Cloud

## Start here

- [NEAR AI Cloud quickstart](https://docs.near.ai/cloud/quickstart)
- [NEAR AI Cloud verification docs](https://docs.near.ai/cloud/verification)
- [Verification example repo](https://github.com/near-examples/nearai-cloud-verification-example)
- [Agent API overview](https://docs.agentsonintents.com/integration/agent-api/overview)

## Prompt

```text
Track: Privacy & Private AI (id: privacy).

Build [a private expense auditor]. A user uploads receipts or a bank statement, a model on NEAR AI Cloud categorizes the spending and flags anything unusual, and the app proves the analysis ran inside a TEE.

Requirements:
- Call NEAR AI Cloud through its OpenAI-compatible API (base URL https://cloud-api.near.ai/v1, API key in .env). Choose a TEE-hosted model from the models endpoint.
- Fetch the attestation report with a fresh random nonce and verify it the way the verification docs describe. Show a "Verified" panel listing what was checked.
- Keep nothing server-side after a response returns. Say so in the README and make it obvious in the code.
- Ship fictional sample documents so judges can run it without real data.

Use the near-ai-cloud agent skill. Start with a minimal script that sends one completion and verifies attestation, show me its output, then build the UI.
```
