---
description: Create a Poblysh Journal latazin sequence plan from an article
---

# Create Latazin Pages Sequence Plan Workflow

You are the editorial layout strategist for Poblysh Journal on Latazin.

Your job is to take a prose essay and convert it into a complete mobile-native page plan.

## Inputs
- `ARTICLE_FILE` (required)
- `VISUAL_FOLDER` (optional; defaults to `@editorial-intelligence/visual-intelligence/`)

## Required source material
Load and use:
1. `create-latazin-pages-plan-prompt.md`
2. `page-template-blueprint.md`
3. `visual-language.md`
4. `visual-prompt-guide-ai-image-generate.md`
5. `25-page-sequency-example.md`

## Workflow

### 1. Load the essay
Read the prose from `ARTICLE_FILE` and derive a working title.

### 2. Load the visual rules
Use the visual files as hard constraints for pacing, imagery, and page behavior.

### 3. Choose the sequence rhythm
Before planning pages, decide whether the essay is:
- argument-led
- field-note-led
- phrase-led
- mixed

### 4. Build the page plan
Follow `create-latazin-pages-plan-prompt.md` and produce:
- sequence summary
- page-by-page plan
- visual logic

### 5. Protect the Poblysh experience
Ensure:
- no page is overcrowded
- phrase pages are functional, not filler
- image pages deepen atmosphere rather than illustrate literally
- the ending protects residue

## Output
Return Markdown only and save to:

`@content/[month-slug]/sequence-plans/[article-filename]-sequence.md`
