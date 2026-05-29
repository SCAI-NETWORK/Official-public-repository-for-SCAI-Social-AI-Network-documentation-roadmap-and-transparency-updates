# Public Architecture Overview

SCAI is designed as a private AI trading operating layer with public transparency around token access and private protection around execution logic.

## Layers

## 1. Investor Access Layer

The investor access layer connects wallet-based identity, token position, tier status, referral identity, purchase history, vesting visibility and claim readiness.

## 2. Bot Engine Layer

The initial platform contains five separated autonomous engines. Each engine has its own decision chain, risk model, configuration surface, runtime view and audit trail.

## 3. Security And Vault Layer

User connectors, wallets, signers and exchange credentials are intended to be configured per user and per bot. Sensitive values should be masked after saving and require additional verification for changes.

## 4. Worker Runtime Layer

Workers monitor data sources, streams, heartbeats, stale-data conditions, parser health and restart policies. Runtime visibility is designed to make the platform feel alive while preserving operational separation.

## 5. Audit And Export Layer

The platform is designed to keep decision trails, trade history, AI reasoning, user actions, missed opportunities, ignored candidates and exportable logs.

## Public vs Private

The public repository documents high-level architecture. It does not publish private execution workers, bot code, scoring models, credentials or deployment secrets.
