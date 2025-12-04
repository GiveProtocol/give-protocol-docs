---
title: Documentation
description: Find guides, tutorials, and reference documentation for Give Protocol
permalink: /docs/
layout: modern
---

<div class="docs-hero">
  <h1>How can we help you?</h1>
  <p>Search our documentation or browse by category below</p>

  <div class="docs-search-box">
    <i class="fas fa-search"></i>
    <input type="text" id="docs-search" placeholder="Search documentation..." autofocus>
  </div>
</div>

<div class="docs-categories">
  <div class="category-grid">
    <a href="{{ '/docs/getting-started/' | relative_url }}" class="category-card">
      <div class="category-icon">
        <i class="fas fa-rocket"></i>
      </div>
      <h3>Getting Started</h3>
      <p>New to Give Protocol? Learn the basics of creating an account, connecting your wallet, and making your first donation.</p>
    </a>

    <a href="{{ '/docs/donors/' | relative_url }}" class="category-card">
      <div class="category-icon">
        <i class="fas fa-heart"></i>
      </div>
      <h3>For Donors</h3>
      <p>Make donations, understand tax benefits through CEFs, and track the impact of your charitable giving.</p>
    </a>

    <a href="{{ '/docs/organizations/' | relative_url }}" class="category-card">
      <div class="category-icon">
        <i class="fas fa-building"></i>
      </div>
      <h3>For Organizations</h3>
      <p>Get verified, receive cryptocurrency donations, manage reporting, and withdraw funds to your organization.</p>
    </a>

    <a href="{{ '/docs/volunteers/' | relative_url }}" class="category-card">
      <div class="category-icon">
        <i class="fas fa-hands-helping"></i>
      </div>
      <h3>For Volunteers</h3>
      <p>Find opportunities, track your volunteer hours, earn credentials, and stay safe while giving your time.</p>
    </a>

    <a href="{{ '/docs/technical/' | relative_url }}" class="category-card">
      <div class="category-icon">
        <i class="fas fa-code"></i>
      </div>
      <h3>Technical Reference</h3>
      <p>Smart contracts, API documentation, security architecture, and supported blockchain tokens.</p>
    </a>

    <a href="{{ '/docs/troubleshooting/' | relative_url }}" class="category-card">
      <div class="category-icon">
        <i class="fas fa-wrench"></i>
      </div>
      <h3>Troubleshooting</h3>
      <p>Solutions for common issues with accounts, wallets, transactions, and platform errors.</p>
    </a>
  </div>
</div>

<div class="docs-popular">
  <h2>Popular Articles</h2>
  <div class="popular-grid">
    {% for article in site.data.navigation.popular_articles limit:6 %}
    <a href="{{ article.url | relative_url }}" class="popular-article">
      <h4>{{ article.title }}</h4>
      <p>{{ article.description }}</p>
      <span class="read-more">Read more <i class="fas fa-arrow-right"></i></span>
    </a>
    {% endfor %}
  </div>
</div>

<div class="docs-support-cta">
  <div class="support-cta-content">
    <h2>Still need help?</h2>
    <p>Our support team is here to assist you</p>
    <a href="{{ '/docs/support/' | relative_url }}" class="btn-support">
      <i class="fas fa-headset"></i>
      Contact Support
    </a>
  </div>
</div>

<style>
.docs-hero {
  text-align: center;
  padding: 3rem 0;
  margin-bottom: 2rem;
}

.docs-hero h1 {
  font-size: 2.5rem;
  color: #111827;
  margin-bottom: 0.5rem;
}

.docs-hero p {
  color: #6b7280;
  font-size: 1.1rem;
  margin-bottom: 2rem;
}

.docs-search-box {
  position: relative;
  max-width: 600px;
  margin: 0 auto;
}

.docs-search-box i {
  position: absolute;
  left: 1.25rem;
  top: 50%;
  transform: translateY(-50%);
  color: #9ca3af;
  font-size: 1.1rem;
}

.docs-search-box input {
  width: 100%;
  padding: 1rem 1rem 1rem 3.5rem;
  border: 2px solid #e5e7eb;
  border-radius: 12px;
  font-size: 1.1rem;
  transition: all 0.2s ease;
}

.docs-search-box input:focus {
  outline: none;
  border-color: #047857;
  box-shadow: 0 0 0 4px rgba(4, 120, 87, 0.1);
}

