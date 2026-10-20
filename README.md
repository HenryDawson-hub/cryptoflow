# CryptoFlow Exchange Prototype

A responsive front-end prototype for a crypto-to-crypto spot exchange.

## Run locally
1. Extract `cryptoflow_exchange.zip`.
2. Open `index.html` in a modern browser. No build step is required.

## Included
- Dark exchange-style dashboard
- Pair selector for BTC/USDT, ETH/USDT, SOL/USDT, BNB/USDT
- Illustrative chart and order book
- Buy/sell form, estimated totals and simulated order list
- Demo login/signup and launch-requirements modals
- Responsive layout

## Critical limitation
This is a front-end demo only. It has no backend, real-time market data, matching engine, user authentication, wallet integration, custody, deposits, withdrawals, KYC, AML, or real order execution. All balances/prices/order book entries are illustrative. Do not accept customer funds or present this prototype as a functioning exchange.

## Production architecture required
- Frontend: React/Next.js or equivalent, strict CSP, HTTPS, secure session handling.
- Backend API: authenticated services, schema validation, rate limiting, audit trails.
- Ledger: append-only double-entry ledger; idempotent transactions; daily reconciliation.
- Trading: tested matching engine, order state machine, market-data ingestion, circuit breakers.
- Custody: institutional custody or audited wallet stack; HSM/MPC where appropriate; withdrawal allowlists, delays, risk checks, hot-wallet limits and offline recovery.
- Security: MFA/passkeys, secrets manager, least privilege, encryption, dependency scanning, SAST/DAST, penetration testing, monitoring, incident response, backups and disaster recovery.
- Compliance: obtain qualified Cambodian legal advice on current licensing/authorization requirements and any cross-border jurisdictions; implement risk-based KYC, AML/CFT, sanctions screening, suspicious-activity escalation, privacy/data-retention policies and customer disclosures as required.
- Operations: customer support, dispute/complaint handling, finance/tax controls, independent security and financial audits, vendor due diligence.

## Suggested launch sequence
1. Validate legal scope and licensing with Cambodian counsel and relevant regulators before handling customer assets.
2. Select custody, KYC/AML, market data and liquidity providers after due diligence.
3. Design threat model, custody/withdrawal policy and ledger invariants.
4. Build backend and automated tests; test against sandbox environments only.
5. Conduct independent security audit, operational drills and reconciliation testing.
6. Launch only after regulatory, security, custody, liquidity and operational gates are signed off.
