# VELOOP Rewards — Entity Relationship (ER) Report

## 1. Purpose

This document describes the main data entities and their relationships in the VELOOP Rewards application.

## 2. Main Entities

### User
Stores user account information.

Important fields:
- User ID
- Name
- Email
- Role
- Account status

### Wallet
Stores wallet balances for a user.

Important fields:
- Wallet ID
- User ID
- Spendable VEs
- Staked SVEs
- Gems
- Tokens
- Spins

### Transaction
Stores wallet activity and transaction history.

Important fields:
- Transaction ID
- User ID
- Transaction type
- Amount
- Previous balance
- New balance
- Created date

### Withdrawal
Stores withdrawal requests.

Important fields:
- Withdrawal ID
- User ID
- Amount
- Payout method
- Status
- Created date

### Payout
Stores payout method and payout-related details.

Important fields:
- Payout ID
- User ID
- Payout method
- Payout details
- Status

## 3. Entity Relationships

- One User can have wallet information.
- One User can have multiple transactions.
- One User can create multiple withdrawal requests.
- A withdrawal request can contain payout method details.
- Admin users can review and manage withdrawal requests.

## 4. Relationship Overview

```text
USER
 |
 |---- WALLET
 |
 |---- TRANSACTION
 |
 |---- WITHDRAWAL
          |
          |---- PAYOUT DETAILS
```

## 5. Data Integrity

The application uses user identifiers to associate wallet, transaction, and withdrawal records with their respective users.

Wallet and withdrawal operations include validation and balance-handling logic in the application.

## 6. Known Limitations

- Referral invite tracking schema is not available.
- External production database connectivity has not been verified.
- The current test environment uses embedded MongoDB Memory Server.
- The exact production data relationships require verification against the approved VELOOP database schema.

## 7. Conclusion

This report documents the major application entities and their intended relationships.

The ER overview represents the current application structure at a high level. Final production schema validation requires access to the approved production database and stakeholder confirmation.
