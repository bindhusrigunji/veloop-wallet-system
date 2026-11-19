# VELOOP Rewards — Analytics Specification

## 1. Purpose

This document describes the analytics dashboard, KPI calculations, data sources, and known limitations of the VELOOP Rewards application.

## 2. Current Data Environment

- Data Origin: SIMULATED_DEMO_DATA
- Production Database: NOT CONNECTED
- Current Data: Seeded demo dataset
- Analytics Mode: Demo / Sandbox

All dashboard metrics currently represent simulated demo records. They must not be interpreted as actual VELOOP production performance.

## 3. Analytics Features

The application provides analytics for monitoring:

- Wallet balances and transactions
- User activity
- Reward credits
- Withdrawals and payout activity
- Transaction history
- KPI summaries
- Date-range filtering
- CSV export

## 4. KPI Coverage

The project defines 46 KPIs.

| Status | Count |
|---|---:|
| Validated | 26 |
| Needs Business Confirmation | 12 |
| Not Testable | 8 |
| Total | 46 |

The 26 validated KPIs have implementation or calculation support in the current demo environment.

The 12 KPIs requiring business confirmation need stakeholder approval of their definitions and calculation rules.

The 8 untestable KPIs require additional source data, schema, or telemetry.

## 5. Calculation and Filtering

Analytics calculations use the available demo collections and fields.

Date filters are intended to restrict analytics to the selected reporting period.

The dashboard supports:

- All Time
- Last 7 Days
- Last 30 Days

CSV export provides a downloadable representation of the available KPI data.

Exact KPI formulas and source-field mappings must be reviewed against the approved VELOOP business definitions before production use.

## 6. Data Integrity and Separation

The application identifies its current data source as SIMULATED_DEMO_DATA.

Production database connectivity is not established.

Demo records and production records must remain separate. No production data is claimed in this report.

## 7. Known Limitations

- Production database integration is pending.
- Actual payment gateway data is not connected.
- Some KPI definitions need business confirmation.
- Some KPI source schemas and telemetry are unavailable.
- Production-scale analytics performance has not been verified.
- Browser end-to-end testing remains pending.

## 8. Production Roadmap

1. Connect and verify the approved production database.
2. Confirm all 46 KPI definitions with VELOOP stakeholders.
3. Implement missing source schemas and telemetry.
4. Validate calculations using approved production data.
5. Test date filters and CSV exports.
6. Perform browser end-to-end and security testing.
7. Obtain stakeholder approval before production reporting.

## 9. Conclusion

The current analytics dashboard demonstrates KPI reporting using simulated demo data.

Production integration, business confirmation, and additional validation are required before the analytics can be considered production-ready.
