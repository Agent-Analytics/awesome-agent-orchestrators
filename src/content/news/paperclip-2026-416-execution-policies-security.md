---
title: "Paperclip v2026.416.0 turns issues into governed agent work"
description: "Paperclip released v2026.416.0 with chat-style issue threads, execution policies, blocker-aware wakes, parent-child tasks, MCP server work, and security fixes."
date: 2026-04-16T15:20:00Z
playerSlug: "paperclip"
sourceName: "Paperclip v2026.416.0 GitHub release"
sourceUrl: "https://github.com/paperclipai/paperclip/releases/tag/v2026.416.0"
category: "Release"
tags:
  - orchestration
  - approvals
  - security
  - mcp
draft: false
---

Paperclip released `v2026.416.0` on 2026-04-16 with a broad pass across the surfaces that matter when agents are doing real work: issue context, approval flow, dependencies, plugins, runtime control, and security. It is still one release, but it changes the feeling of the product from "agents working through tickets" toward "a company queue with visible runs and enforceable rules."

Highlights:

- Issue pages now carry the agent run as a chat-like story, so transcripts and user replies sit together instead of being scattered through a timeline.
- Execution policies bring review and approval stages into the issue itself, with Paperclip moving work through the selected signoff path.
- Blockers now have runtime behavior: when upstream issues finish, Paperclip can wake the blocked assignee automatically.
- Parent and child issues are easier to navigate, with nested inbox groups and sub-issues pulled into the detail view.
- The new beta `@paperclipai/mcp-server` turns Paperclip into an MCP tool surface, including tools for approval creation.
- Adapter plugins become more portable because external adapters can load from npm packages or local directories.
- Agent runs get practical workflow upgrades: scoped checkout on comment wakes, automatic skill enablement for heartbeat runs, skill autocomplete, Codex fast mode, Bedrock model selection for Claude, and a worktree reseed command.
- The rest is the kind of release-note bulk operators care about later: search, backups, mobile layout, keyboard shortcuts, runtime controls, issue-detail stability, and transcript parsing fixes.

For Open Orchestrators readers, the important shift is that Paperclip keeps moving from "agents can work on issues" toward "agent work can be governed like company work." Review stages, approval creation, blocker-aware wakes, task nesting, and visible transcripts are all orchestration primitives, not just UI polish.

Operators should still read the full release notes before upgrading. This release includes authorization hardening for import, approval, activity, and heartbeat API routes tied to `GHSA-68qg-g8mg-6pr7`, removes a hardcoded JWT secret fallback, redacts Bearer tokens in server logs, includes dependency security bumps, and ships eight additive database migrations. The search migration requires PostgreSQL `pg_trgm` extension support.

Source confidence: High. The article is based on the official GitHub release and public advisory link.

Evidence:

- [Paperclip v2026.416.0 GitHub release](https://github.com/paperclipai/paperclip/releases/tag/v2026.416.0)
- [Paperclip GitHub repository](https://github.com/paperclipai/paperclip)
- [GHSA-68qg-g8mg-6pr7 advisory](https://github.com/cryppadotta/paperclip/security/advisories/GHSA-68qg-g8mg-6pr7)
- [Open Orchestrators Paperclip player note](https://openorchestrators.org/players/paperclip/)

Explicit non-claims:

- This update does not claim every Paperclip deployment is affected in the same way by the security advisory.
- This update does not claim the beta MCP server is a stable API surface.
- This update does not replace each operator's own upgrade, migration, and security review.
- This update does not rely on social posts or private adoption claims as source evidence.
