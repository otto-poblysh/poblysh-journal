# Poblysh Journal Editorial System

## 0. Agentic Team Operating Model

The editorial system now includes a sub-agent organization under
[`editorial-intelligence/agentic-team/`](/Users/akamaotto/code/latazin-publications/poblysh-journal/editorial-intelligence/agentic-team/).

Use it as the source of truth for:
- who owns each stage
- what each stage must protect
- what artifacts must be produced before handoff
- how issue and article states advance

Key docs:
- [`README.md`](/Users/akamaotto/code/latazin-publications/poblysh-journal/editorial-intelligence/agentic-team/README.md)
- [`workflow-states.md`](/Users/akamaotto/code/latazin-publications/poblysh-journal/editorial-intelligence/agentic-team/workflow-states.md)
- [`handoff-contracts.md`](/Users/akamaotto/code/latazin-publications/poblysh-journal/editorial-intelligence/agentic-team/handoff-contracts.md)
- [`monthly-editorial-workflow.md`](/Users/akamaotto/code/latazin-publications/poblysh-journal/editorial-intelligence/agentic-team/planning/monthly-editorial-workflow.md)
- [`article-workflow.md`](/Users/akamaotto/code/latazin-publications/poblysh-journal/editorial-intelligence/agentic-team/planning/article-workflow.md)
- [`reader-critique-rubric.md`](/Users/akamaotto/code/latazin-publications/poblysh-journal/editorial-intelligence/agentic-team/planning/reader-critique-rubric.md)

The operating principle is simple:
- planning agents first
- writing next
- reader critique before heavy editing
- editing before integrity checks
- sequence planning after text stabilizes
- final QA last

No single agent should define, write, critique, edit, and approve the same
piece alone.

## 1. Create a monthly editorial plan
Create a yearly plan first with `@agent/workflows/create-editorial-plan-for-year.md {Year}`.

Then create a monthly plan with `@agent/workflows/create-editorial-plan-for-month.md {Month - Year}`.

The expected monthly output is:
- 1 issue theme
- 4 essays
- essay titles that fit Poblysh Journal's startup-operator tone
- a clear sequence from tension to consequence to residue
- alignment with the relevant quarter and annual plan
- topic, example, and emotional distribution that fits the full year

Behind the workflow, the role order is:
- `editorial_strategy`
- `issue_planner`
- `essay_architect`
- `reader_perspective_critic`
- `editor_in_chief`

Reference artifacts:
- [`monthly-theme-brief.md`](/Users/akamaotto/code/latazin-publications/poblysh-journal/editorial-intelligence/agentic-team/templates/monthly-theme-brief.md)
- [`issue-map.md`](/Users/akamaotto/code/latazin-publications/poblysh-journal/editorial-intelligence/agentic-team/templates/issue-map.md)
- Example filled brief:
  [`april-2026-monthly-theme-brief.md`](/Users/akamaotto/code/latazin-publications/poblysh-journal/editorial-intelligence/agentic-team/examples/april-2026-monthly-theme-brief.md)

## 2. Create the essays for a month
For `x` in `1` to `4`, use [$ralph-wiggum](/Users/akamaotto/.agents/skills/ralph-wiggum/SKILL.md) to draft one essay at a time.

For each essay:
- use [create-article.md](/Users/akamaotto/code/latazin-publications/poblysh-journal/agent/workflows/create-article.md)
- pull only Piece `{x}` from `content/{year}/{month}/editorial-plan.md`
- finish drafting, QA, and revision before moving to the next piece

Behind the workflow, the role order is:
- `essay_architect`
- `lead_writer`
- `reader_perspective_critic`
- `developmental_editor`
- `style_editor`
- `fact_checker`
- `final_qa`

Reference artifacts:
- [`essay-brief.md`](/Users/akamaotto/code/latazin-publications/poblysh-journal/editorial-intelligence/agentic-team/templates/essay-brief.md)
- [`critique-report.md`](/Users/akamaotto/code/latazin-publications/poblysh-journal/editorial-intelligence/agentic-team/templates/critique-report.md)
- [`edit-report.md`](/Users/akamaotto/code/latazin-publications/poblysh-journal/editorial-intelligence/agentic-team/templates/edit-report.md)
- [`qa-report.md`](/Users/akamaotto/code/latazin-publications/poblysh-journal/editorial-intelligence/agentic-team/templates/qa-report.md)
- Example filled brief:
  [`april-2026-piece-01-essay-brief.md`](/Users/akamaotto/code/latazin-publications/poblysh-journal/editorial-intelligence/agentic-team/examples/april-2026-piece-01-essay-brief.md)

Example:
Create the four essays for `content/2026/april/editorial-plan.md` by looping through Piece `1` to Piece `4` with [$ralph-wiggum](/Users/akamaotto/.agents/skills/ralph-wiggum/SKILL.md), using [create-article.md](/Users/akamaotto/code/latazin-publications/poblysh-journal/agent/workflows/create-article.md).

## 3. Create a latazin page sequence plan
Use [create-latazin-pages-sequence-plan.md](/Users/akamaotto/code/latazin-publications/poblysh-journal/agent/workflows/create-latazin-pages-sequence-plan.md) with the target essay file in `content/{year}/{month}/essays/`.

Owner:
- `latazin_sequence_planner`

Example:
Create a sequence plan for `content/{year}/{month}/essays/01-the-cost-of-private-traction.md` with [create-latazin-pages-sequence-plan.md](/Users/akamaotto/code/latazin-publications/poblysh-journal/agent/workflows/create-latazin-pages-sequence-plan.md). Save the output to `content/{year}/{month}/sequence-plans/01-the-cost-of-private-traction-sequence.md`.

## 4. Canonical content structure
All editorial artifacts now live under:

`content/{year}/{month}/`

Expected month layout:
- `content/{year}/{month}/editorial-plan.md`
- `content/{year}/{month}/essays/`
- `content/{year}/{month}/sequence-plans/`
- `content/{year}/{month}/designs/` when needed

Use lowercase month names such as `april`, `may`, `june`.




