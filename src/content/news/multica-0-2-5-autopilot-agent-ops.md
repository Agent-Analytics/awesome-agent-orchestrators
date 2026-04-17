---
title: "Multica 0.2.5 adds autopilot commands and deeper agent work controls"
description: "Multica released 0.2.5 with autopilot commands, issue subscriber commands, persistent daemon identity, progress cards, and command-palette improvements."
date: 2026-04-17T09:39:30Z
playerSlug: "multica"
sourceName: "Multica v0.2.5 GitHub release"
sourceUrl: "https://github.com/multica-ai/multica/releases/tag/v0.2.5"
category: "Release"
tags:
  - orchestration
  - coding-agents
  - autopilot
  - agent-ops
draft: false
---

Multica released `v0.2.5` on April 17, 2026 with a broad batch of CLI, desktop, daemon, issue, workspace, and autopilot changes. The release adds `issue subscriber` commands, new autopilot commands, persistent daemon identity, project/sub-issue progress cards, command-palette actions, and several fixes around autopilot-created issues and daemon workspace resolution.

The important signal is that Multica keeps turning managed coding agents into something closer to a team operating surface. Subscribers, autopilot commands, progress cards, project-aware CLI commands, and machine-scoped daemon identity are the kinds of controls teams need when agent work is no longer a one-off chat session.

For operators and builders, this release is worth testing around the handoff points: who gets notified when an agent creates or updates an issue, how autopilot-created work is tracked, whether CLI and desktop identity stay aligned, and how project/sub-issue progress appears in the board. The release also includes UI and safety-adjacent fixes such as typed delete confirmation, sole-owner leave preflight, external-link scheme restrictions, and duplicate agent-name handling.

Source confidence: High.

Evidence:

- [Multica v0.2.5 GitHub release](https://github.com/multica-ai/multica/releases/tag/v0.2.5)
- [Multica GitHub repository](https://github.com/multica-ai/multica)
- [Multica official homepage](https://multica.ai/)

Explicit non-claims:

- This update does not claim that every `v0.2.5` change applies equally to hosted, desktop, and self-hosted usage.
- This update does not claim autopilot is fully autonomous or production-safe without operator review.
- This update does not rely on third-party social posts as release evidence.
