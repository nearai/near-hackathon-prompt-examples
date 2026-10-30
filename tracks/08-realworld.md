# 08. Real-World Money

**Track id:** `realworld` · **Tagline:** Bring the boring money onchain

Build payroll, invoicing, remittances, merchant payments and stablecoin rails for real businesses. Something a normal company could use tomorrow.

**Lean on:** Stablecoins, NEAR Intents, meta transactions

## Start here

- [1Click API quickstart](https://docs.near-intents.org/integration/distribution-channels/1click-api/quickstart)
- [Building a meta transaction relayer](https://docs.near.org/web3-apps/tutorials/meta-transactions)
- [NEP-141 fungible token standard](https://github.com/near/NEPs/blob/master/neps/nep-0141.md)
- [PingPay Agent Pay facilitator](https://pingpay.gitbook.io/docs/pingpay-api/agent-pay-facilitator)

## Note

PingPay's facilitator lets agents pay an x402 paywall in USDC on Base, settling to your NEAR recipient.

## Prompt

```text
Track: Real-World Money (id: realworld).

Build [crypto invoicing for freelancers who don't care about crypto]. A freelancer creates an invoice and gets a link. The client pays from whatever chain and token they already hold. The freelancer receives USDC on NEAR and never buys NEAR for gas.

Requirements:
- Invoice page with amount, due date, line items and a pay button. Payment goes through the 1Click API.
- Gasless for the freelancer: route their transactions through a meta transaction relayer that only pays for calls to our own contract.
- Status updates the freelancer can trust: paid, pending or refunded, with links to the transactions.
- CSV export an accountant could open without asking a single question.

Write the README first as if a bookkeeper will read it. Then build the invoice page and one full paid-invoice flow on testnet before anything else.
```
