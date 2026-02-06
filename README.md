# Quackback Documentation

Welcome to the Quackback documentation. Quackback is an open-source customer feedback platform for collecting, organizing, and acting on user feedback.

## Documentation Structure

### Getting Started
- [Introduction](getting-started/introduction.mdx) - What is Quackback
- [Quick Start](getting-started/quick-start.mdx) - Deploy in 5 minutes
- [Core Concepts](getting-started/concepts.mdx) - Boards, posts, statuses, and more

### Self-Hosting
- [Requirements](self-hosting/requirements.mdx) - System requirements
- [Docker Deployment](self-hosting/docker.mdx) - Recommended deployment method
- [Manual Installation](self-hosting/manual.mdx) - Install without Docker
- [Reverse Proxy](self-hosting/reverse-proxy.mdx) - Nginx, Caddy, Traefik configuration
- [Troubleshooting](self-hosting/troubleshooting.mdx) - Common issues and solutions

### User Guide
- [Submitting Feedback](users/submitting-feedback.mdx) - How to share ideas
- [Voting](users/voting.mdx) - Supporting ideas you care about
- [Comments](users/comments.mdx) - Joining the discussion
- [Notifications](users/notifications.mdx) - Managing alerts
- [Account Settings](users/account.mdx) - Profile and preferences

### Admin Guide
- [Managing Feedback](admin/inbox.mdx) - Feedback inbox and workflow
- [Boards](admin/boards.mdx) - Organizing feedback categories
- [Statuses](admin/statuses.mdx) - Workflow stages
- [Tags](admin/tags.mdx) - Additional categorization
- [Roadmap](admin/roadmap.mdx) - Public progress tracking
- [Portal Users](admin/users.mdx) - Managing portal user accounts
- [Notifications](admin/notifications.mdx) - Admin notification settings
- [Team](admin/team.mdx) - Team member management
- [Security](admin/security.mdx) - Team authentication settings
- [Portal Authentication](admin/portal-auth.mdx) - Portal user sign-in options
- [Branding](admin/branding.mdx) - Customization
- [Import & Export](admin/import-export.mdx) - Data migration

### Authentication
- [Overview](auth/overview.mdx) - Auth methods and configuration
- [Email OTP](auth/email-otp.mdx) - Magic link authentication
- [OAuth](auth/oauth.mdx) - GitHub, Google, Microsoft setup

### Integrations
- [Overview](integrations/overview.mdx) - How integrations work
- [Slack](integrations/slack.mdx) - Slack notifications
- [Webhooks](integrations/webhooks.mdx) - Send events to any HTTP endpoint
- [Discord](integrations/discord.mdx) - Discord integration (community)
- [Linear](integrations/linear.mdx) - Linear integration (community)

### API Reference
- [Overview](api/overview.mdx) - REST API v1 documentation
- [Posts API](api/posts.mdx) - Post operations
- [Comments API](api/comments.mdx) - Comment operations

### Developer Guide
- [Development Setup](developers/setup.mdx) - Local environment
- [Architecture](developers/architecture.mdx) - System design
- [Server Functions](developers/server-functions.mdx) - RPC patterns
- [Database](developers/database.mdx) - Schema and queries
- [Adding Features](developers/adding-features.mdx) - Feature development guide
- [Testing](developers/testing.mdx) - Vitest and Playwright
- [Contributing](developers/contributing.mdx) - How to contribute

### Reference
- [Environment Variables](reference/environment-variables.mdx) - Configuration options
- [CLI Commands](reference/cli.mdx) - Command reference
- [Database Schema](reference/database-schema.mdx) - Tables and relationships

## Quick Links

| I want to... | Go to... |
|--------------|----------|
| Deploy Quackback | [Quick Start](getting-started/quick-start.mdx) |
| Understand the product | [Introduction](getting-started/introduction.mdx) |
| Configure settings | [Environment Variables](reference/environment-variables.mdx) |
| Use the REST API | [API Overview](api/overview.mdx) |
| Set up Slack | [Slack Integration](integrations/slack.mdx) |
| Set up webhooks | [Webhooks](integrations/webhooks.mdx) |
| Build a feature | [Adding Features](developers/adding-features.mdx) |
| Contribute code | [Contributing](developers/contributing.mdx) |
| Fix a problem | [Troubleshooting](self-hosting/troubleshooting.mdx) |

## Support

- [GitHub Issues](https://github.com/quackbackio/quackback/issues) - Bug reports
- [GitHub Discussions](https://github.com/quackbackio/quackback/discussions) - Questions and ideas

## License

AGPL-3.0 — See [LICENSE](https://github.com/quackbackio/quackback/blob/main/LICENSE) for details.
