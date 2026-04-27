---
title: "Orca v1.3.21 pushes agent IDE workflows deeper into PR review"
description: "Orca's latest releases turn PR review into a first-class agent IDE flow: open a worktree from a pull request, ask an agent to review it, and send inline comments through gh, while v1.3.21 adds more PR and terminal setup polish."
date: 2026-04-27T07:30:00Z
playerSlug: "orca"
sourceName: "Orca GitHub release"
sourceUrl: "https://github.com/stablyai/orca/releases/tag/v1.3.21"
category: "Release"
tags:
  - orchestration
  - coding-agents
  - pr-review
  - worktrees
  - agent-ide
draft: false
---

Orca's latest release run makes PR review feel less like an external checklist and more like a native agent-IDE workflow. The clearest product signal came from Orca's own Apr 26 post: an AI can now review pull requests end to end in Orca by spinning up a worktree from the PR, asking the agent to review it, and having it leave inline comments through `gh` without disturbing the current branch.

The fresh stable anchor is `v1.3.21`, published Apr 27. Its release notes add more operator-facing polish around server-side task scope filtering, pagination, PR checks and comments, SSH file search, and terminal setup. Orca's official X account also framed the same release window around everyday IDE adoption details: Ghostty settings import, live terminal preview, Vue single-file-component highlighting, and ligature support.

This matters for Open Orchestrators readers because the direction is broader than one IDE nicety. Orca is making agent work visible and reviewable inside the local development loop: worktrees, diffs, comments, terminal settings, syntax support, and PR state are all becoming part of the operator surface around coding agents. That is what turns "run an agent" into "manage agent work."

For builders, the practical signal is that PR review is becoming an agent workflow surface. If an agent can inspect a PR in an isolated worktree, read diffs, receive line-level human intent, and leave comments through the same tooling developers already use, the IDE becomes a coordination layer between humans, agents, branches, and review systems.

The smaller terminal and language-support updates still matter because adoption often happens through workflow fit. Ghostty import, Vue highlighting, and ligatures do not create an orchestration platform by themselves, but they remove friction for developers who want the agent IDE to feel like their normal coding environment rather than a separate demo app.

Source confidence: High for the `v1.3.21` release and official Orca X posts. Medium for downstream workflow implications because the posts and release notes describe capability surfaces, not measured PR-review success rates.

Evidence:

- [Orca v1.3.21 GitHub release](https://github.com/stablyai/orca/releases/tag/v1.3.21)
- [Orca official X post on PR review in v1.3.18](https://x.com/orca_build/status/2048192633688997940)
- [Orca official X post on Ghostty settings import in v1.3.21](https://x.com/orca_build/status/2048666107146637467)
- [Orca official X post on Vue SFC highlighting in v1.3.20](https://x.com/orca_build/status/2048553320525242587)
- [Orca GitHub repository](https://github.com/stablyai/orca)

Explicit non-claims:

- This update does not claim Orca's PR-review flow autonomously guarantees review quality.
- This update does not benchmark agent PR-review accuracy or compare it against GitHub-native review tools.
- This update does not claim every feature named here first appeared in `v1.3.21`; the story covers Orca's latest release run, anchored by the Apr 27 stable release.
