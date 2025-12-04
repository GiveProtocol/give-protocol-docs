---
title: Help & Support
description: Find answers, browse guides, and get support for Give Protocol
permalink: /docs/support/
---

<div class="support-hero">
  <h1>How can we help you?</h1>
  <p>Search for answers or browse our most popular topics</p>

  <div class="support-search-box">
    <i class="fas fa-search"></i>
    <input type="text" id="support-search" placeholder="Search for help..." autofocus>
  </div>
</div>

## Popular Articles

<div class="popular-articles-grid">
{% for article in site.data.navigation.popular_articles limit:6 %}
<a href="{{ article.url | relative_url }}" class="popular-article-card">
  <h4>{{ article.title }}</h4>
  <p>{{ article.description }}</p>
  <span class="read-arrow"><i class="fas fa-arrow-right"></i></span>
</a>
{% endfor %}
</div>

## Quick Answers

<div class="faq-accordion">
{% for faq in site.data.navigation.quick_faqs %}
<div class="faq-item">
  <button class="faq-question" aria-expanded="false">
    <span>{{ faq.question }}</span>
    <i class="fas fa-chevron-down"></i>
  </button>
  <div class="faq-answer">
    <p>{{ faq.answer }}</p>
  </div>
</div>
{% endfor %}
</div>

## Browse by Topic

<div class="topic-cards">
  <a href="{{ '/docs/getting-started/' | relative_url }}" class="topic-card">
    <i class="fas fa-rocket"></i>
    <span>Getting Started</span>
  </a>
  <a href="{{ '/docs/donors/' | relative_url }}" class="topic-card">
    <i class="fas fa-heart"></i>
    <span>For Donors</span>
  </a>
  <a href="{{ '/docs/organizations/' | relative_url }}" class="topic-card">
    <i class="fas fa-building"></i>
    <span>For Organizations</span>
  </a>
  <a href="{{ '/docs/volunteers/' | relative_url }}" class="topic-card">
    <i class="fas fa-hands-helping"></i>
    <span>For Volunteers</span>
  </a>
  <a href="{{ '/docs/technical/' | relative_url }}" class="topic-card">
    <i class="fas fa-code"></i>
    <span>Technical</span>
  </a>
  <a href="{{ '/docs/troubleshooting/' | relative_url }}" class="topic-card">
    <i class="fas fa-wrench"></i>
    <span>Troubleshooting</span>
  </a>
</div>

<div class="still-stuck">
  <div class="still-stuck-content">
    <h2>Still stuck?</h2>
    <p>Our support team is here to help with any questions you can't find answers to.</p>

    <div class="contact-options">
      <a href="mailto:support@giveprotocol.org" class="contact-option">
        <div class="contact-icon">
          <i class="fas fa-envelope"></i>
        </div>
        <div class="contact-details">
          <strong>Email Support</strong>
          <span>support@giveprotocol.org</span>
          <small>Response time: 1-2 business days</small>
        </div>
      </a>

      <a href="https://discord.gg/giveprotocol" class="contact-option" target="_blank" rel="noopener">
        <div class="contact-icon discord">
          <i class="fab fa-discord"></i>
        </div>
        <div class="contact-details">
          <strong>Discord Community</strong>
          <span>Join our Discord server</span>
          <small>Community support & discussions</small>
        </div>
      </a>
    </div>
  </div>
</div>

<style>
.support-hero {
  text-align: center;
  padding: 2rem 0 3rem;
  margin-bottom: 2rem;
}

.support-hero h1 {
  font-size: 2.25rem;
  color: #111827;
  margin-bottom: 0.5rem;
}

.support-hero p {
  color: #6b7280;
  font-size: 1.1rem;
  margin-bottom: 2rem;
}

.support-search-box {
  position: relative;
  max-width: 550px;
  margin: 0 auto;
}

