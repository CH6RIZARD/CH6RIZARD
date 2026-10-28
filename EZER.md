# EZER

We catch recurring charges. EZER finds every subscription, trial and monthly charge before it bills, makes cancelling easy (one guided flow, proof kept), and puts a savings module right next to your existing and cancelled subscriptions so what you cut shows up as money saved.

## Features

### Core Features (Tier 1 - Fully Implemented)

- **Pre-Trial Intercept**: Detect new trials via email/transaction parsing and prompt users to set auto-cancel rules
- **Funding-First Wallet UI**: Visual card carousel showing subscription drains by funding instrument
- **Direct Cancellation Spine**: Guided cancel flow with proof upload and confirmation tracking
- **Price-Drain Timeline**: Historical cost analysis with investment opportunity cost calculator (7% annualized)
- **Reallocation Engine**: Redirect canceled subscription amounts to savings, debt, investing, or intentional subscriptions

### Data Intake
- On-device inbox scan (Gmail API, Outlook Graph API) — raw email never leaves the device
- Transaction CSV import with recurrence detection

### OAuth & Security
- Google OAuth (Sign-in + Gmail API)
- Microsoft OAuth (Sign-in + Outlook Graph API)
- Apple Sign-In

## Tech Stack

- **Mobile**: Expo, React Native, TypeScript (plus a native SwiftUI iPhone app)
- **Backend**: Fastify, Node.js, TypeScript
- **Database**: PostgreSQL (Prisma ORM)
- **Auth**: OAuth 2.0 (Google, Microsoft, Apple)

## Mobile App Screens

1. **Onboarding**: Choose sign-in method (Google / Apple / Microsoft)
2. **Home**: Monthly burn rate, 30-day risk, silent subscriptions count
3. **Wallet**: Card carousel with drain summary by funding instrument
4. **Card Detail**: Merchants draining specific card
5. **Risks**: Trials expiring + upcoming renewals in next 30 days
6. **Trials**: Active trials list with countdown
7. **Trial Decision**: Set auto-cancel or conversion rules
8. **Subscription Detail**: Charge history, price timeline, lifetime cost, cancellation difficulty
9. **Cancel Flow**: Guided cancel with proof upload
10. **Confirm Cancel**: Proof summary + mark confirmed
11. **Reallocate**: Choose allocation target after cancellation
12. **Ledger**: Reclaimed this month + allocations

## Design Principles

- **White/near-white background UI**: Clean, minimal aesthetic
- **One primary action per screen**: Single prominent CTA
- **Numbers > charts**: Plain numbers with red (drain) / green (reclaimed) semantics
- **The app acts**: Not just informative, but actionable (cancel flows, reallocations)

## Links

- Website: https://ch6rizard.github.io/ezer/
- Privacy policy: https://ch6rizard.github.io/ezer/privacy.html

---

This repository is an overview only. EZER's source code is private.
© 2026 Chiagozie Oliver. All rights reserved.
