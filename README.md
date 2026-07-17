# Quackback Documentation

Collect feedback, support customers, and close the loop. Open source, self-hosted.

## Quick Links

| I want to... | Go to... |
|--------------|----------|
| Get Quackback running | [Quick Start](getting-started/quick-start.mdx) |
| Understand the core ideas | [Core Concepts](getting-started/concepts.mdx) |
| Organize feedback by category | [Organize feedback with boards](admin/boards.mdx) |
| Answer customers in one inbox | [Work the support inbox](support/inbox.mdx) |
| Turn emails into conversations | [Set up the email channel](support/channels.mdx) |
| Let AI answer support questions | [Configure the Quinn Agent](automation/quinn-agent.mdx) |
| Automate conversations and tickets | [Build a workflow](automation/workflows.mdx) |
| Publish a status page | [Set up a status page](support/status-pages.mdx) |
| Show users what I'm building | [Build a public roadmap](admin/roadmap.mdx) |
| Connect to Slack | [Set up Slack notifications](integrations/slack.mdx) |
| Send events to my server | [Send events with webhooks](integrations/webhooks.mdx) |
| Build a custom integration | [API Overview](api/overview.mdx) |
| Deploy to production | [Deploy with Docker](self-hosting/docker.mdx) |
| Scale beyond one container | [Scale with multiple replicas](self-hosting/scaling.mdx) |
| Configure settings | [Environment Variables](reference/environment-variables.mdx) |
| Fix a problem | [Troubleshooting](self-hosting/troubleshooting.mdx) |
| Contribute code | [Contribute to Quackback](developers/contributing.mdx) |

## Getting Started

- [Introduction](getting-started/introduction.mdx): What is Quackback
- [Quick Start](getting-started/quick-start.mdx): Get running in 5 minutes
- [Core Concepts](getting-started/concepts.mdx): Boards, posts, statuses, and roles

## Cloud

- [Quackback Cloud](cloud/index.mdx): Managed hosting vs self-hosting
- [AI operations](cloud/ai-operations.mdx): AI features on Cloud plans
- [Upgrades and downgrades](cloud/upgrade-downgrade.mdx): What happens at tier limits

## Guides

A structured course for building a feedback program that ships the right features.

- [Guides Overview](guides/overview.mdx): Course structure and module overview
- [Define your feedback strategy](guides/define-your-feedback-strategy.mdx): Set goals before touching settings
- [Structure your workspace](guides/structure-your-workspace.mdx): Boards, statuses, and tags for your team
- [Launch your portal](guides/launch-your-portal.mdx): Get users submitting feedback
- [Triage feedback effectively](guides/triage-feedback-effectively.mdx): A repeatable review process
- [Write responses users love](guides/write-responses-users-love.mdx): Build trust with every response
- [Merge and organize](guides/merge-and-organize.mdx): Keep feedback clean as volume grows
- [Read the signals](guides/read-the-signals.mdx): Understand what users actually need
- [Build your roadmap](guides/build-your-roadmap.mdx): Public planning that builds trust
- [Align your team](guides/align-your-team.mdx): Multi-person feedback operations
- [Ship and announce](guides/ship-and-announce.mdx): Close the feedback loop
- [Measure and iterate](guides/measure-and-iterate.mdx): Program health and improvement
- [Segment your users](guides/segment-your-users.mdx): Prioritize by customer group
- [Automate your workflow](guides/automate-your-workflow.mdx): Reduce manual work with workflows and integrations
- [Internationalization](guides/internationalization.mdx): Locales for the portal and widget
- [Migrate from another tool](guides/migrate-from-another-tool.mdx): Switch from other platforms or spreadsheets

## For Users

- [Submit feedback](users/submitting-feedback.mdx): Share ideas and report bugs
- [Vote on feedback](users/voting.mdx): Support ideas you care about
- [Comment on posts](users/comments.mdx): Join the discussion
- [Get help from support](users/get-support.mdx): Chat with the team or file a ticket
- [Follow service status](users/status-updates.mdx): Status page and incident updates
- [Manage your notifications](users/notifications.mdx): Control your alerts
- [Manage your account](users/account.mdx): Profile and preferences

## For Admins

