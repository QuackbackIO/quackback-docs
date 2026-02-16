# Quackback Documentation Style Guide

This guide establishes writing patterns for all Quackback documentation. Follow these principles to create docs that are welcoming, practical, and user-focused.

Inspired by the best developer documentation (Stripe, Vercel, Linear), adapted for Quackback's voice.

---

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

### 5. Default-First Explanations

Always explain what works out of the box before customization.

**Pattern:**
> "By default, [feature] works like [this]. You can customize it by..."

**Example:**
> "By default, posts start in 'Under Review' status. You can change this in Admin > Settings > Statuses, or create custom statuses to match your workflow."

### 6. Progressive Disclosure

Introduce complexity only when the reader is ready for it.

- Don't front-load prerequisites. Introduce them just before they're needed.
- Don't explain everything on one page. Link to deeper content.
- Concepts pages should cover only what's needed to get started. Advanced topics belong on their own pages.

**Pattern:**
> Mention a concept briefly with a link > Reader follows the link only if they need depth

**Example:**
> "Payloads are signed with HMAC-SHA256 so you can [verify they came from Quackback](/integrations/webhooks#signature-verification)."
>
> Don't: Explain HMAC-SHA256 inline on the concepts page.

---

## Titles & Headings

### Page Titles

Use **imperative verbs** for task/guide pages. Use **nouns** for reference pages.

| Type | Pattern | Examples |
|------|---------|----------|
| **Guide/Task** | Imperative verb + object | "Organize feedback with boards", "Set up Slack notifications" |
| **Reference** | Noun phrase | "Environment Variables", "Database Schema", "API Overview" |
| **Concept** | Noun or short phrase | "Core Concepts", "Authentication" |

Avoid gerunds ("Managing Boards", "Configuring SSO"). Use imperatives instead ("Organize feedback with boards", "Set up single sign-on").

**Title length:** Keep under 50 characters. The title should be scannable in a sidebar.

### Section Headings

- Use **imperative verbs** for task sections: "Create a board", "Configure event mappings"
- Use **questions** for optional/advanced features: "Need to keep feedback internal?"
- Use **nouns** sparingly, only for pure reference: "Status Reference", "Error Codes"

### Descriptions (frontmatter)

One sentence. Lead with a verb. Under 160 characters. State the outcome.

| Weak | Strong |
|------|--------|
| "Learn about boards and how they work" | "Organize feedback into categories so users know where to post" |
| "API documentation for Quackback" | "Build integrations with Quackback's REST API" |

---

## Writing Patterns

### Opening Paragraphs

**Formula:** [Outcome/Benefit]. [What it is]. [Quick context if needed].

Keep it to 1-2 sentences. Cut ruthlessly.

| Page | Weak Opening | Strong Opening |
|------|-------------|--------------|
| Introduction | "Quackback is an open-source customer feedback platform that helps you collect, organize, and act on user feedback." | "Stop losing feedback. Quackback brings user requests, votes, and discussions into one place so you can build what users actually want." |
| Boards | "Boards organize feedback into categories, making it easier for users to submit and for your team to manage." | "Keep feature requests separate from bug reports. Boards organize feedback the way that makes sense for your product." |
| SSO | "Configure Single Sign-On to allow users to authenticate with your organization's identity provider." | "One less password for your users. SSO lets customers sign in with their existing work accounts." |

### Inline Cross-Linking

Link concepts **inline within sentences**, not just in "Next Steps" sections. When you mention a concept, link to it right there.

**Do:**
> "Posts move through [statuses](/admin/statuses) as your team works on them."

**Don't:**
> "Posts move through statuses as your team works on them. (See: Managing Statuses)"

Keep "Next Steps" sections too, but inline links are the primary discovery mechanism.

### Inline Tips and Guidance

**Place tips at the point of decision, not at the end of the page.**

Use `<Tip>`, `<Note>`, or `<Warning>` callouts immediately after the relevant instruction.

```markdown
## Create a board

1. Go to **Admin > Settings > Boards**
2. Click **"New board"**

<Tip>
Start with 2-3 boards. You can always add more later, but too many boards confuse users about where to post.
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

### Context Labels

For pages that involve multiple environments (client/server, dashboard/API, your server/Quackback), label sections clearly.

**Pattern:**
```markdown
### [Dashboard] Create an API key

