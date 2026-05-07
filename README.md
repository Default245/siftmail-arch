# SiftMail Architecture

**SiftMail** is an AI-powered inbox shield and triage layer designed to sit between your email inbox and everything trying to reach you.

This public repository is a sanitized product and architecture showcase. The commercial codebase remains private.

## Problem

Email inboxes are noisy, unsafe, and increasingly difficult to trust. Important messages get buried beside spam, abuse, phishing, promotional noise, transactional clutter, and low-value notifications.

## Core product areas

### Inbox Shield
Blocks or flags suspicious, abusive, manipulative, or low-trust email patterns.

### AI Triage
Classifies messages into useful categories such as VIP, critical, transactional, promotional, normal, spam, suspicious, and abusive.

### Exposure Index
Shows where attention, risk, and inbox clutter are coming from.

### Smart Actions
Recommends actions such as archive, quarantine, label, snooze, allowlist, denylist, or escalate.

## Architecture overview

```text
Email Provider
  -> OAuth + Sync Layer
  -> Message Normalization
  -> AI Classification + Rules Engine
  -> Risk / Priority / Intent Scoring
  -> Actions: Label, Quarantine, Archive, Alert, Allow, Block
  -> Dashboard + Reports + User Feedback
```

## Security posture

- OAuth-based provider access
- Backend-controlled privileged actions
- Stripe-gated plan logic
- Proxy allowlists
- Token encryption
- Privacy-aware audit logging
- Protected main branch and PR-based development

## Why this repo exists

This repository demonstrates product depth, architecture, security thinking, and execution quality without exposing the private commercial codebase.
