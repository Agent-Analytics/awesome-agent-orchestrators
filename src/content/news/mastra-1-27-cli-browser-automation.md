---
title: "Mastra 1.27 adds CLI-driven browser automation and Studio screencasts"
description: "Mastra's April 24 release adds BrowserViewer and BrowserCliHandler so CLI-based agent workflows can launch or connect to browser sessions, pass CDP endpoints, and stream live screencasts into Studio."
date: 2026-04-24T09:58:42Z
playerSlug: "mastra"
sourceName: "Mastra GitHub release"
sourceUrl: "https://github.com/mastra-ai/mastra/releases/tag/%40mastra/core%401.27.0"
category: "Release"
tags:
  - orchestration
  - browser-automation
  - coding-agents
  - cli-agents
  - observability
draft: false
---

Mastra's `@mastra/core@1.27.0` release adds CLI-driven browser automation through `@mastra/browser-viewer`, `BrowserViewer`, and `BrowserCliHandler`. The release says the new browser layer can launch Chrome with Playwright remote debugging, detect browser CLIs such as `agent-browser`, `browser-use`, and `browse`, inject the CDP URL into commands, and stream live screencasts into Mastra Studio.

This matters for Open Orchestrators readers because browser control is becoming part of the agent runtime surface rather than a separate demo layer. A production agent workflow increasingly needs code execution, browser interaction, operator visibility, and replayable state in one loop. Mastra's release is notable because it connects CLI-based agents to browser sessions while also making the session visible through Studio.

For builders, the practical signal is that Mastra is moving beyond framework primitives toward operator-grade agent workflows. Thread-isolated browser sessions, lifecycle management, external CDP endpoint support, and Studio screencasts all point at the same category direction: agents need observable tools to inspect and act on web products, not just call APIs or edit code.

The release also includes S3 prefix mounts for workspace providers, more robust workflow resumes for parallel `foreach`, observational memory improvements, and a new `@mastra/tavily` package. Those are useful, but the browser automation and screencast capability is the strongest Open Orchestrators angle because it changes what a Mastra-based agent workflow can operate and what a human can watch.

Source confidence: High for the release contents. Medium for downstream workflow impact because the release describes the capability surface but does not publish independent reliability or task-success benchmarks.

Evidence:

- [Mastra `@mastra/core@1.27.0` GitHub release](https://github.com/mastra-ai/mastra/releases/tag/%40mastra/core%401.27.0)
- [Mastra GitHub repository](https://github.com/mastra-ai/mastra)
- [Mastra website](https://mastra.ai/)

Explicit non-claims:

- This update does not claim that Mastra's browser automation supports every browser CLI or cloud browser provider.
- This update does not benchmark browser-task success rates.
- This update does not claim that Studio screencasts replace full session replay, analytics, or product instrumentation.
