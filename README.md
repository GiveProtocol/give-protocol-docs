# Give Protocol - Documentation

Comprehensive documentation for Give Protocol, including user guides, technical documentation, API references, and integration guides.

## Overview

This repository contains the official documentation site for Give Protocol, built with Jekyll and hosted on GitHub Pages.

## Documentation Structure

```
├── introduction/          # Project overview and concepts
├── getting-started/       # Quick start guides
├── user-guides/           # User documentation
│   ├── donor/            # Donor guides
│   ├── charity/          # Charity guides
│   └── volunteer/        # Volunteer guides
├── platform-features/     # Feature documentation
├── technical/             # Technical documentation
│   ├── contracts/        # Smart contract docs
│   ├── api/              # API documentation
│   └── integration/      # Integration guides
├── resources/             # Additional resources
├── safety-security/       # Security guidelines
└── help-center/          # FAQ and support
```

## Local Development

### Prerequisites

- Ruby 2.7+
- Bundler
- Jekyll

### Setup

```bash
# Install dependencies
bundle install

# Run local server
bundle exec jekyll serve

# View at http://localhost:4000
```

### Building

```bash
# Production build
JEKYLL_ENV=production bundle exec jekyll build
```

## Contributing to Documentation

### Adding New Pages

1. Create a new markdown file in the appropriate directory
2. Add front matter with layout and title
3. Write content using Markdown
4. Test locally before committing

Example front matter:
```yaml
---
layout: default
title: Your Page Title
description: Brief description
---
```

### Search Index

After adding or updating documentation:

```bash
# Regenerate search index
node generate-search.cjs
```

## Translation

Documentation is available in multiple languages:
- English (default)
- Spanish (`/es`)
- Chinese (`/zh`)

To add a new language:
1. Create language directory (e.g., `/fr`)
2. Copy English documentation structure
3. Translate content
4. Update `_config.yml` with new language

## Deployment

Documentation is automatically deployed to GitHub Pages on push to main branch.

Manual deployment:
```bash
# Build production site
JEKYLL_ENV=production bundle exec jekyll build

# Deploy _site directory to hosting
```

## Documentation Guidelines

- Use clear, concise language
- Include code examples where appropriate
- Add images/diagrams for complex concepts
- Keep technical accuracy high
- Cross-reference related pages

See `guides/documentation-guidelines.md` for detailed guidelines.

## Links

- [Live Documentation](https://docs.giveprotocol.io)
- [Main Repository](https://github.com/give-protocol)
- [Report Issues](https://github.com/give-protocol/give-protocol-docs/issues)

## License

UNLICENSED - Private Repository
