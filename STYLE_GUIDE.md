# Quackback Documentation Style Guide

This guide establishes writing patterns for all Quackback documentation. Follow these principles to create docs that are welcoming, practical, and user-focused.

## Core Principles

### 1. User-First, Not Product-First

**Don't start with:** "Quackback is..." or "[Feature] is..."
**Start with:** What the user can accomplish or the problem solved

| Avoid | Use Instead |
|-------|-------------|
| "Quackback is an open-source feedback platform..." | "Collect, organize, and act on user feedback with a single source of truth." |
| "Boards organize feedback into categories." | "Stop losing feedback across emails, Slack, and spreadsheets. Boards keep everything in one place." |
| "Statuses represent the stages of your workflow." | "Track feedback from idea to shipped. Statuses show users what's happening with their requests." |

### 2. Lead with Benefits, Not Features

Every section should answer "why should I care?" before "what is this?"

**Pattern:**
1. Problem or benefit (1-2 sentences)
2. What it is (1 sentence)
3. How to use it (steps/details)

**Example:**

> **Before:** "Custom statuses allow you to define your own workflow stages."
>
> **After:** "Your workflow isn't one-size-fits-all. Create custom statuses that match how your team actually works, whether that's 'In Design', 'Awaiting Legal', or 'Beta Testing'."

### 3. Use Permission Language

Frame features as options, not demands.

| Avoid | Use Instead |
|-------|-------------|
| "Configure the settings" | "You can configure..." |
| "Create a board" | "You can create..." or "Create a board to..." |
| "You must enable SSO" | "Enable SSO to..." |

### 4. Acknowledge Pain Points

Show you understand the user's situation before presenting solutions.

**Examples:**
- "Tired of feedback scattered across emails, Slack, and spreadsheets?"
- "Switching status back and forth? That's fine. Priorities change."
- "Not sure which board to use? Start with just one and split later."

### 5. Questions as Section Headers

Replace declarative headers with questions when explaining optional features.

| Declarative | Question-Based |
|-------------|----------------|
| "Private Boards" | "Need to keep feedback internal?" |
| "Custom Statuses" | "Want a workflow that fits your team?" |
| "SSO Configuration" | "Ready to enable single sign-on?" |

### 6. Default-First Explanations

Always explain what works out of the box before customization.

**Pattern:**
> "By default, [feature] works like [this]. You can customize it by..."

**Example:**
> "By default, posts start in 'Under Review' status. You can change this in Admin → Settings → Statuses, or create custom statuses to match your workflow."

---

## Writing Patterns

### Opening Paragraphs

**Formula:** [Outcome/Benefit]. [What it is]. [Quick context if needed].

**Examples:**

| Page | Bad Opening | Good Opening |
|------|-------------|--------------|
| Introduction | "Quackback is an open-source customer feedback platform that helps you collect, organize, and act on user feedback." | "Stop losing feedback. Quackback brings user requests, votes, and discussions into one place so you can build what users actually want." |
| Boards | "Boards organize feedback into categories, making it easier for users to submit and for your team to manage." | "Keep feature requests separate from bug reports. Boards let you organize feedback the way that makes sense for your product." |
| SSO | "Configure Single Sign-On to allow users to authenticate with your organization's identity provider." | "One less password for your users to remember. SSO lets customers sign in with their existing work accounts." |

### Inline Tips and Guidance

**Place tips at the point of decision, not at the end of the page.**

Use `<Tip>`, `<Note>`, or `<Warning>` callouts immediately after the relevant instruction.

```markdown
## Creating a Board

1. Go to **Admin → Settings → Boards**
2. Click **"New board"**

<Tip>
Start with just 2-3 boards. You can always add more later, but too many boards confuse users about where to post.
</Tip>
```

### Communication Templates

For user-facing features, provide copy-paste text that users can adapt.

**Example for Status Changes:**

