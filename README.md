# Stock Lens Analyzer Starter

Starter repo for maintaining a multi-lens ChatGPT Skill focused on Atlas + TradingView chart analysis.

## Purpose

This repo is the source-of-truth for:

- the installed ChatGPT skill
- lens definitions and scoring rubrics
- output contracts
- regression test cases
- future roadmap and changes

## Suggested workflow

1. Edit the docs in `specs/` and `references/`
2. Keep `SKILL.md` concise and use it as the dispatcher
3. Test changes against examples in `test-cases/`
4. Package the skill as `skill.zip` when you want to reinstall/update it in ChatGPT

## Folder guide

- `SKILL.md` — primary skill entrypoint
- `agents/openai.yaml` — UI metadata
- `references/` — stable supporting docs
- `specs/` — one spec per lens or scoring concern
- `test-cases/` — prompts and expected behavior for regression testing
- `templates/` — reusable output shapes
- `.github/workflows/` — optional CI checks

## Recommended iteration loop

- Add a chart/test case whenever the skill makes a bad call
- Update the lens spec, not just the prompt
- Note scoring changes in `CHANGELOG.md`
- Repackage and reinstall after meaningful revisions
