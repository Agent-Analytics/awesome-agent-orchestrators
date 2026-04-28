---
title: "Paperclip v2026.427.0 turns the agent company OS into a shared control plane"
description: "Paperclip released v2026.427.0 with multi-user access, invite flows, structured issue-thread interactions, liveness recovery, sub-issue checklists, subtree pause/cancel/restore, and beta sandbox environments."
date: 2026-04-27T15:01:40Z
playerSlug: "paperclip"
sourceName: "Paperclip v2026.427.0 GitHub release"
sourceUrl: "https://github.com/paperclipai/paperclip/releases/tag/v2026.427.0"
category: "Release"
tags:
  - orchestration
  - approvals
  - sandboxes
  - collaboration
draft: false
---

Paperclip released `v2026.427.0` on 2026-04-27, and the center of gravity is clear: Paperclip is moving from a local agent-company board toward a shared, authenticated control plane for human and agent work.

The headline changes are not just UI polish. They affect who can operate the system, how agents ask for decisions, how interrupted work resumes, and where agent runs execute.

Highlights:

- Multi-user access and invite flows make Paperclip a shared, authenticated control plane with real human identities, company memberships, onboarding, profile settings, and company-scoped access controls.
- Structured issue-thread interactions let agents post suggested tasks, multi-question forms, and request-for-confirmation cards directly into the thread.
- The board can render those proposals as interactive accept, reject, answer, and resume flows, making plan approvals and yes/no decisions explicit and replayable.
- Run liveness continuations record liveness state, next-action hints, continuation attempts, and operator-visible recovery decisions for long or interrupted work.
- Sub-issues now act more like workflow checklists, with dependency-aware progress, current-step affordances, blocker context, and de-emphasized completed work.
- Issue subtree pause, cancel, and restore gives operators a durable way to hold or stop a whole branch of work rather than chasing individual child issues.
- Beta environments add first-class execution targets with lease lifecycle tracking, including local, SSH-backed remote, and sandboxed providers.
- The new `@paperclipai/plugin-e2b` package is the reference third-party sandbox provider for the environment system.
- Plugin orchestration host APIs let plugins request namespaced databases, register orchestration hosts, and expose richer APIs back to the control plane.
- A first-class security agent role makes security responsibilities explicit in the org chart and route coverage.

For Open Orchestrators readers, the important shift is that Paperclip is adding more of the missing operating system around agent work: identity, access, approval cards, continuation state, dependency-aware execution, environment leases, sandbox providers, and subtree-level controls.

That matters because multi-agent systems rarely fail only because an agent cannot write code. They fail when ownership is unclear, approvals vanish into chat, interrupted runs cannot be recovered, or sandboxed execution is bolted on after the fact. This release pushes those concerns into the product surface.

Operators should read the full release notes before upgrading. The release includes fourteen additive database migrations, a new environment/provider model, API route authorization hardening, and an upgrade note for anyone previously using in-tree sandbox execution.

Source confidence: High. The article is based on the official Paperclip GitHub release.

Evidence:

- [Paperclip v2026.427.0 GitHub release](https://github.com/paperclipai/paperclip/releases/tag/v2026.427.0)
- [Paperclip GitHub repository](https://github.com/paperclipai/paperclip)
- [Open Orchestrators Paperclip player note](https://openorchestrators.org/players/paperclip/)

Explicit non-claims:

- This update does not claim the beta environment and sandbox-provider system is stable for every production deployment.
- This update does not claim Paperclip has replaced external project-management, identity, or security-review systems.
- This update does not rely on private adoption claims or social posts as source evidence.