.support-search-box i {
  position: absolute;
  left: 1.25rem;
  top: 50%;
  transform: translateY(-50%);
  color: #9ca3af;
  font-size: 1.1rem;
}

.support-search-box input {
  width: 100%;
  padding: 1rem 1rem 1rem 3.5rem;
  border: 2px solid #e5e7eb;
  border-radius: 12px;
  font-size: 1.1rem;
  transition: all 0.2s ease;
  background: #fff;
}

.support-search-box input:focus {
  outline: none;
  border-color: #047857;
  box-shadow: 0 0 0 4px rgba(4, 120, 87, 0.1);
}

/* Popular Articles */
.popular-articles-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
  gap: 1rem;
  margin-bottom: 3rem;
}

.popular-article-card {
  display: block;
  background: #f9fafb;
  border: 1px solid #e5e7eb;
  border-radius: 10px;
  padding: 1.25rem;
  text-decoration: none;
  transition: all 0.2s ease;
  position: relative;
}

.popular-article-card:hover {
  background: #fff;
  border-color: #047857;
  transform: translateY(-2px);
  box-shadow: 0 4px 12px rgba(4, 120, 87, 0.1);
}

.popular-article-card h4 {
  color: #111827;
  margin: 0 0 0.5rem;
  font-size: 1rem;
  padding-right: 1.5rem;
}

.popular-article-card p {
  color: #6b7280;
  margin: 0;
  font-size: 0.875rem;
  line-height: 1.4;
}

.popular-article-card .read-arrow {
  position: absolute;
  right: 1.25rem;
  top: 1.25rem;
  color: #047857;
  opacity: 0;
  transform: translateX(-4px);
  transition: all 0.2s ease;
}

.popular-article-card:hover .read-arrow {
  opacity: 1;
  transform: translateX(0);
}

/* FAQ Accordion */
.faq-accordion {
  margin-bottom: 3rem;
}

.faq-item {
  border: 1px solid #e5e7eb;
  border-radius: 10px;
  margin-bottom: 0.75rem;
  overflow: hidden;
  background: #fff;
}

.faq-question {
  width: 100%;
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 1rem 1.25rem;
  background: none;
  border: none;
  cursor: pointer;
  text-align: left;
  font-size: 1rem;
  font-weight: 500;
  color: #111827;
  transition: all 0.2s ease;
}

.faq-question:hover {
  background: #f9fafb;
}

.faq-question i {
  color: #6b7280;
  transition: transform 0.3s ease;
  flex-shrink: 0;
  margin-left: 1rem;
}

.faq-item.active .faq-question i {
  transform: rotate(180deg);
}

.faq-answer {
  max-height: 0;
  overflow: hidden;
  transition: max-height 0.3s ease;
}

.faq-item.active .faq-answer {
  max-height: 300px;
}

.faq-answer p {
  padding: 0 1.25rem 1.25rem;
  margin: 0;
  color: #4b5563;
  line-height: 1.6;
}

/* Topic Cards */
.topic-cards {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
  gap: 1rem;
  margin-bottom: 3rem;
}

.topic-card {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 0.75rem;
  padding: 1.5rem 1rem;
  background: #fff;
  border: 1px solid #e5e7eb;
  border-radius: 10px;
  text-decoration: none;
  transition: all 0.2s ease;
}

.topic-card:hover {
  border-color: #047857;
  box-shadow: 0 4px 12px rgba(4, 120, 87, 0.1);
  transform: translateY(-2px);
}

.topic-card i {
  font-size: 1.5rem;
  color: #047857;
}

.topic-card span {
  color: #374151;
  font-weight: 500;
  font-size: 0.9rem;
  text-align: center;
}

/* Still Stuck Section */
.still-stuck {
  background: #f9fafb;
  border-radius: 12px;
  padding: 2rem;
  margin-top: 2rem;
}

.still-stuck h2 {
  color: #111827;
  margin: 0 0 0.5rem;
}