.category-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 1.5rem;
  margin-bottom: 3rem;
}

.category-card {
  background: #fff;
  border: 1px solid #e5e7eb;
  border-radius: 12px;
  padding: 1.5rem;
  text-decoration: none;
  transition: all 0.2s ease;
}

.category-card:hover {
  border-color: #047857;
  box-shadow: 0 4px 12px rgba(4, 120, 87, 0.1);
  transform: translateY(-2px);
}

.category-icon {
  width: 48px;
  height: 48px;
  background: linear-gradient(135deg, #047857, #059669);
  border-radius: 10px;
  display: flex;
  align-items: center;
  justify-content: center;
  margin-bottom: 1rem;
}

.category-icon i {
  color: #fff;
  font-size: 1.25rem;
}

.category-card h3 {
  color: #111827;
  margin-bottom: 0.5rem;
  font-size: 1.25rem;
}

.category-card p {
  color: #6b7280;
  font-size: 0.95rem;
  line-height: 1.5;
  margin: 0;
}

.docs-popular {
  margin-bottom: 3rem;
}

.docs-popular h2 {
  margin-bottom: 1.5rem;
  color: #111827;
}

.popular-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
  gap: 1rem;
}

.popular-article {
  background: #f9fafb;
  border: 1px solid #e5e7eb;
  border-radius: 8px;
  padding: 1.25rem;
  text-decoration: none;
  transition: all 0.2s ease;
}

.popular-article:hover {
  background: #fff;
  border-color: #047857;
}

.popular-article h4 {
  color: #111827;
  margin: 0 0 0.5rem 0;
  font-size: 1rem;
}

.popular-article p {
  color: #6b7280;
  font-size: 0.875rem;
  margin: 0 0 0.75rem 0;
  line-height: 1.4;
}

.popular-article .read-more {
  color: #047857;
  font-size: 0.875rem;
  font-weight: 500;
}

.popular-article .read-more i {
  margin-left: 0.25rem;
  transition: transform 0.2s ease;
}

.popular-article:hover .read-more i {
  transform: translateX(4px);
}

.docs-support-cta {
  background: linear-gradient(135deg, #047857, #059669);
  border-radius: 12px;
  padding: 2.5rem;
  text-align: center;
  color: #fff;
}

.docs-support-cta h2 {
  color: #fff;
  margin: 0 0 0.5rem 0;
}

.docs-support-cta p {
  color: rgba(255,255,255,0.9);
  margin: 0 0 1.5rem 0;
}

.btn-support {
  display: inline-flex;
  align-items: center;
  gap: 0.5rem;
  background: #fff;
  color: #047857;
  padding: 0.875rem 1.75rem;
  border-radius: 8px;
  text-decoration: none;
  font-weight: 600;
  transition: all 0.2s ease;
}

.btn-support:hover {
  background: #f0fdf4;
  transform: translateY(-1px);
}

/* Dark mode */
body.dark-mode .docs-hero h1 {
  color: #f3f4f6;
}

body.dark-mode .docs-search-box input {
  background: #1f2937;
  border-color: #374151;
  color: #f3f4f6;
}

body.dark-mode .docs-search-box input:focus {
  border-color: #10b981;
}

body.dark-mode .category-card {
  background: #1f2937;
  border-color: #374151;
}

body.dark-mode .category-card h3 {
  color: #f3f4f6;
}

body.dark-mode .category-card p {
  color: #9ca3af;
}

body.dark-mode .docs-popular h2 {
  color: #f3f4f6;
}

body.dark-mode .popular-article {
  background: #1f2937;
  border-color: #374151;
}

body.dark-mode .popular-article h4 {
  color: #f3f4f6;
}

body.dark-mode .popular-article p {
  color: #9ca3af;
}

@media (max-width: 768px) {
  .docs-hero h1 {
    font-size: 1.75rem;
  }

  .category-grid {
    grid-template-columns: 1fr;
  }
}
</style>

<script>
// Link docs search to main search
document.getElementById('docs-search').addEventListener('input', function() {
  const mainSearch = document.getElementById('search-input');
  if (mainSearch) {
    mainSearch.value = this.value;
    mainSearch.dispatchEvent(new Event('input'));
  }
});
</script>
