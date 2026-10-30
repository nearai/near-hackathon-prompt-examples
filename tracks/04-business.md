# 04. Autonomous Business

**Track id:** `business` · **Tagline:** The company of one, or none

Build AI-native businesses that run their own treasury, sales, procurement, cross-chain payments through NEAR Intents and revenue sharing. Humans only set the constraints.

**Lean on:** AI agents, NEAR Intents, Chain Signatures

## Start here

- [AI and NEAR](https://docs.near.org/ai/introduction)
- [OutLayer getting started](https://app.outlayer.ai/docs/getting-started)
- [1Click API](https://docs.near-intents.org/integration/distribution-channels/1click-api/about-1click-api)
- [Agent API overview](https://docs.agentsonintents.com/integration/agent-api/overview)
- [PingPay Agent Pay facilitator](https://pingpay.gitbook.io/docs/pingpay-api/agent-pay-facilitator)

## Prompt

```text
Track: Autonomous Business (id: business).

Build [a one-agent research shop]. The agent sells short market reports. Customers pay in whatever token they hold through NEAR Intents, the agent buys its own inference from NEAR AI Cloud, and a fixed share of every sale goes to a contributors' account automatically. I set the rules in one config file and the agent runs everything else.

Rules the agent must obey (config.yaml):
- maximum inference spend per day
- minimum price per report
- revenue split percentages
- a kill switch I can flip at any time

Requirements:
- Give the agent its own NEAR account. Never store a full-access key in plain text; use OutLayer agent custody or a scoped function-call key.
- Log every sale, cost and payout to a public ledger page.
- A demo mode that runs one full loop on testnet, from sale to payout, in under two minutes.

Read the AI and NEAR docs and the OutLayer docs first. Then sketch the architecture in text and wait for my OK.
```