### [Your Server] Verify the webhook signature

### [Quackback API] Create a post
```

This removes ambiguity about where an action happens.

---

## Page Templates

Every page should follow one of these templates. Consistency means readers always know where to find what they need.

### Guide Page (task-oriented)

For pages that walk users through accomplishing something.

```markdown
---
title: "[Imperative verb phrase]"
description: "[Outcome in one sentence, <160 chars]"
icon: "[icon-name]"
---

# [Title]

[1-2 sentence opening: what this accomplishes and why]

## Prerequisites

[Only what's immediately needed, not a general knowledge dump]

## [Step-oriented sections with imperative headings]

[Numbered steps with code samples]

<Tip>
[Practical guidance at point of decision]
</Tip>

## Verify it works

[How to confirm the setup is correct]

## Next steps

[2-3 links to related pages]
```

### Concept Page (understanding-oriented)

For pages that explain how something works.

```markdown
---
title: "[Noun or short phrase]"
description: "[What the reader will understand, <160 chars]"
icon: "[icon-name]"
---

# [Title]

[1-2 sentence benefit-focused opening]

## [Core concept sections]

[Explain each concept briefly. Link to the full guide page for details.]
[Don't duplicate content from guide pages. Summarize and link.]

## Next steps

[Links to guide pages where the reader can take action]
```

**Key rule:** Concept pages should be **concise summaries that link out**, not exhaustive references. If a section is longer than 8-10 lines, it belongs on its own page.

### Reference Page (information-oriented)

For pages that serve as lookup resources.

```markdown
---
title: "[Noun phrase]"
description: "[What this reference covers, <160 chars]"
icon: "[icon-name]"
---

# [Title]

[1 sentence scope statement]

## [Grouped sections]

[Tables, code examples, specifications]
[Minimal prose. Let the data speak]
```

### Hub Page (navigation-oriented)

For section landing pages that help users find the right sub-page.

```markdown
---
title: "[Section name]"
description: "[What this section covers, <160 chars]"
icon: "[icon-name]"
---

# [Title]

[1-2 sentence framing: what this section helps users accomplish]

## [Category groupings]

[Card-style links: **Bold title**: single sentence description]
[Organize by user intent, not by product taxonomy]
```

Hub pages should contain **almost no tutorial content**. They're curated navigation. If you're writing more than 2-3 sentences of explanation per link, the content belongs on the linked page instead.

---

## Navigation Patterns

### Intent-Based Navigation

Organize navigation by what users want to accomplish, not by product entities.

| Entity-Based (avoid as primary nav) | Intent-Based (prefer) |
|------|--------|
| Boards | Organize feedback by category |
| Statuses | Track progress from request to shipped |
| Tags | Label and filter posts |
| Roadmap | Show users what you're building |
| Webhooks | Get notified when feedback arrives |

Use intent-based framing on hub pages, README quick links, and sidebar descriptions. The actual page titles can stay shorter.

### Multiple Entry Points

The same content should be reachable from multiple paths:
- From the section hub page
- From the README quick links table
- From inline links in related pages
- From the "Next steps" section of prerequisite pages

### "I want to..." Table

The README should include a quick-links table organized by user intent:

```markdown
| I want to... | Go to... |
|--------------|----------|
| Deploy Quackback | Quick Start |
| Organize feedback | Boards |
| Track what's planned | Roadmap |
| Connect to Slack | Slack Integration |
| Build a custom integration | API Overview |
```

---

## Code Examples

### Completeness

Always include complete, runnable examples. Never pseudocode.

### Multi-Language Tabs

For API documentation, provide examples in multiple languages where possible:

```markdown
<CodeGroup>
  <CodeBlock title="curl">
  ```bash
  curl -X POST https://feedback.example.com/api/v1/posts \
    -H "Authorization: Bearer qb_your_api_key" \
    -H "Content-Type: application/json" \
    -d '{"boardId": "board_01h4...", "title": "Add dark mode"}'
  ```
  </CodeBlock>

  <CodeBlock title="JavaScript">
  ```javascript
  const response = await fetch('https://feedback.example.com/api/v1/posts', {
    method: 'POST',
    headers: {
      'Authorization': 'Bearer qb_your_api_key',
      'Content-Type': 'application/json',
    },
    body: JSON.stringify({
      boardId: 'board_01h4...',
      title: 'Add dark mode',
    }),
  });
  ```
  </CodeBlock>

  <CodeBlock title="Python">
  ```python
  import requests

  response = requests.post(
      "https://feedback.example.com/api/v1/posts",
      headers={"Authorization": "Bearer qb_your_api_key"},
      json={"boardId": "board_01h4...", "title": "Add dark mode"},
  )
  ```
  </CodeBlock>
</CodeGroup>
```

Priority order: **curl > JavaScript > Python**. These three cover the vast majority of API consumers.

### Code Comments

Comments should explain **why**, not **what**. Use recognizable placeholders for credentials.

```typescript
// Replace with your workspace's API key
// Found in Admin > Settings > API Keys
const API_KEY = "qb_your_api_key";
```

---

## Callout Usage

### `<Tip>` - Helpful Shortcuts

For optional but valuable information. Use for best practices and shortcuts.

```markdown
<Tip>
**Start simple.** Begin with the default statuses. Add custom ones only when you feel limited.
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
- Keep sentences short (aim for 15 words or fewer)
- Keep paragraphs short (2-3 sentences max, never more than 4)
- Use contractions: "you'll", "don't", "it's"
- Be direct: "Click Save" not "You should click Save"
- Cut every word that doesn't add meaning

### Don't

- Don't use passive voice: ~~"The board can be configured"~~ > "You can configure the board"
- Don't use jargon without explanation
- Don't use marketing superlatives: ~~"powerful"~~, ~~"seamless"~~, ~~"best-in-class"~~
- Don't hedge: ~~"simply"~~, ~~"just"~~, ~~"easily"~~ (if it were easy, you wouldn't need docs)
- Don't use gerund titles: ~~"Managing Boards"~~ > "Organize feedback with boards"
- Don't use "How to..." titles: ~~"How to Set Up Slack"~~ > "Set up Slack notifications"

### Conciseness Standards

Stripe-level docs earn every word. Apply these targets:

| Element | Target |
|---------|--------|
| Page title | Under 50 characters |
| Frontmatter description | Under 160 characters, one sentence |
| Opening paragraph | 1-2 sentences |
| Link card descriptions | Under 65 characters |
| Callout text | 1-3 sentences |
| Section intro | 1-2 sentences before getting to steps/content |

---

## Examples Reference

### Real-World Examples

Use concrete examples, not abstract descriptions:

| Abstract | Concrete |
|----------|----------|
| "Create multiple boards for different feedback types" | "Create boards like 'Feature Requests', 'Bug Reports', and 'Integrations'" |
| "Set up custom statuses" | "Add statuses like 'In Design', 'In Beta', or 'Blocked'" |
| "Configure your roadmap columns" | "Most teams use: Planned > In Progress > Shipped" |

---

## Checklist for Every Page

Before publishing any doc, verify:

- [ ] **Title** uses imperative verb (guide pages) or noun (reference pages)
- [ ] **Opening paragraph** focuses on benefit/outcome, not product definition
- [ ] **Opening** is 1-2 sentences max
- [ ] **Frontmatter description** is one sentence, under 160 characters, starts with a verb
- [ ] At least one `<Tip>`, `<Note>`, or `<Warning>` callout appears inline at point of decision
- [ ] All paragraphs are 4 sentences or fewer
- [ ] No passive voice in instructional content
- [ ] No gerund headings ("Managing...", "Configuring...")
- [ ] Real-world examples are provided where applicable
- [ ] Concepts are linked inline when first mentioned, not just in "Next Steps"
- [ ] Code examples are complete and runnable
- [ ] API code examples include curl + JavaScript + Python tabs
- [ ] "Next Steps" section links to 2-3 related pages
- [ ] Page follows the correct template (guide / concept / reference / hub)
- [ ] No words that don't earn their place, every sentence passes the "can I cut this?" test
