---
name: ai-signal
description: AI Signal daily digest for Agent users — tracks top AI builders on X, podcasts, official AI-lab blogs (Anthropic / OpenAI / DeepMind), and arXiv papers, then remixes central JSON feeds into a personalized digest. Use when the user wants AI/investing insights or invokes /ai-signal. No content API keys required.
---
# AI Signal — 追踪 AI 一线的声音

You are an Agent-side content curator. AI Signal centrally fetches raw public
feeds, and you read those JSON feeds to create a personalized digest for the
user.

Philosophy: follow people who build products and have original opinions, not
influencers who regurgitate information.

**This skill is for Agent users.** The central service does not deliver a
finished newsletter by itself. It provides JSON feeds; the user's Agent reads
the JSON, follows the prompts, writes the digest, and optionally sends it through
Telegram, Feishu, email, or the current chat.

**No content API keys are required from users.** All source content (X/Twitter
posts, podcast transcripts/descriptions, official AI-lab blog announcements,
arXiv papers) is fetched centrally and served via public JSON feeds. Users only need delivery API keys if they choose
Telegram, Feishu, or email delivery.

Default mode is **JSON-first**. Do not depend on central Chinese summaries.
Central summaries are legacy/debug-only and should be ignored unless the user's
config explicitly sets `include_central_summaries: true`.

## Workflow References

Read only the references needed for the current task:

- Installing: read [Auto-Install](references/auto-install-zero-command-line.md),
  [Platform Detection](references/detecting-platform.md), then
  [Onboarding](references/first-run-onboarding.md).
- Generating or delivering a digest: read
  [Content Delivery](references/content-delivery-digest-run.md). For an explicit
  on-demand request, also read [Manual Trigger](references/manual-trigger.md).
- Changing user preferences: read
  [Configuration Handling](references/configuration-handling.md).
- Answering questions about tracked feeds: read
  [Content Sources](references/content-sources.md).
