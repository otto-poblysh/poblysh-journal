# Poblysh Journal Editorial System

## 1. Create a monthly editorial plan
Create a monthly plan with `@.agent/workflows/create-editorial-plan-for-month.md {Month - Year}`.

The expected monthly output is:
- 1 issue theme
- 4 essays
- essay titles that fit Poblysh Journal's startup-operator tone
- a clear sequence from tension to consequence to residue

## 2. Create the essays for a month
For `x` in `1` to `4`, use [$ralph-wiggum](/Users/akamaotto/.agents/skills/ralph-wiggum/SKILL.md) to draft one essay at a time.

For each essay:
- use [create-article.md](.agent/workflows/create-article.md)
- pull only Piece `{x}` from `content/<month-slug>/editorial-plan.md`
- finish drafting, QA, and revision before moving to the next piece

Example:
Create the four essays for `content/<month-slug>/editorial-plan.md` by looping through Piece `1` to Piece `4` with [$ralph-wiggum](/Users/akamaotto/.agents/skills/ralph-wiggum/SKILL.md), using [create-article.md](.agent/workflows/create-article.md).

## 3. Create a latazin page sequence plan
Use [create-latazin-pages-sequence-plan.md](.agent/workflows/create-latazin-pages-sequence-plan.md) with the target essay file in `content/<month-slug>/essays/`.

Example:
Create a sequence plan for `content/<month-slug>/essays/01-the-cost-of-private-traction.md` with [create-latazin-pages-sequence-plan.md](.agent/workflows/create-latazin-pages-sequence-plan.md). Save the output to `content/<month-slug>/sequence-plans/01-the-cost-of-private-traction-sequence.md`.

Create a sequence plan for `content/<month-slug>/essays/02-why-funding-is-easier-to-cover-than-progress.md` with [create-latazin-pages-sequence-plan.md](.agent/workflows/create-latazin-pages-sequence-plan.md). Save the output to `content/<month-slug>/sequence-plans/02-why-funding-is-easier-to-cover-than-progress-sequence.md`.