```markdown
## Communicating Status Changes

When you update a status, add a comment so users know why. Here are templates:

**Moving to Planned:**
> "We've added this to our roadmap! Thanks for the suggestion. We'll keep you posted."

**Moving to Declined:**
> "After reviewing, we've decided to go a different direction. [Brief reason]. We appreciate you sharing this idea."

**Reverting to Under Review:**
> "We're putting this back under review. Our priorities shifted, but we haven't forgotten about it."
```

---

## Structural Patterns

### Page Template

```markdown
---
title: "[Action-Oriented Title]"
description: "[Benefit-focused description, <160 chars]"
icon: "[icon-name]"
---

# [Title]

[Opening: 1-2 sentences on benefit/outcome]

## Overview / Why [Feature]?

[Problem acknowledgment + solution framing]

## Getting Started / Quick Start

[Fastest path to value - numbered steps]

<Tip>
[Practical guidance at point of decision]
</Tip>

## [Core Feature Sections]

[Details organized by user task, not by feature]

## Tips & Best Practices

[Consolidated wisdom - but key tips should also appear inline]

## Troubleshooting

[Common issues with solutions]

## Next Steps

[Links to related pages]
```

### Section Headings

- Use **verbs** for task sections: "Creating a Board", "Configuring SSO"
- Use **questions** for optional/advanced: "Need private boards?"
- Use **nouns** sparingly, only for reference: "Status Reference"

---

## Callout Usage

### `<Tip>` - Helpful Shortcuts

For optional but valuable information. Use for best practices and shortcuts.

```markdown
<Tip>
**Start simple** - Begin with the default statuses. Add custom ones only when you feel limited.
</Tip>
```

### `<Note>` - Contextual Information

For clarifications that prevent confusion. Use when something might not be obvious.

```markdown
<Note>
Team members can also use the public portal like regular users, in addition to having admin access.
</Note>
```

### `<Warning>` - Destructive or Important

For irreversible actions or critical requirements. Use sparingly for impact.

```markdown
<Warning>
Deleting a board also deletes all posts in that board. This cannot be undone.
</Warning>
```

### `<Info>` - Additional Context

For supplementary information that's helpful but not critical.

```markdown
<Info>
Users are automatically subscribed to posts they create or vote on.
</Info>
```

---

## Voice & Tone

### Do

- Use "you" and "your" to address the reader directly
- Write in present tense
- Keep sentences short (aim for 15-20 words)
- Keep paragraphs short (2-4 sentences max)
- Use contractions: "you'll", "don't", "it's"
- Be direct: "Click Save" not "You should click Save"

### Don't

- Don't use passive voice: ~~"The board can be configured"~~ → "You can configure the board"
- Don't use jargon without explanation
- Don't use marketing superlatives: ~~"powerful"~~, ~~"seamless"~~, ~~"best-in-class"~~
- Don't hedge: ~~"simply"~~, ~~"just"~~, ~~"easily"~~ (if it were easy, you wouldn't need docs)

---

## Examples Reference

### Real-World Examples

Use concrete examples, not abstract descriptions:

| Abstract | Concrete |
|----------|----------|
| "Create multiple boards for different feedback types" | "Create boards like 'Feature Requests', 'Bug Reports', and 'Integrations'" |
| "Set up custom statuses" | "Add statuses like 'In Design', 'In Beta', or 'Blocked'" |
| "Configure your roadmap columns" | "Most teams use: Planned → In Progress → Shipped" |

### Code Examples

- Always include complete, runnable examples
- Add comments explaining the "why"
- Show the callback URL or endpoint clearly

```typescript
// Replace 'your-workspace-id' with your actual workspace ID
// Found in Admin → Settings → General
<QuackbackWidget workspaceId="your-workspace-id" theme="dark" />
```

---

## Checklist for Every Page

Before publishing any doc, verify:

- [ ] Opening paragraph focuses on benefit/outcome, not product definition
- [ ] At least one `<Tip>`, `<Note>`, or `<Warning>` callout appears inline
- [ ] All paragraphs are 4 sentences or fewer
- [ ] No passive voice in instructional content
- [ ] Real-world examples are provided where applicable
- [ ] Links to related pages appear at the end
