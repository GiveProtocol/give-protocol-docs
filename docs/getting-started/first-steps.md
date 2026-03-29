---
title: First Steps
description: What to do after creating your Give Protocol account — browsing charities, making your first donation, and exploring the platform.
permalink: /docs/getting-started/first-steps/
---

# First Steps

You've created your account. Here's what to do next.

## Browse Charities

Give Protocol features thousands of verified charitable organizations sourced from official national charity registers. You can browse and search for charities by name, registration number, location, or cause category.

Each charity has a profile page showing:

- Organization name, location, and registration details
- Mission statement and cause category
- Verification status (Unclaimed, Verification Pending, or Verified)
- A donate widget for making contributions

**Verified charities** have completed the claim and identity verification process. They can receive donations directly (crypto and fiat), operate CEF vaults, and manage volunteer credentials.

**Unclaimed charities** have profiles auto-populated from official register data but haven't yet claimed their profile on Give Protocol. You can still donate to unclaimed charities — your contribution will be held in escrow until the organization claims its profile and connects a payment method. You can cancel an escrowed donation at any time before it's released.

If a charity you care about hasn't been claimed yet, you can **nominate** them — this sends an invitation to the organization's public contact email encouraging them to join. The nomination count is visible on the profile, creating social proof for other donors and the organization.

## Make Your First Donation

### Donating by Card (Fiat)

1. Navigate to the charity's profile page.
2. In the donate widget (right sidebar on desktop), enter your donation amount.
3. Select your payment method — card payment is processed through Helcim (USD) or PayPal (international currencies).
4. Complete the payment in the secure hosted payment form.
5. You'll receive a receipt with the charity's name, your donation amount, and a reference number prefixed with "GP-."

No wallet or crypto knowledge is required. Give Protocol charges a 0.5% platform fee on direct fiat donations, plus the payment processor's standard fee (charged by Helcim or PayPal, not by Give Protocol).

### Donating with Crypto

1. Make sure your wallet is connected and set to the network you want to donate on (Moonbeam, Base, or Optimism).
2. Navigate to the charity's profile page.
3. In the donate widget, select the token you'd like to donate. The widget shows only tokens available on your connected network.
4. Enter the amount. A gas fee estimate will appear before you confirm.
5. Click **Donate** and confirm the transaction in your wallet.
6. The smart contract routes your donation directly to the charity's wallet. A `DonationProcessed` event is recorded on-chain — you can verify the transaction on a block explorer.

Give Protocol charges a 0.5% platform fee on direct crypto donations, deducted automatically by the smart contract. You also pay the blockchain network's gas fee.

### Supported Tokens

The tokens available depend on which network your wallet is connected to:

| Network | Available Tokens |
|---------|-----------------|
| Moonbeam | GLMR, xcDOT, xcUSDC, xcUSDT, WGLMR |
| Base | ETH, USDC, USDT, DAI |
| Optimism | ETH, USDC.e, DAI, OP |

## Explore Charitable Equity Funds (CEFs)

CEFs are endowment-style vaults that generate sustainable yield for charities. Instead of a one-time donation that gets spent, a CEF contribution is deployed into conservative yield-generating protocols, and the returns flow to the charity on an ongoing basis.

Once CEF vaults are live for a charity, you'll see the option to contribute to their fund directly from the charity's profile page. The yield (minus a 5% protocol fee that funds Give Protocol's operations) is distributed to the charity on a regular schedule. The principal is never touched.

CEFs are currently in development and will be available on the platform after mainnet launch and security audits.

## Explore Portfolio / Cause Funds

Portfolio Funds let you support an entire field of charitable work — like environmental conservation, education, or poverty relief — with a single contribution. Your donation is distributed equally among the verified charities participating in that fund.

Three initial funds are planned. The participating charities are curated by the Foundation based on verification and mission alignment, with final composition determined through community governance.

Portfolio Funds are coming soon as a post-launch feature.

## Volunteer Opportunities

Give Protocol is building a system for verifiable volunteer credentials using Soul-Bound Tokens (SBTs). Verified charities will be able to post volunteer opportunities and issue non-transferable credential tokens to volunteers who complete them — attesting to hours served, skills demonstrated, and impact achieved.

These credentials are recorded on the blockchain and can be exported as W3C Verifiable Credentials for use on resumes, LinkedIn, or other platforms.

The volunteer credential system is currently in development.

## Track Your Impact

Your [Dashboard](/docs/getting-started/dashboard/) provides a unified view of everything you've done on Give Protocol:

- **Donation history** — All your crypto and fiat donations in one place, with transaction details, timestamps, and verification links.
- **CEF portfolio** — Track the performance of any Charitable Equity Funds you've contributed to.
- **Credentials** — View any Soul-Bound Tokens you've earned for donations or volunteer work.
- **Receipts** — Access and download donation receipts for your records.

## Next Steps

- **Complete your profile** — Add a display name and notification preferences from Settings.
- **Link a wallet** (if you haven't) — Unlock crypto donations and on-chain credentials from Settings → Wallet.
- **Nominate a charity** — If an organization you support isn't on the platform yet, nominate them from their unclaimed profile.
- **Tell others** — Give Protocol grows through word of mouth. Share a charity's profile link or your experience with friends and colleagues.
