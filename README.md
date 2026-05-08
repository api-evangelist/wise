# Wise (wise)

Wise (formerly TransferWise) provides cross-border payments and multi-currency accounts for personal and business customers. The Wise Platform API exposes profiles, balances, transfers, recipients, quotes, multi-currency accounts, cards, statements, and webhooks.

**URL:** [Visit APIs.json URL](https://raw.githubusercontent.com/api-evangelist/wise/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=wise-api-evangelist&utm_content=repo)

## Type

- **x-type:** company

## Tags

- Payments, FX, Cross-Border, Banking, Multi-Currency

## Timestamps

- **Created:** 2026-05-08
- **Modified:** 2026-05-08

## APIs

| API | Description |
|---|---|
| Wise Profiles API | Personal and business identity records that own balances, transfers, and recipients. |
| Wise Recipients API | Beneficiary bank account records used as transfer destinations across 70+ currencies. |
| Wise Quotes API | Exchange rate, fee, and delivery-time calculation; required prerequisite for a transfer. |
| Wise Transfers API | Create, fund, cancel, and track cross-border transfers. |
| Wise Balances API | Multi-currency wallet balances scoped to a profile. |
| Wise Multi-Currency Account API | Provisions local bank account details (USD/EUR/GBP/AUD/NZD/etc.) for receiving funds. |
| Wise Statements API | Transaction statements per balance over arbitrary date ranges in JSON, CSV, PDF, or MT940. |
| Wise Cards API | Issue and manage Wise debit cards bound to a profile balance. |
| Wise Webhooks API | Subscriptions for transfer, balance, card, and profile-state events. |
| Wise Simulation API | Sandbox-only endpoints to advance test-transfer lifecycles without moving real money. |

## Common Properties

- [Website](https://wise.com/)
- [Documentation](https://docs.wise.com/)
- [Sandbox](https://api.sandbox.transferwise.tech)
- [Plans](plans/wise-plans-pricing.yml) - API Commons Plans 0.1
- [RateLimits](rate-limits/wise-rate-limits.yml) - API Commons Rate Limits 0.1
- [FinOps](finops/wise-finops.yml) - FOCUS-aligned FinOps Framework 1.0

## Plans (Pay-As-You-Go)

Wise does not sell tiered API plans. The Platform API is free; revenue is per-transaction.

- **Personal Account** - Free; per-transfer fixed + percentage fee plus FX markup over the mid-market rate.
- **Business Account** - One-time account-opening fee in most regions (~$31 US / GBP 45 UK), then the same per-transfer economics; adds batch payments, multi-user RBAC, and accounting integrations.
- **Wise Platform (Embedded)** - Custom-negotiated partner offering for banks, fintechs, and software platforms.

## Rate Limits

- 429 Too Many Requests applied at the account level with dynamic ceilings; no published RPS.
- Authentication endpoints throttled more aggressively.
- Webhooks retry with exponential backoff up to ~14 attempts.
- Use the X-idempotence-uuid header on transfer creation and funding calls.

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
