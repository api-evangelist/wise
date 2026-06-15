# Wise (wise)

Wise (formerly TransferWise) provides cross-border payments and multi-currency accounts for personal and business customers. The Wise Platform API exposes profiles, balances, transfers, recipients, quotes, multi-currency accounts, cards, statements, and webhooks.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/wise/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/wise/refs/heads/main/apis.yml)

## Tags

- Payments
- FX
- Cross-Border
- Banking
- Multi-Currency

## Timestamps

- **Created:** 2026-05-08
- **Modified:** 2026-05-30

## APIs

### Wise Profiles API

Manages Wise user identity records. A profile represents either a personal or business entity that owns balances, can send and receive money, and can hold recipients. Profiles are the root resource that other Wise Platform API calls are scoped against.

- **Human URL:** [https://docs.wise.com/api-docs/api-reference/profile](https://docs.wise.com/api-docs/api-reference/profile)
- **Base URL:** `https://api.wise.com/v2`

#### Tags

- Profiles
- Identity
- KYC

#### Properties

- [Documentation](https://docs.wise.com/api-docs/api-reference/profile)
- [Sandbox](https://api.sandbox.transferwise.tech)
- [OpenAPI](openapi/wise-platform-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/wise-platform.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/wise-platform.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Wise Recipients API

Manages beneficiary bank account records. Recipients store the destination account details (name, currency, account number, routing/IBAN/SWIFT details) used as the target of a transfer. The API supports creating, retrieving, listing, and deleting recipient accounts across 70+ supported currencies.

- **Human URL:** [https://docs.wise.com/api-docs/api-reference/recipient](https://docs.wise.com/api-docs/api-reference/recipient)
- **Base URL:** `https://api.wise.com/v1`

#### Tags

- Recipients
- Beneficiaries
- Bank Accounts

#### Properties

- [Documentation](https://docs.wise.com/api-docs/api-reference/recipient)
- [OpenAPI](openapi/wise-platform-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/wise-platform.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/wise-platform.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Wise Quotes API

Calculates the exchange rate, fees, and estimated delivery time for a prospective transfer between two currencies. A quote pins the FX rate for a short window and is a required prerequisite to creating a transfer. Supports source-amount, target-amount, and pay-in option variations.

- **Human URL:** [https://docs.wise.com/api-docs/api-reference/quote](https://docs.wise.com/api-docs/api-reference/quote)
- **Base URL:** `https://api.wise.com/v3`

#### Tags

- Quotes
- FX
- Pricing

#### Properties

- [Documentation](https://docs.wise.com/api-docs/api-reference/quote)
- [OpenAPI](openapi/wise-platform-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/wise-platform.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/wise-platform.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Wise Transfers API

Creates and tracks cross-border money movements. A transfer ties a quote to a recipient and is funded from a source balance or pay-in method. The API exposes create, fund, cancel, list, and detail operations along with status events.

- **Human URL:** [https://docs.wise.com/api-docs/api-reference/transfer](https://docs.wise.com/api-docs/api-reference/transfer)
- **Base URL:** `https://api.wise.com/v1`

#### Tags

- Transfers
- Payments
- Cross-Border

#### Properties

- [Documentation](https://docs.wise.com/api-docs/api-reference/transfer)
- [OpenAPI](openapi/wise-platform-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/wise-platform.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/wise-platform.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Wise Balances API

Manages multi-currency balances held inside a profile. Supports listing balances, retrieving the available and reserved amounts per currency, opening and closing currency balances, and moving funds between balances within the same profile.

- **Human URL:** [https://docs.wise.com/api-docs/api-reference/balance](https://docs.wise.com/api-docs/api-reference/balance)
- **Base URL:** `https://api.wise.com/v4`

#### Tags

- Balances
- Multi-Currency
- Wallets

#### Properties

- [Documentation](https://docs.wise.com/api-docs/api-reference/balance)
- [OpenAPI](openapi/wise-platform-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/wise-platform.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/wise-platform.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Wise Multi-Currency Account API

Provisions local bank account details (account number / routing / IBAN / SWIFT) for a profile across the supported receiving currencies, allowing a customer to receive money like a local in 56+ currencies.

- **Human URL:** [https://docs.wise.com/api-docs/api-reference/multi-currency-account](https://docs.wise.com/api-docs/api-reference/multi-currency-account)
- **Base URL:** `https://api.wise.com/v1`

#### Tags

- Multi-Currency Account
- Receive Money
- Local Bank Details

#### Properties

- [Documentation](https://docs.wise.com/api-docs/api-reference/multi-currency-account)
- [OpenAPI](openapi/wise-platform-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/wise-platform.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/wise-platform.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Wise Statements API

Generates and downloads transaction statements for a balance over an arbitrary date range. Output formats include JSON, CSV, PDF, and MT940, supporting reconciliation and accounting workflows.

- **Human URL:** [https://docs.wise.com/api-docs/api-reference/balance-statement](https://docs.wise.com/api-docs/api-reference/balance-statement)
- **Base URL:** `https://api.wise.com/v1`

#### Tags

- Statements
- Reporting
- Accounting

#### Properties

- [Documentation](https://docs.wise.com/api-docs/api-reference/balance-statement)
- [OpenAPI](openapi/wise-platform-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/wise-platform.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/wise-platform.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Wise Cards API

Issues, lists, and manages Wise debit cards linked to a profile balance. Includes operations for retrieving card details, freezing/unfreezing, replacing cards, and managing spending controls.

- **Human URL:** [https://docs.wise.com/api-docs/api-reference/card](https://docs.wise.com/api-docs/api-reference/card)
- **Base URL:** `https://api.wise.com/v3`

#### Tags

- Cards
- Issuing
- Spending Controls

#### Properties

- [Documentation](https://docs.wise.com/api-docs/api-reference/card)
- [OpenAPI](openapi/wise-platform-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/wise-platform.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/wise-platform.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Wise Webhooks API

Subscribes a partner application to event notifications for transfers, balances, cards, and profile-state changes. Supports creating, listing, and deleting webhook subscriptions and verifying signed payloads.

- **Human URL:** [https://docs.wise.com/api-docs/api-reference/subscription](https://docs.wise.com/api-docs/api-reference/subscription)
- **Base URL:** `https://api.wise.com/v3`

#### Tags

- Webhooks
- Events
- Notifications

#### Properties

- [Documentation](https://docs.wise.com/api-docs/api-reference/subscription)
- [OpenAPI](openapi/wise-platform-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/wise-platform.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/wise-platform.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [AsyncAPI](asyncapi/wise-webhooks-asyncapi.yml) — [AsyncAPI Specification](https://www.asyncapi.com/docs/reference/specification/latest)

### Wise Simulation API

Sandbox-only endpoints for advancing the lifecycle of test transfers (simulating funding, processing, completion, and failure paths) without moving real money. Used to exercise integration logic end-to-end against api.sandbox.transferwise.tech.

- **Human URL:** [https://docs.wise.com/api-docs/api-reference/simulation](https://docs.wise.com/api-docs/api-reference/simulation)
- **Base URL:** `https://api.sandbox.transferwise.tech`

#### Tags

- Simulation
- Sandbox
- Testing

#### Properties

- [Documentation](https://docs.wise.com/api-docs/api-reference/simulation)
- [OpenAPI](openapi/wise-platform-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/wise-platform.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/wise-platform.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [GitHub Organization](https://github.com/transferwise)
- [LinkedIn](https://www.linkedin.com/company/wiseaccount)
- [Website](https://wise.com/)
- [Documentation](https://docs.wise.com/)
- [Sandbox](https://api.sandbox.transferwise.tech)
- [Plans](plans/wise-plans-pricing.yml)
- [Rate Limits](rate-limits/wise-rate-limits.yml)
- [Fin Ops](finops/wise-finops.yml)
- [L L Ms Txt](https://docs.wise.com/llms.txt)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
