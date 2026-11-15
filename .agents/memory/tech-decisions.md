---
type: project
created: 2026-07-18
updated: 2026-11-16
---

# Technical Decisions

- Component metadata uses SemVer while the toolkit release keeps CalVer.
- `manifest.json` and `manifest.lock.json` must remain synchronized with component frontmatter.
- Antigravity 2.0 runtime migration: Legacy static workflows (`.agents/workflows/*.md`) are fully converted to on-demand skills (`.agents/skills/<name>/SKILL.md`) with native `/<name>` chat autocomplete support.
- All 20 specialist agents and 60 skills use standardized Antigravity 2.0 runtime tools: `read_file`, `edit_file`, `write_file`, `run_command`, `invoke_subagent`, `swarm`.
- Fork origin repository is `https://github.com/thanh-nguyennam/ag-kit.git`.
- Project documentation, internal review plans, and migration notes are stored in `ag-kit-doc/` (kept private via `.gitignore`).
- Feature branch workflow: Development, skill reviews, and refactorings must be pushed to dedicated feature branches first, and merged into `main` in a single consolidated step upon full verification.