.still-stuck > .still-stuck-content > p {
  color: #6b7280;
  margin: 0 0 1.5rem;
}

.contact-options {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
  gap: 1rem;
}

.contact-option {
  display: flex;
  align-items: flex-start;
  gap: 1rem;
  padding: 1.25rem;
  background: #fff;
  border: 1px solid #e5e7eb;
  border-radius: 10px;
  text-decoration: none;
  transition: all 0.2s ease;
}

.contact-option:hover {
  border-color: #047857;
  box-shadow: 0 2px 8px rgba(0, 0, 0, 0.05);
}

.contact-option .contact-icon {
  width: 48px;
  height: 48px;
  background: #047857;
  border-radius: 10px;
  display: flex;
  align-items: center;
  justify-content: center;
  flex-shrink: 0;
}

.contact-option .contact-icon.discord {
  background: #5865F2;
}

.contact-option .contact-icon i {
  color: #fff;
  font-size: 1.25rem;
}

.contact-details {
  display: flex;
  flex-direction: column;
}

.contact-details strong {
  color: #111827;
  font-size: 1rem;
  margin-bottom: 0.125rem;
}

.contact-details span {
  color: #047857;
  font-size: 0.9rem;
}

.contact-details small {
  color: #9ca3af;
  font-size: 0.8rem;
  margin-top: 0.25rem;
}

/* Dark mode */
body.dark-mode .support-hero h1 {
  color: #f3f4f6;
}

body.dark-mode .support-search-box input {
  background: #1f2937;
  border-color: #374151;
  color: #f3f4f6;
}

body.dark-mode .support-search-box input:focus {
  border-color: #10b981;
}

body.dark-mode .popular-article-card {
  background: #1f2937;
  border-color: #374151;
}

body.dark-mode .popular-article-card h4 {
  color: #f3f4f6;
}

body.dark-mode .popular-article-card p {
  color: #9ca3af;
}

body.dark-mode .faq-item {
  background: #1f2937;
  border-color: #374151;
}

body.dark-mode .faq-question {
  color: #f3f4f6;
}

body.dark-mode .faq-question:hover {
  background: #374151;
}

body.dark-mode .faq-answer p {
  color: #d1d5db;
}

body.dark-mode .topic-card {
  background: #1f2937;
  border-color: #374151;
}

body.dark-mode .topic-card span {
  color: #d1d5db;
}

body.dark-mode .topic-card i {
  color: #34d399;
}

body.dark-mode .still-stuck {
  background: #1f2937;
}

body.dark-mode .still-stuck h2 {
  color: #f3f4f6;
}

body.dark-mode .contact-option {
  background: #111827;
  border-color: #374151;
}

body.dark-mode .contact-details strong {
  color: #f3f4f6;
}

body.dark-mode .contact-details span {
  color: #34d399;
}

@media (max-width: 768px) {
  .support-hero h1 {
    font-size: 1.75rem;
  }

  .topic-cards {
    grid-template-columns: repeat(2, 1fr);
  }

  .contact-options {
    grid-template-columns: 1fr;
  }
}
</style>

<script>
// FAQ Accordion functionality
document.querySelectorAll('.faq-question').forEach(button => {
  button.addEventListener('click', () => {
    const faqItem = button.parentElement;
    const isActive = faqItem.classList.contains('active');

    // Close all other FAQs
    document.querySelectorAll('.faq-item').forEach(item => {
      item.classList.remove('active');
      item.querySelector('.faq-question').setAttribute('aria-expanded', 'false');
    });

    // Toggle current FAQ
    if (!isActive) {
      faqItem.classList.add('active');
      button.setAttribute('aria-expanded', 'true');
    }
  });
});

// Link support search to main search
document.getElementById('support-search').addEventListener('input', function() {
  const mainSearch = document.getElementById('search-input');
  if (mainSearch) {
    mainSearch.value = this.value;
    mainSearch.dispatchEvent(new Event('input'));
  }
});
</script>