- [Triage feedback](admin/inbox.mdx): Filter, triage, and respond
- [Organize feedback with boards](admin/boards.mdx): Categorize by type
- [Track progress with statuses](admin/statuses.mdx): Define workflow stages
- [Categorize posts with tags](admin/tags.mdx): Label and filter
- [Build a public roadmap](admin/roadmap.mdx): Filter-based roadmap views
- [Review AI suggestions](admin/suggestions.mdx): Triage AI-captured feedback
- [Configure AI features](admin/ai-features.mdx): Summaries, duplicates, semantic search
- [Publish a changelog](admin/changelog.mdx): Announce what shipped
- [Moderate content](admin/moderation.mdx): Approval queues and anonymous access
- [Understand analytics](admin/analytics.mdx): Feedback and team metrics
- [Track visitor analytics](admin/visitors.mdx): Cookieless pageview analytics
- [Manage portal users](admin/users.mdx): Users, leads, and invitations
- [Manage companies](admin/companies.mdx): Company directory and attributes
- [Segment your users](admin/segments.mdx): Manual and dynamic segments
- [Configure admin notifications](admin/notifications.mdx): Team alert settings
- [Manage your team](admin/team.mdx): Members, teams, and roles
- [Roles and permissions](admin/roles-permissions.mdx): Role presets and the permission catalogue
- [Configure team security](admin/security.mdx): Team sign-in methods and audit log
- [Set up portal sign-in](admin/portal-auth.mdx): User authentication options
- [Customize your portal](admin/branding.mdx): Branding, navigation, and welcome card
- [Finish setup with the launch checklist](admin/getting-started.mdx): Goal-based setup tasks
- [Import from other tools](admin/imports.mdx): In-app import adapters
- [Import and export data](admin/import-export.mdx): CSV import and export
- [Search](admin/search.mdx): Find posts fast
- [Privacy and data](admin/privacy.mdx): Data handling, retention, and GDPR

## Support

- [Support overview](support/overview.mdx): Conversations, tickets, and the unified inbox
- [Work the support inbox](support/inbox.mdx): Queues, views, assignment, bulk actions
- [Handle conversations](support/conversations.mdx): Messenger chats, notes, CSAT
- [Manage support tickets](support/tickets.mdx): Statuses, categories, and customer-facing stages
- [Configure ticket types](support/ticket-types.mdx): Intake forms per ticket type
- [Set SLA policies](support/sla.mdx): Response and resolution targets
- [Use macros](support/macros.mdx): Saved replies and actions
- [Configure office hours](support/office-hours.mdx): Coverage windows and SLA timing
- [Save inbox views](support/saved-views.mdx): Reusable filter sets
- [Set up the email channel](support/channels.mdx): Inbound routing and sending domains
- [Set up a status page](support/status-pages.mdx): Services, incidents, maintenance, subscribers

## AI & Automation

- [AI & Automation overview](automation/overview.mdx): Quinn agents and the workflows engine
- [Configure the Quinn Agent](automation/quinn-agent.mdx): Customer-facing AI in Messenger
- [Use Quinn Copilot](automation/quinn-copilot.mdx): AI drafts and answers for teammates
- [Knowledge sources](automation/knowledge-sources.mdx): What Quinn can draw on
- [Give Quinn actions](automation/actions.mdx): Built-in and custom actions
- [Test and monitor Quinn](automation/test-and-monitor.mdx): Sandbox and performance
- [Build a workflow](automation/workflows.mdx): Triggers, actions, versions
- [Workflow blocks](automation/workflow-blocks.mdx): Conversational node reference
- [Start from a workflow template](automation/templates.mdx): Template gallery and funnels

## Authentication

- [Authentication](auth/overview.mdx): Overview of auth methods
- [Set up magic links](auth/magic-link.mdx): Passwordless email sign-in
- [Set up OAuth providers](auth/oauth.mdx): GitHub, Google, and more
- [Set up single sign-on](auth/sso.mdx): OIDC SSO

## Integrations

