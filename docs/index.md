---
title: Documentation
description: Find guides, tutorials, and reference documentation for Give Protocol
permalink: /docs/
layout: modern
---

<div class="docs-hero-compact">
  <h1>Give Protocol Documentation</h1>
  <p class="hero-subtitle">Everything you need to donate, receive, and manage crypto philanthropy</p>
</div>

<div class="filter-pills">
  <a href="{{ '/docs/getting-started/' | relative_url }}" class="filter-pill"><i class="fas fa-rocket"></i> Getting Started</a>
  <a href="{{ '/docs/donors/' | relative_url }}" class="filter-pill"><i class="fas fa-heart"></i> Donors</a>
  <a href="{{ '/docs/organizations/' | relative_url }}" class="filter-pill"><i class="fas fa-building"></i> Organizations</a>
  <a href="{{ '/docs/volunteers/' | relative_url }}" class="filter-pill"><i class="fas fa-hands-helping"></i> Volunteers</a>
  <a href="{{ '/docs/technical/' | relative_url }}" class="filter-pill"><i class="fas fa-code"></i> Technical</a>
</div>

<div class="journey-cards">
  <a href="{{ '/docs/donors/' | relative_url }}" class="journey-card">
    <div class="journey-icon"><i class="fas fa-heart"></i></div>
    <span class="journey-title">I want to donate</span>
    <span class="journey-desc">Connect your wallet and make tax-advantaged crypto donations</span>
  </a>
  <a href="{{ '/docs/organizations/' | relative_url }}" class="journey-card">
    <div class="journey-icon"><i class="fas fa-building"></i></div>
    <span class="journey-title">I'm a nonprofit</span>
    <span class="journey-desc">Get verified and start receiving cryptocurrency donations</span>
  </a>
  <a href="{{ '/docs/volunteers/' | relative_url }}" class="journey-card">
    <div class="journey-icon"><i class="fas fa-hands-helping"></i></div>
    <span class="journey-title">I want to volunteer</span>
    <span class="journey-desc">Find opportunities and track your volunteer hours</span>
  </a>
  <a href="{{ '/docs/technical/' | relative_url }}" class="journey-card">
    <div class="journey-icon"><i class="fas fa-code"></i></div>
    <span class="journey-title">I'm a developer</span>
    <span class="journey-desc">Explore smart contracts, APIs, and technical architecture</span>
  </a>
</div>

<div class="popular-articles-section">
  <div class="section-header">
    <h2>Popular Articles</h2>
  </div>
  <div class="popular-articles-grid">
    {% for article in site.data.popular_articles limit:6 %}
    <a href="{{ article.url | relative_url }}" class="popular-article-card">
      <span class="article-category">{{ article.category }}</span>
      <span class="article-title">{{ article.title }}</span>
      <span class="article-desc">{{ article.description }}</span>
      <span class="article-meta"><i class="fas fa-clock"></i> {{ article.read_time }} min read</span>
    </a>
    {% endfor %}
  </div>
</div>

<div class="quickstart-section">
  <h2><i class="fas fa-list-check"></i> Quick Start Checklist</h2>
  <ul class="checklist">
    <li class="checklist-item">
      <span class="check-circle"></span>
      <div class="check-content">
        <span class="check-title"><a href="{{ '/docs/getting-started/wallet-connection/' | relative_url }}">Connect your wallet</a></span>
        <span class="check-desc">Link MetaMask, WalletConnect, or another Web3 wallet</span>
      </div>
    </li>
    <li class="checklist-item">
      <span class="check-circle"></span>
      <div class="check-content">
        <span class="check-title"><a href="{{ '/docs/getting-started/' | relative_url }}">Create your account</a></span>
        <span class="check-desc">Set up your Give Protocol profile in minutes</span>
      </div>
    </li>
    <li class="checklist-item">
      <span class="check-circle"></span>
      <div class="check-content">
        <span class="check-title"><a href="{{ '/docs/donors/making-donations/' | relative_url }}">Make your first donation</a></span>
        <span class="check-desc">Donate crypto to verified charitable organizations</span>
      </div>
    </li>
    <li class="checklist-item">
      <span class="check-circle"></span>
      <div class="check-content">
        <span class="check-title"><a href="{{ '/docs/donors/tax-documentation/' | relative_url }}">Download tax receipt</a></span>
        <span class="check-desc">Get IRS-compliant documentation for your contribution</span>
      </div>
    </li>
  </ul>
</div>

<div class="recently-updated-section">
  <h2><i class="fas fa-clock-rotate-left"></i> Recently Updated</h2>
  <div class="updated-list">
    <a href="{{ '/docs/technical/supported-tokens/' | relative_url }}" class="updated-item">
      <span class="updated-title">Supported Cryptocurrencies</span>
      <span class="updated-date">Updated Dec 2024</span>
    </a>
    <a href="{{ '/docs/donors/understanding-cefs/' | relative_url }}" class="updated-item">
      <span class="updated-title">Understanding CEFs</span>
      <span class="updated-date">Updated Nov 2024</span>
    </a>
    <a href="{{ '/docs/organizations/verification/' | relative_url }}" class="updated-item">
      <span class="updated-title">Organization Verification</span>
      <span class="updated-date">Updated Nov 2024</span>
    </a>
  </div>
</div>

<div class="docs-support-cta">
  <div class="support-cta-content">
    <h2>Need help?</h2>
    <p>Can't find what you're looking for? Our support team is here to assist.</p>
    <a href="{{ '/docs/support/' | relative_url }}" class="btn-support">
      <i class="fas fa-headset"></i>
      Contact Support
    </a>
  </div>
</div>

<style>
/* Support CTA - kept from original */
.docs-support-cta {
  background: linear-gradient(135deg, #047857, #059669);
  border-radius: 12px;
  padding: 2rem;
  text-align: center;
  color: #fff;
  margin-top: 1rem;
}

.docs-support-cta h2 {
  color: #fff;
  margin: 0 0 0.5rem 0;
  font-size: 1.25rem;
}

.docs-support-cta p {
  color: rgba(255,255,255,0.9);
  margin: 0 0 1.25rem 0;
  font-size: 0.9375rem;
}

.btn-support {
  display: inline-flex;
  align-items: center;
  gap: 0.5rem;
  background: #fff;
  color: #047857;
  padding: 0.75rem 1.5rem;
  border-radius: 8px;
  text-decoration: none;
  font-weight: 600;
  font-size: 0.9375rem;
  transition: all 0.2s ease;
}

.btn-support:hover {
  background: #f0fdf4;
  transform: translateY(-1px);
}

.btn-support i {
  font-style: normal !important;
}
</style>
