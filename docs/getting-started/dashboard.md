---
title: Dashboard
description: How to navigate the Give Protocol dashboard — your central hub for donations, credentials, settings, and organization management.
permalink: /docs/getting-started/dashboard/
---

# Dashboard

The Give Protocol dashboard is your central hub. It's a single page at `/dashboard` that adapts based on your role (Donor or Charity) and your connected state (wallet linked or not). Everything you need — donation history, settings, wallet management, and organization tools — lives here.

## Accessing Your Dashboard

After signing in (via email, wallet, or both), you're taken directly to your dashboard. You can return to it at any time by clicking **Dashboard** in the navigation bar.

## Donor Dashboard

If you're logged in as a donor, your dashboard includes:

### Donation History

A unified view of all your contributions — both crypto and fiat — in one table. Each entry shows:

- **Type** — Crypto (with chain icon and token) or Fiat (with currency badge)
- **Amount** — The donation amount in the original currency
- **Charity** — The recipient organization
- **Date** — When the donation was made
- **Status** — Confirmed, pending, or escrowed
- **Verification** — For crypto donations, a link to the transaction on the relevant block explorer. For fiat donations, a Helcim or PayPal reference.

If you linked a wallet after making earlier donations with it, those historical on-chain transactions will appear in your history automatically — the system looks up contributions by both your user ID and your linked wallet address.

### CEF Portfolio (Coming Soon)

Once Charitable Equity Funds are live, this section will show:

- CEF vaults you've contributed to
- Current principal balance and yield performance
- Distribution history to the beneficiary charity
- Your share of the fund

### SBT Credentials (Coming Soon)

A display of any Soul-Bound Tokens you've earned, including:

- Donor reputation credentials (automatically issued based on your giving history)
- Volunteer credentials (issued by verified charities)
- Impact achievement badges (tied to specific campaigns or milestones)

### Tax Receipts

Access and download receipts for any donation you've made. Receipts include the Foundation's details, the receiving charity's name, your donation amount, and a GP-prefixed reference number.

### Settings

- **Account** — Update your display name, email, and notification preferences.
- **Wallet** — Link or unlink a crypto wallet. View your linked address and the date it was connected.

## Charity Dashboard

If you're logged in as a charity representative and your organization's profile is verified, your dashboard provides management tools for your organization.

### Post-Claim Onboarding Checklist

If you've recently claimed your organization's profile, the dashboard will prominently display your onboarding checklist:

- ✅ Identity verified
- ⬜ Add receiving wallet — Connect your organization's crypto wallet to receive crypto donations
- ⬜ Connect bank account — Set up Helcim to receive fiat (USD) donations
- ⬜ Complete profile — Add your mission statement, logo, and program details

Complete these steps to unlock full functionality and release any escrowed donations from before your profile was claimed.

### Incoming Donations

A view of all donations received by your organization, combining crypto and fiat:

- Individual transaction details with donor information (where provided)
- Running totals by time period
- On-chain verification links for crypto donations

### CEF Vault Management (Coming Soon)

Once CEF vaults are deployed, this section will let you:

- View your vault's current balance and yield performance
- See the distribution schedule and history
- Optionally reinvest a portion of yield to grow the fund
- Review which protocols your assets are deployed in

### Portfolio Fund Status (Coming Soon)

If your organization participates in a Portfolio/Cause Fund, this section shows:

- Which fund(s) you're included in
- Distribution history and upcoming scheduled distributions
- Your share of the fund

### Volunteer Opportunity Management (Coming Soon)

Tools for managing volunteer credentials:

- Post volunteer opportunities
- Issue Soul-Bound Token credentials to verified volunteers
- Track issued credentials and volunteer activity

### Fiat Disbursement Pipeline

A view of the status of fiat donations being processed for disbursement to your organization. Statuses include Pending, Processing, and Disbursed. During the early phase of the platform, fiat disbursements are processed manually in batches (ACH or wire transfer) and status updates are managed by the Give Protocol team.

## Wallet Connection Prompt

If you're signed in via email and attempt a blockchain-specific action (like making a crypto donation or viewing SBT credentials), a modal will appear prompting you to connect a wallet. This is a contextual prompt — it appears only when needed, not as a barrier to accessing the platform.

You can dismiss it and continue using fiat features, or connect your wallet to proceed with the blockchain action.

## Tips for Using the Dashboard

- **Bookmark it.** The dashboard is at `giveprotocol.io/dashboard` — you can go straight there after signing in.
- **Check both views.** If you have both donor and charity roles, the dashboard adapts to show relevant sections for each.
- **Donation history is retroactive.** If you link a wallet that was used for donations before your account existed, those transactions will appear in your history.
- **Settings are always accessible.** Account, wallet, and notification settings are available from the dashboard sidebar or settings page regardless of your role.