- [Integrations](integrations/overview.mdx): How integrations work
- [Send events with webhooks](integrations/webhooks.mdx): HTTP event notifications
- [Email](integrations/email.mdx): Notification email delivery
- Notifications: [Slack](integrations/slack.mdx), [Discord](integrations/discord.mdx), [Microsoft Teams](integrations/microsoft-teams.mdx)
- Issue trackers: [Linear](integrations/linear.mdx), [GitHub](integrations/github.mdx), [Jira](integrations/jira.mdx), [GitLab](integrations/gitlab.mdx), [Asana](integrations/asana.mdx), [ClickUp](integrations/clickup.mdx), [Monday](integrations/monday.mdx), [Trello](integrations/trello.mdx), [Notion](integrations/notion.mdx), [Shortcut](integrations/shortcut.mdx), [Azure DevOps](integrations/azure-devops.mdx)
- CRM and enrichment: [HubSpot](integrations/hubspot.mdx), [Intercom](integrations/intercom.mdx), [Zendesk](integrations/zendesk.mdx), [Salesforce](integrations/salesforce.mdx), [Freshdesk](integrations/freshdesk.mdx), [Stripe](integrations/stripe.mdx), [Segment](integrations/segment.mdx)
- Automation platforms: [Zapier](integrations/zapier.mdx), [Make](integrations/make.mdx), [n8n](integrations/n8n.mdx)

## Widget

- [Widget overview](widget/index.mdx): The embeddable panel
- [Install the widget](widget/installation.mdx): Embed snippet and SDK commands
- [Add Messenger chat](widget/chat.mdx): Conversations in the widget
- [Customize the widget](widget/customization.mdx): Hero backdrops and live preview
- [Identify users](widget/identify-users.mdx): Verified identity and SSO tokens
- [Widget events](widget/events.mdx): Host-page event reference
- [Session metadata](widget/metadata.mdx): Attach context to posts
- [Mobile SDKs](widget/mobile-sdks.mdx): iOS and Android wrappers

## Help Center

- [Help center](help-center/index.mdx): Knowledge base overview
- [Set up the help center](help-center/setup.mdx): Subdomain and visibility
- [Write articles](help-center/articles.mdx): Author and publish
- [Organize categories](help-center/categories.mdx): Structure your knowledge base
- [Search](help-center/search.mdx): Hybrid keyword and semantic search
- [Custom domains](help-center/custom-domains.mdx): Serve docs on your domain

## API Reference

- [API Overview](api/overview.mdx): Auth, pagination, errors, and the live Swagger UI
- [Tickets API](api/tickets.mdx): Read ticket data
- [Status API](api/status.mdx): Status page services and incidents
- [Health endpoints](api/health.mdx): Liveness and readiness probes

## MCP

- [MCP server](mcp/index.mdx): Connect AI agents to Quackback
- [MCP reference](mcp/reference.mdx): Tools, resources, and scopes

## Self-Hosting

- [Overview](self-hosting/overview.mdx): Pick a deployment path
- [System Requirements](self-hosting/requirements.mdx): Hardware and software
- [Deploy with Docker](self-hosting/docker.mdx): Recommended deployment
- [Deploy on Railway](self-hosting/railway.mdx): One-click template
- [Install without Docker](self-hosting/manual.mdx): Manual installation
- [Scale with multiple replicas](self-hosting/scaling.mdx): Web and worker roles
- [Receive email over IMAP](self-hosting/email-imap.mdx): Inbound email without webhooks
- [Set up a reverse proxy](self-hosting/reverse-proxy.mdx): Nginx, Caddy, Traefik
- [Config file](self-hosting/config-file.mdx): Declarative workspace configuration
- [Troubleshooting](self-hosting/troubleshooting.mdx): Common issues

## Developer Guide

- [Set up local development](developers/setup.mdx): Local environment
- [Architecture](developers/architecture.mdx): System design
- [Server Functions](developers/server-functions.mdx): RPC patterns
- [Database](developers/database.mdx): Schema and queries
- [Add a new feature](developers/adding-features.mdx): Feature development
- [Testing](developers/testing.mdx): Vitest and Playwright
- [Contribute to Quackback](developers/contributing.mdx): How to contribute

## Reference

- [Environment Variables](reference/environment-variables.mdx): Configuration options
- [CLI Reference](reference/cli.mdx): Command reference
- [Database Schema](reference/database-schema.mdx): Tables and relationships

## Support

- [GitHub Issues](https://github.com/quackbackio/quackback/issues): Bug reports
- [GitHub Discussions](https://github.com/quackbackio/quackback/discussions): Questions and ideas

## License

AGPL-3.0. See [LICENSE](https://github.com/quackbackio/quackback/blob/main/LICENSE) for details.
