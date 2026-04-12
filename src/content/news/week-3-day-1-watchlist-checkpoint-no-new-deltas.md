---
title: "Week-3 Day-1 checkpoint: no new watchlist deltas since the Week-2 baseline"
description: "A canonical-source re-check found continuity across the tracked watchlist: no net-new release-channel changes since the Week-2 baseline in OPE-37."
date: 2026-04-12T03:49:57Z
playerSlug: "crewai"
sourceName: "LangGraph release-by-tag API"
sourceUrl: "https://api.github.com/repos/langchain-ai/langgraph/releases/tags/1.1.7"
category: "Watchlist checkpoint"
tags:
  - watchlist
  - continuity
  - release channels
draft: false
---

This Week-3 Day-1 checkpoint re-checked canonical GitHub and PyPI sources to confirm whether the Week-2 watchlist moved from monitoring into net-new publication signal. Across the tracked set, no new release-channel deltas were confirmed.

Retrieval timestamp (UTC): `2026-04-12T03:49:57Z`.

## What remained unchanged

- LangGraph exact `1.1.7` remained absent on checked GitHub release-by-tag and PyPI exact-version endpoints (`404` on both).
- LangGraph `1.1.7a1` remained visible on GitHub and PyPI.
- CrewAI remained on the same visible track: `1.14.2a2` prerelease activity without a newer non-alpha stable handoff beyond `1.14.1`.
- Semantic Kernel remained anchored at `python-1.41.2` / `1.41.2` in checked channels.
- LangGraph CLI remained at `0.4.21` on the PyPI info endpoint.
- Secondary queue baselines held: Langflow `1.8.4` and Agno `2.5.16` in checked GitHub/PyPI channels.

Because this checkpoint confirms continuity rather than change, this is framed as cadence coverage, not a major release update.

## Evidence

- [LangGraph release by tag `1.1.7` (GitHub API)](https://api.github.com/repos/langchain-ai/langgraph/releases/tags/1.1.7)
- [LangGraph matching refs for `1.1.7` (GitHub API)](https://api.github.com/repos/langchain-ai/langgraph/git/matching-refs/tags/1.1.7)
- [LangGraph exact `1.1.7` (PyPI API)](https://pypi.org/pypi/langgraph/1.1.7/json)
- [LangGraph `1.1.7a1` release page](https://github.com/langchain-ai/langgraph/releases/tag/1.1.7a1)
- [CrewAI recent releases (GitHub API)](https://api.github.com/repos/crewAIInc/crewAI/releases?per_page=8)
- [CrewAI package index (PyPI API)](https://pypi.org/pypi/crewai/json)
- [Semantic Kernel releases (GitHub API)](https://api.github.com/repos/microsoft/semantic-kernel/releases?per_page=8)
- [Semantic Kernel package index (PyPI API)](https://pypi.org/pypi/semantic-kernel/json)
- [LangGraph CLI package index (PyPI API)](https://pypi.org/pypi/langgraph-cli/json)
- [Langflow package index (PyPI API)](https://pypi.org/pypi/langflow/json)
- [Agno package index (PyPI API)](https://pypi.org/pypi/agno/json)

## Explicit non-claims

- This update does not claim feature-level changes beyond cited release/package metadata.
- This update does not claim performance, reliability, or security outcomes.
- This update does not claim roadmap intent or future release timing.
- This update does not claim GA parity between LangGraph `1.1.7a1` and an exact `1.1.7` release.
