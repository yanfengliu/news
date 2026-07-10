---
name: multi-cli-review
description: Use when running the multi-CLI (Codex + Claude) adversarial code review on high-risk changes or full-codebase audits — routes to the fleet-canonical runbook (pins, commands, output extraction, failure modes) plus news-specific notes.
---

# Multi-CLI review — news stub

**Read the fleet-canonical runbook now:** `../loop-ops/docs/skills/multi-cli-review.md` — current review model pins (the fleet's single bump site), exact CLI commands, `-o` output extraction, Windows gotchas, and failure modes. Do not act from memory of an older per-repo copy of this skill.

news-specific notes:

- Reviewer pin sites in scripts: NONE (verified 2026-07-10 — repo is pre-code: no `package.json`, `src/`, or scripts are tracked; re-grep for hard-coded reviewer models when the first scripts land).
- Review capture files use the canonical default `tmp/review-runs/<objective>/<date>/<iteration_number>/` (never staged, cleaned up after synthesis) — no repo override; AGENTS.md → Team of subagents documents the same convention.
