# 01. Unstoppable DeFi

**Track id:** `defi` · **Tagline:** Markets that never close

Build exchanges, perps, lending, vaults and trading agents that settle across chains through NEAR Intents, with no custodian and nobody who can switch it off.

**Lean on:** Trading, NEAR Intents, Chain Signatures

## Start here

- [1Click API quickstart](https://docs.near-intents.org/integration/distribution-channels/1click-api/quickstart)
- [Chain Signatures getting started](https://docs.near.org/chain-abstraction/chain-signatures/getting-started)
- [Rhea guide](https://guide.rhea.finance/)
- [Agent API overview](https://docs.agentsonintents.com/integration/agent-api/overview)
- [Aurora Intents](https://intents.aurora.dev/)

## Prompt

```text
Track: Unstoppable DeFi (id: defi).

Build [a cross-chain DCA vault]. A user deposits USDC from any chain NEAR Intents supports, picks a target asset (BTC, ETH or NEAR) and a schedule. On each interval the app requests a quote from the 1Click API, rejects it if slippage beats the user's limit, and executes the swap so the asset lands in the user's own address on the target chain.

Requirements:
- Use the near-intents agent skill and the 1Click API for quotes, deposits and status tracking. Handle REFUNDED and FAILED statuses and show them in the UI.
- Show the user where their funds sit at every step.
- A small web UI: deposit, schedule, and a history of executed buys with explorer links.
- A dry-run mode that fetches real quotes without executing, so judges can try it with no funds.
- Stretch: have a NEAR contract own the vault and use Chain Signatures to control a derived BTC address directly.

Read the 1Click quickstart first and tell me which parts of this design it already handles. Then propose a file layout and wait for my OK.
```
