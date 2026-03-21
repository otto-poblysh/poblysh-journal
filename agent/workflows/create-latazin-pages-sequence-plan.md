---
description: Create a Poblysh Journal latazin sequence plan from an article
---

# Create Latazin Pages Sequence Plan Workflow

You are the editorial layout strategist for **Poblysh Journal**, published on
the **Latazin** platform.

Your job is to take a prose essay and convert it into a complete
**Latazin Page Plan** for a mobile-native editorial story.

## Inputs

- `ARTICLE_FILE` (required, for example
  `@content/2026/april/essays/01-the-cost-of-private-traction.md`)
- `VISUAL_FOLDER` (optional; defaults to
  `@editorial-intelligence/visual-intelligence/`)

## Required source material

Load and use these files from `VISUAL_FOLDER` or
`@editorial-intelligence/visual-intelligence/` by default:

1. `create-latazin-pages-plan-prompt.md`
2. `page-template-blueprint.md`
3. `visual-language.md`
4. `visual-prompt-guide-ai-image-generate.md`
5. `25-page-sequency-example.md`

If any file is missing, rely on the available Poblysh Journal visual rules
rather than inventing a new system.

## Workflow Steps

### 1. Load the Content

Read the prose from `ARTICLE_FILE`.

Treat the prose as the `RAW_PROSE` input required by
`create-latazin-pages-plan-prompt.md`.

Use the filename or internal headings to determine the `WORKING_TITLE`.

### 2. Load the Visual Rules

Review:

- the structural rules in `page-template-blueprint.md`
- the aesthetic rules in `visual-language.md`
- the image direction rules in `visual-prompt-guide-ai-image-generate.md`

Use `25-page-sequency-example.md` as a quality reference for pacing, page
detail, extraction notes, and output depth.

### 3. Build a Background Rhythm Plan Before Sequencing

Before executing the core sequence-plan prompt, derive a **background rhythm
plan** for the full story using the visual-language rules.

Use Poblysh's monochrome editorial spectrum intentionally. Group it into three
working grounds for planning:

- `Light Monochrome`
  Paper white, bone, soft ash
- `Mid Monochrome`
  Light slate, iron
- `Dark Monochrome`
  Charcoal, near-black, true black

Page-level balancing rules:

- Do **not** let light monochrome become the passive default for nearly every
  page.
- `Light Monochrome` should mainly hold calm reading pages, reflective essay
  pages, and quieter threshold or residue moments.
- `Mid Monochrome` should carry object studies, bridge pages, late-middle
  tension, and pages that need more editorial density without full severity.
- `Dark Monochrome` should carry openings, closings, statement hinges,
  gravitas-heavy transitions, and the most severe image-led pauses.

Sequence-level balancing rules:

- For a standard **25-page** plan, aim for a near-even spread, usually in the
  range of:
  - `Light Monochrome`: 8 to 10 pages
  - `Mid Monochrome`: 7 to 9 pages
  - `Dark Monochrome`: 6 to 8 pages
- For any chosen page count between 20 and 30, keep the three grounds as evenly
  distributed as the prose allows.
- No ground should exceed roughly **40%** of the sequence unless the essay
  clearly demands it.
- Avoid more than **3 consecutive pages** on the same ground.
- Avoid more than **2 consecutive Light Monochrome pages** when another ground
  can do the job just as well.
- Each 5-page stretch should contain at least **2 different grounds**.

This background rhythm plan is a hard planning constraint when assigning page
families and pacing.

### 4. Execute the Sequence Plan Prompt

Execute the instructions found in `create-latazin-pages-plan-prompt.md` using
the loaded `RAW_PROSE` and `WORKING_TITLE`.

Follow all steps in that prompt, including:

- diagnosing the piece
- extracting page-bearing units
- choosing the right page count, default 25
- building the sequence logic
- assigning correct page families
- adding image directions that conform closely to
  `visual-prompt-guide-ai-image-generate.md`
- ensuring every essay page carries two to three paragraphs so the reading
  experience feels like a genuine essay rather than an Instagram carousel; a
  single-paragraph essay page is only acceptable when it also carries a
  subheading introduction or the paragraph itself is unusually long and
  structurally dense
- applying the background rhythm plan so the sequence visibly balances
  `Light Monochrome`, `Mid Monochrome`, and `Dark Monochrome`
- explicitly naming the chosen ground inside each page's `Design Notes`
- explicitly naming typography inside `Design Notes` for every page with visible
  text
- listing typography by text role when a page contains more than one role, such
  as title, subheading, body, statement, overlay, or caption
- always specifying at minimum the font face, weight, size, and line height
- summarizing the overall ground distribution in the `Page Strategy Summary` or
  `Extraction and Editing Notes`

### 5. Output Rules

Return the answer in Markdown only.

The output must feel closer to the Sterling-quality example than to a skeletal
outline. That means it should include:

- article metadata
- page strategy summary
- extraction and editing notes
- a fully detailed page plan
- page-type balance check
- a closing note on why the sequence works

Typography instruction for all generated sequence plans:

- If `Text:` is not `None`, `Design Notes` must include a `Typography:`
  sentence.
- Use Poblysh Journal house typography values drawn from `visual-language.md`.
- Format the note with exact roles and specs, for example:
  - `Typography: Statement in Lato Medium 24/30.`
  - `Typography: Subheading in Lato Medium 18/24; body copy in Lato Regular 18/26.`
  - `Typography: Title in Merriweather Bold 32/38; supporting line in Lato Medium 18/24.`

Return the final output into a new file located at:

`@content/[year]/[month]/sequence-plans/[article-filename]-sequence.md`

For example, if the input is
`content/2026/april/essays/01-the-cost-of-private-traction.md`, the output
should be saved to
`content/2026/april/sequence-plans/01-the-cost-of-private-traction-sequence.md`.
