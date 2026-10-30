# 05. AI Swarms

**Track id:** `swarms` · **Tagline:** Many agents, one economy

Build coordination markets, bidding, collective purchasing, intent-based settlement and economies that emerge between agents.

**Lean on:** Multi-agent systems, NEAR Intents, sub-accounts

## Start here

- [What are intents](https://docs.near-intents.org/getting-started/what-are-intents)
- [Tools for AI agents](https://docs.near.org/getting-started/tools-for-ai)
- [NEAR MCP server](https://github.com/nearai/near-mcp)
- [Top Level Accounts](https://nearaccounts.com/)
- [Agent API overview](https://docs.agentsonintents.com/integration/agent-api/overview)

## Prompt

```text
Track: AI Swarms (id: swarms).

Build [a group-buying swarm]. Buyer agents each represent one user who wants [GPU hours]. They find each other, pool their demand, and run a sealed-bid round against seller agents. The winning bid settles through NEAR Intents and each buyer pays only its share.

Requirements:
- Each agent gets its own sub-account under one parent (buyer-1.swarm.testnet, seller-3.swarm.testnet and so on), so every action on chain traces back to a specific agent.
- A coordinator contract or service that opens a round, collects sealed bids, reveals them and picks a winner. Write down the rules in RULES.md before writing code.
- A simulation mode with 20 buyers and 5 sellers using scripted strategies, so the market runs without any LLM calls.
- A live page showing rounds, bids, clearing price and who got what.

Start with RULES.md and a sequence diagram of one round in text. Wait for my OK before writing contracts.
```
