---
type: learning
created: 24.06.2026
tags: [#source/article, #area/work]
source: https://medium.com/@AnalyticsAtMeta/how-we-built-an-ai-second-brain-for-60k-knowledge-workers-78c507dd795b
author: Analytics at Meta
status: draft
related: []
---

# How We Built an AI Second Brain for 60K Knowledge Workers

> [!info] Source
> **Type**: #source/article
> **Author**: Analytics at Meta
> **Link**: https://medium.com/@AnalyticsAtMeta/how-we-built-an-ai-second-brain-for-60k-knowledge-workers-78c507dd795b

## Summary

Meta built an "AI Second Brain": an agent with persistent, structured access to a person's work that carries context across every interaction, rather than starting each session cold. It began in the analytics org and grew organically to 60,000+ users across engineering, PM, design, legal, finance, comms, and sales, with roughly 10,000 daily active users. The system rests on four pieces: a PARA-based workspace, an infrastructure layer connecting internal tools, the agent (model + harness), and skills written as markdown.

## Key Takeaways

1. **PARA gives the agent a map.** Tiago Forte's PARA framework (Projects, Areas, Resources, Archives) was built for humans but works for agents too: it tells the agent what's active, what matters, and where new information belongs. A root `CLAUDE.md` holds identity and active portfolio; per-project `CLAUDE.md` files hold detail.
2. **Progressive disclosure beats context dumping.** Loading everything degrades output quality. The agent starts each session with lean root context and drills into project folders only when needed. Skills follow the same pattern: a short description until invoked.
3. **Infrastructure comes first.** Authenticated, scoped access to internal tools (via MCP servers and CLIs) is what separates a useful agent from a chatbot. Without it the agent can only read local files.
4. **The agent is a model plus a harness.** The harness provides the agentic loop (reason, act, observe, repeat), filesystem access, tool calling, and error recovery. Their deployment runs on Claude Code, but the architecture is harness-agnostic.
5. **Skills are reusable workflows in plain markdown.** No compiled code or servers. Examples: `/para-init` (bootstrap a workspace), `/start-project` (project from a brain dump), `/read-meeting-notes` (route notes to the right project), `/debrief:team` (manager-level rollup).
6. **Low-friction onboarding drove viral adoption.** `/para-init` let users see value in their first session. A non-technical PM's post in February ("I finally built my second brain") spread it across every function within days.
7. **Users became the builders.** Every major feature after launch (laptop support, Drive optimization, meeting-note processing, visual reporting, shared team context) came from the community, not the original author. Composability turned the plugin into a platform.

## Quotes

> "Not a chatbot that answers questions, but a working partner that tracks projects, reads meeting notes, surfaces connections, and builds on prior conversations."

> "Lean context up front, deeper detail on demand."

> "The plugin stopped being a tool and became a platform, and each extension made the whole system more useful for everyone."

## How I'll Apply This

- Notice that this vault already mirrors the article's core ideas: a root `CLAUDE.md` for conventions, folders by type, and skills as markdown. The PARA "lifecycle" angle (Projects / Areas / Resources / Archives) is one lens to compare against the current structure.
- Watch for progressive disclosure in practice: keep root context lean, push detail into per-note or per-project context.

## Related Ideas

-
