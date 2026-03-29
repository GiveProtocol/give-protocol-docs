---
title: Setting Up Your Profile
description: How to complete your donor or charity profile on Give Protocol, including wallet linking, payment setup, and profile customization.
permalink: /docs/getting-started/setting-up-profile/
---

# Setting Up Your Profile

After creating your account, the next step is completing your profile. What this looks like depends on whether you're a donor or a charity representative.

## Donor Profile Setup

Your donor profile is straightforward. Most of it is optional, and you can update it anytime from your dashboard settings.

### Basic Information

From your dashboard, navigate to **Settings** to update:

- **Display name** — How you appear on the platform. You can use your real name or remain pseudonymous.
- **Email** — Your primary contact email (set during account creation).
- **Notification preferences** — Choose what updates you'd like to receive.

### Linking a Wallet (Optional)

If you signed up with email and want to add crypto donation capability:

1. Go to **Settings → Wallet**.
2. Click **Link a Wallet**.
3. Your browser wallet (MetaMask, Coinbase Wallet, etc.) will prompt you to sign a message. This is free — it's not a transaction.
4. Once signed, your wallet address is linked to your account.

Linking a wallet lets you make crypto donations, view your on-chain donation history, and earn blockchain-verified credentials (SBTs). You can unlink a wallet later if needed.

If you signed up with a wallet and want to add email/password for recovery, you can do that from the same settings page.

### Tax Receipts

Give Protocol generates donation receipts that include the Foundation's details and your donation amount. You can access these from your donation history in the dashboard.

**Important:** Give Protocol Foundation's 501(c)(3) status is currently pending IRS review. Until the determination letter is received, receipts will include conditional deductibility language. This does not affect the donation itself — only the tax treatment.

## Charity Profile Setup

Setting up a charity profile involves more steps, since the platform needs to verify your organization's identity before unlocking full features.

### Understanding Profile States

Every charity on Give Protocol exists in one of three states:

- **Unclaimed** — The profile was auto-populated from official national charity register data. It shows public information (name, registration number, classification, location) but is not yet managed by the organization. Donations to unclaimed profiles are held in escrow.
- **Claimed-Pending** — The organization has submitted a claim and verification is in progress. Escrowed donations continue to be held until verification completes.
- **Verified** — The organization's identity is confirmed. Full features are unlocked, including direct donations, CEF vaults, and volunteer credential management.

### The Claim Process

If your organization already has an unclaimed profile on Give Protocol (populated from your country's official charity register), claiming it is a two-step process:

**Step 1 — Verify Identity**
- Confirm your organization's registration number (e.g., EIN for US entities).
- Provide your name, title, and official email address as an authorized representative.
- The platform checks your email domain against the organization's publicly listed website as a guardrail.
- A verification link is sent to your email (valid for 24 hours).

**Step 2 — Confirm Profile**
- Review the register-sourced information on your profile.
- Edit your mission statement to better represent your organization.
- Upload your logo.
- Confirm and submit.

Wallet setup is intentionally not part of the claim flow. Identity verification and payment method configuration are separate tasks.

### Post-Claim Onboarding Checklist

After your claim is verified, your charity dashboard will show an onboarding checklist:

- ✅ **Identity verified** — Completed during the claim process.
- ⬜ **Add receiving wallet** — Connect an organizational crypto wallet to receive crypto donations. This should be your organization's dedicated wallet, not a personal wallet.
- ⬜ **Connect bank account via Helcim** — Required to receive fiat (USD) donations via direct bank transfer.
- ⬜ **Complete profile** — Add additional details, photos, and program descriptions to help donors understand your work.

Escrowed donations (from donors who gave while your profile was unclaimed) are released once you connect at least one payment method.

### Important: Wallet Separation

Give Protocol enforces a strict separation between personal wallets and organizational wallets. When you're logged into a charity account:

- The wallet-link toggle from the donor signup flow does not appear.
- If you have a personal wallet connected in your browser, the navbar will show it labeled as "Personal wallet — not linked to org accounts."
- Your organization's receiving wallet is configured separately through the charity dashboard.

This separation protects both the organization's governance structure and the individual's personal privacy.

### Customizing Your Charity Profile

Once verified, you can enhance your profile with:

- **Mission statement** — Editable text that appears on your public profile page.
- **Logo** — Uploaded via the charity dashboard; stored in the platform's asset system.
- **Website and social links** — Help donors learn more about your work.
- **Cause categories** — Tags that help donors discover your organization through search and browsing.

The core data from the official charity register (name, registration number, classification, location, tax status) remains visible and cannot be edited — this ensures donors can always see the verified source information.
