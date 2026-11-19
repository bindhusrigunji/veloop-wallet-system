# VELOOP Rewards

A rewards and wallet management demo application built to demonstrate user wallets, reward balances, transactions, withdrawals, and admin analytics.

## Live Application

https://veloop-rewards-fpii.onrender.com/

## GitHub Repository

https://github.com/bindhusrigunji/veloop-wallet-system

## Features

- User login and dashboard
- Wallet balance management
- Spendable VEs and Staked SVEs
- Gems, Tokens, and Spins
- Transaction history
- Withdrawal request workflow
- Multiple payout options displayed
- Admin dashboard and analytics
- KPI reporting and CSV export

## Technology Stack

- React
- TypeScript
- Tailwind CSS
- Node.js
- Express
- MongoDB / MongoDB Memory Server fallback

## Demo Environment

**Data Origin:** SIMULATED_DEMO_DATA

**Production Database:** NOT CONNECTED

The current application uses seeded demo data and an embedded MongoDB Memory Server fallback. It is intended for demonstration and technical evaluation.

Actual production database and payment gateway integrations have not been completed or verified.

## Documentation

| File | Description |
|---|---|
| TEST_EVIDENCE_REPORT.md | Test results and limitations |
| KPI_Validation_Report.md | Validation status of 46 KPIs |
| Analytics_Specification.md | Analytics features and limitations |
| ER_Diagram_Report.md | Main entities and relationships |
| PRODUCTION_ROADMAP.md | Pending production requirements |

## Test Summary

- Primary test suite: 21 PASS
- Failed tests: 0
- Not testable: 2
- Security checks: 6 PASS
- KPI checks: 6 PASS
- TypeScript lint: PASS
- Vite production build: PASS
- Browser E2E: Not executed

## Production Roadmap

Production readiness requires:

1. Production database configuration
2. Actual payment gateway integration
3. Referral tracking implementation
4. KPI business confirmation
5. Browser end-to-end testing
6. Production security verification

## Project Status

This repository contains a deployed demo application and supporting technical documentation. Production integrations and final business validation remain pending.
