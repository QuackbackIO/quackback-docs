# Quackback Documentation

Collect, organize, and act on user feedback. Open source, self-hosted.

## Quick Links

| I want to... | Go to... |
|--------------|----------|
| Get Quackback running | [Quick Start](getting-started/quick-start.mdx) |
| Understand the core ideas | [Core Concepts](getting-started/concepts.mdx) |
| Organize feedback by category | [Organize feedback with boards](admin/boards.mdx) |
| Track feedback from idea to shipped | [Track progress with statuses](admin/statuses.mdx) |
| Show users what I'm building | [Build a public roadmap](admin/roadmap.mdx) |
| Connect to Slack | [Set up Slack notifications](integrations/slack.mdx) |
| Send events to my server | [Send events with webhooks](integrations/webhooks.mdx) |
| Build a custom integration | [API Overview](api/overview.mdx) |
| Deploy to production | [Deploy with Docker](self-hosting/docker.mdx) |
| Configure settings | [Environment Variables](reference/environment-variables.mdx) |
| Fix a problem | [Troubleshooting](self-hosting/troubleshooting.mdx) |
| Contribute code | [Contribute to Quackback](developers/contributing.mdx) |

## Getting Started

- [Introduction](getting-started/introduction.mdx) — What is Quackback
- [Quick Start](getting-started/quick-start.mdx) — Get running in 5 minutes
- [Core Concepts](getting-started/concepts.mdx) — Boards, posts, statuses, and roles

## For Users

- [Submit feedback](users/submitting-feedback.mdx) — Share ideas and report bugs
- [Vote on feedback](users/voting.mdx) — Support ideas you care about
- [Comment on posts](users/comments.mdx) — Join the discussion
- [Manage your notifications](users/notifications.mdx) — Control your alerts
- [Manage your account](users/account.mdx) — Profile and preferences

## For Admins

- [Triage feedback in the inbox](admin/inbox.mdx) — Filter, triage, and respond
- [Organize feedback with boards](admin/boards.mdx) — Categorize by type
- [Track progress with statuses](admin/statuses.mdx) — Define workflow stages
- [Categorize posts with tags](admin/tags.mdx) — Label and filter
- [Build a public roadmap](admin/roadmap.mdx) — Show what you're building
- [Manage portal users](admin/users.mdx) — See who's giving feedback
- [Configure admin notifications](admin/notifications.mdx) — Team alert settings
- [Manage your team](admin/team.mdx) — Invite teammates and assign roles
- [Configure team security](admin/security.mdx) — Team sign-in methods
- [Set up portal sign-in](admin/portal-auth.mdx) — User authentication options
- [Customize your portal](admin/branding.mdx) — Logo, colors, and fonts
- [Import and export data](admin/import-export.mdx) — Migrate from other tools

## Authentication

- [Authentication](auth/overview.mdx) — Overview of auth methods
- [Set up email sign-in](auth/email-otp.mdx) — Passwordless email codes
- [Set up OAuth providers](auth/oauth.mdx) — GitHub, Google, Microsoft
- [Set up single sign-on](auth/sso.mdx) — OIDC SSO

## Integrations

- [Integrations](integrations/overview.mdx) — How integrations work
- [Set up Slack notifications](integrations/slack.mdx) — Feedback alerts in Slack
- [Send events with webhooks](integrations/webhooks.mdx) — HTTP event notifications
- [Set up Discord notifications](integrations/discord.mdx) — Community contribution
- [Sync feedback with Linear](integrations/linear.mdx) — Community contribution

## API Reference

- [API Overview](api/overview.mdx) — REST API v1 documentation
- [Posts API](api/posts.mdx) — Post operations
- [Comments API](api/comments.mdx) — Comment operations

## Self-Hosting

- [System Requirements](self-hosting/requirements.mdx) — Hardware and software
- [Deploy with Docker](self-hosting/docker.mdx) — Recommended deployment
- [Install without Docker](self-hosting/manual.mdx) — Manual installation
- [Set up a reverse proxy](self-hosting/reverse-proxy.mdx) — Nginx, Caddy, Traefik
- [Troubleshooting](self-hosting/troubleshooting.mdx) — Common issues

## Developer Guide

- [Set up local development](developers/setup.mdx) — Local environment
- [Architecture](developers/architecture.mdx) — System design
- [Server Functions](developers/server-functions.mdx) — RPC patterns
- [Database](developers/database.mdx) — Schema and queries
- [Add a new feature](developers/adding-features.mdx) — Feature development
- [Testing](developers/testing.mdx) — Vitest and Playwright
- [Contribute to Quackback](developers/contributing.mdx) — How to contribute

## Reference

- [Environment Variables](reference/environment-variables.mdx) — Configuration options
- [CLI Reference](reference/cli.mdx) — Command reference
- [Database Schema](reference/database-schema.mdx) — Tables and relationships

## Support

- [GitHub Issues](https://github.com/quackbackio/quackback/issues) — Bug reports
- [GitHub Discussions](https://github.com/quackbackio/quackback/discussions) — Questions and ideas

## License

AGPL-3.0 — See [LICENSE](https://github.com/quackbackio/quackback/blob/main/LICENSE) for details.
