---
description: Create a detailed Poblysh Journal monthly editorial plan from a monthly theme
---

# Create Monthly Editorial Plan Workflow

You are the editorial strategist for Poblysh Journal.

Your job is to turn one monthly theme into a detailed, publication-ready plan for a four-essay issue.

## Inputs
- `MONTH_NAME` (required)
- `YEAR` (optional)
- `CURRENT_YEAR_PLAN_PATH` (optional; strongly recommended when a year plan exists)
- `EDITORIAL_THEME` (optional; if supplied, validate it against the month)
- `THEME_GOAL` (optional; if omitted, derive it from the chosen theme)
- `SEASONAL_OR_EVENT_CONTEXT` (optional)
- `PREVIOUS_MONTH_THEME` (optional)
- `PREVIOUS_MONTH_ARTICLES` (optional)
- `PREVIOUS_ISSUE_PATH` (optional)
- `EXTERNAL_EVENT_SCAN_SCOPE` (optional; defaults to startup subculture for the target month)
- `GEOGRAPHIC_EXAMPLE_PRIORITY` (optional; default `Africa-first, then global`)
- `INTELLIGENCE_FOLDER` (optional; defaults to `/editorial-intelligence/`)
- `TARGET_PIECE_COUNT` (optional; default `4`)
- `PRIORITY_PILLARS` (optional)
- `MUST_INCLUDE` (optional)
- `MUST_AVOID` (optional)

## Required source material
Load and use:
1. `editorial-plan.md`
2. `house-voice.md`
3. `house-metaphors.md`
4. `quality-rubric.md`
5. `style-guide.md`
6. `notes/essay-types.md`
7. `notes/intellectualization-engine.md`
8. `notes/principles-of-taste-forward-articles.md`
9. `agentic-team/README.md`
10. `agentic-team/workflow-states.md`
11. `agentic-team/handoff-contracts.md`
12. `agentic-team/planning/monthly-editorial-workflow.md`
13. `agentic-team/planning/reader-critique-rubric.md`
14. `agentic-team/agents/editorial-strategy.md`
15. `agentic-team/agents/issue-planner.md`
16. `agentic-team/agents/essay-architect.md`
17. `agentic-team/agents/reader-perspective-critic.md`
18. `agentic-team/agents/editor-in-chief.md`

When available, also load:
- the current year's annual editorial plan from `CURRENT_YEAR_PLAN_PATH`
- the previous year's annual editorial plan

## Planning context

Poblysh Journal is a thought-led editorial publication for founders, CMOs, PMMs, and strategic operators who care about visibility, perception, timing, and public meaning.

The plan should feel:
- editorial
- strategic
- coherent across the month
- recognizably Poblysh
- emotionally sequenced rather than emotionally flat

## Workflow

### 0. Load annual and quarter constraints
If `CURRENT_YEAR_PLAN_PATH` is available, extract and obey:
- the year thesis and annual reader transformation goal
- the relevant quarter theme and this month's role inside that quarter
- the annual core topic inventory, including underused and overused topics
- year-level emotional strategy and any emotional register already overused in
  recent months
- annual example governance, including:
  - African example floor
  - company repetition budget
  - sector mix rule
  - geography mix rule
  - public-surface mix
  - year cliché blacklist
  - example ledger constraints
- monthly planner handoff rules from the annual plan

If no annual plan is available:
- infer quarter logic from the year and month
- but note that topic, example, and emotional distribution will be less
  governed and should be marked as lower-confidence

### 1. Build the calendar-month context
Research the target month in the calendar year before locking the theme.

You must:
- identify the deeper rhythms, pressures, rituals, moods, and interpretive tensions that make the month distinct
- prioritize African social, cultural, political, economic, and religious contexts when they meaningfully shape how founders or operators might experience the month
- widen the scan to global contexts so the month does not become provincially framed
- treat startup subculture as one layer of the month, not the whole of it
- use the month as an interpretive atmosphere, not as a list of named events

Good context categories include:
- religious periods, fasting seasons, feasts, mourning periods, and renewal rituals
- quarter transitions, year-openings, year-end closures, budget resets, hiring waves, and reporting cycles
- public commemorations, elections, civic anniversaries, deaths, births, and historical echoes
- school calendars, migration periods, travel windows, holiday returns, and family obligations
- weather, harvest, fiscal, or cultural rhythms that change how attention and seriousness behave
- startup-specific windows only when they reveal a larger pressure rather than acting as calendar filler

Named conferences, cities, and startup gatherings are optional, not mandatory.
Use them only when they genuinely change the meaning of the month. Do not let
the month become a travel itinerary.

Do not force shallow seasonality. Do not build the month around tech-event
name-dropping. Build around the interpretive pressures that would still matter
even if no conference existed.

### 2. Interpret or select the theme
Determine:
- whether the supplied theme genuinely fits the current month context
- whether it fits the quarter theme and the year thesis
- if no theme is supplied, derive one from the month context and Poblysh pillars
- the central tension
- why it matters now
- whether the calendar frame is load-bearing or merely atmospheric
- the durable core of the argument that would still matter outside this month
- the seasonal edge that this month makes sharper
- which Poblysh pillars it best serves
- how it connects to any prior month context
- how it continues the publication's ongoing conversation rather than starting fresh
- which annual core topics this month should advance because they are
  under-covered, strategically due for revisit, or quarter-relevant
- which overused topics should be backgrounded this month so the year does not
  collapse into a few favorite arguments

If a supplied theme does not fit the month's deeper interpretive context, refine
it.

Agent ownership:
- `editorial_strategy` owns theme formation and no-go zones
- `editor_in_chief` approves the monthly direction

### 3. Design the issue shape
Default monthly shape:
- essay 1: opening tension
- essay 2: widening interpretation
- essay 3: applied business consequence
- essay 4: closing reframe or residue piece

Emotional sequencing rule:
- do not let all four essays sit in the same register of cool intelligence
- the month should move through an intentional emotional cadence, even when the
  prose stays composed
- default emotional shape:
  - essay 1 should create recognition, unease, surprise, or sharpened curiosity
  - essay 2 should deepen the feeling with wonder, pattern-recognition, or a
    harder interpretive pressure
  - essay 3 should convert the theme into consequence, urgency, or exposed cost
  - essay 4 should leave residue: reflection, sober ambition, haunted clarity,
    or another feeling that survives after reading
- you may vary this default, but only if the alternative cadence is explicit

### 3a. Design the month's emotional cadence
Before finalizing the issue shape, define how the month will make the target
reader feel across all four essays.

For the month overall, specify:
- the dominant emotional thesis of the issue
- the 2 to 4 emotional registers the month will move through
- which emotional note is intentionally withheld until later in the month
- which emotional excess to avoid across the issue: monotone alarm, monotone
  coolness, decorative wonder, or another flattening habit
- the business activation goal for the month: what kind of internal
  conversation, decision, or re-evaluation the full issue should provoke

For each piece, define:
- `PRIMARY EMOTIONAL EFFECT`: the main feeling the piece should leave behind
- `SECONDARY EMOTIONAL UNDERTONE`: the quieter note under the main feeling
- `BUSINESS ACTIVATION GOAL`: what the reader should want to question, discuss,
  revisit, or act on after reading
- `MEMORY SURFACE`: the kind of line, scene, reversal, or cost that should stay
  in mind after the essay ends

Distribution rules:
- at least three distinct primary emotional effects should appear across a
  four-piece month unless the month is explicitly designed as a single-note
  pressure issue
- no two adjacent pieces should have identical primary emotional effects unless
  the repetition is the point and is named as such
- the issue should not peak emotionally in essay 1 and then explain itself for
  the rest of the month
- emotion must arise from business truth, interpretive pressure, and felt
  stakes, not from melodrama or decorative intensity
- if the annual plan marks a recent emotional register as overused, bias this
  month away from repeating it in the same way

### 4. Choose the essay actions
Use `notes/essay-types.md` to vary the monthly set without losing coherence.

Agent ownership:
- `issue_planner` owns monthly sequence logic
- `essay_architect` owns per-piece framing

### 5. Build the issue sequence as a continuing conversation
Make sure the month feels curated rather than random.

Each piece should:
- inherit a tension, phrase, or unresolved question from the piece before it
- subtly reference prior month themes or earlier Poblysh concerns when useful
- feel like it is continuing an existing conversation, not launching an isolated essay

The issue should contain a visible narrative bridge:
- from the previous month into this month
- from piece 1 into piece 2
- from piece 2 into piece 3
- from piece 3 into piece 4

Before finalizing the issue plan, run a reader hook test:
- would the target reader stop for each title
- is the opening promise of each piece strong enough
- does each piece sound worth sustained reading

Agent ownership:
- `reader_perspective_critic` owns pre-draft hook testing
- `editor_in_chief` gives final approval on theme, sequence, and essay tensions

### 6. Assign visual rhythm
For each essay, name:
- dominant mood
- likely sequence style: argument-led, field-note-led, phrase-led, or mixed
- likely visual ground emphasis: light monochrome, mid monochrome, or dark monochrome

### 7. Plan the example logic
For the month overall and for each piece:
- prefer passive, subtle mentions of real companies, founders, publications, or startup situations
- prioritize African examples when they are relevant and strong
- complement them with global examples where contrast sharpens the argument
- where useful, pair startup examples with non-startup reference points such as
  writers, clergy, artists, historians, philosophers, political moments, or
  public rituals that deepen the theme
- use geography as perspective, not as tourism; a company may be American while
  the interpretive counterpart may come from Nigeria, Kenya, South Africa, or
  elsewhere
- avoid loud case-study blocks, listicles, city-dropping, or namedrop-heavy writing
- ensure examples feel intellectually woven into the essay logic rather than bolted on
- choose examples for interpretive fit, not prestige; the best example is often
  the quieter, lower-glamour signal that proves the mechanism more exactly
- do not default to funding rounds, launches, or big-brand moments when a
  sponsorship, update log, partnership thread, recurring ritual, maintenance
  surface, policy page, support artifact, or stewardship behavior would make
  the argument cleaner
- vary signal classes across the month so the issue does not feel like four
  essays drawing from the same obvious pool of startup proof
- decide in advance what each piece's examples must *do*, not just what sectors
  or geographies they should come from
- for universal arguments, plan examples that preserve universality; do not let
  example choice accidentally force a narrower company type unless the piece is
  explicitly designed around that subset
- when a piece depends on public form, trust surfaces, or institutional
  legibility, prefer examples that expose those surfaces directly: security
  portals, safety pages, support artifacts, policy language, dated evidence,
  procurement surfaces, update logs, and other inspectable forms
- identify any prestige traps for the month: example types that look impressive
  but would weaken the argument by making the piece louder, flatter, or more
  familiar than it should be
- if the month pairs African and global examples, ask whether the issue should
  surface an asymmetry in documentation, institutional scaffolding, or public
  proof burden rather than treating the examples as equivalent by default
- every essay must have at least one African example, company, operator,
  publication, institution, or public surface; this is a floor, not an
  optional preference
- if an annual example ledger is available, do not reuse companies, sectors,
  or example classes in ways that violate the year plan's repetition budget or
  variety rules
- prefer month-level example choices that repair year-level imbalance rather
  than month-level convenience

Reference quality rule:
- the best examples do not merely show where something happened
- they reveal how one domain can clarify another
- they should feel like thematic rhyme, not database retrieval

### 7a. Assign Per-Piece Example Burden

Before finalizing the issue plan, define the example logic for each piece
explicitly. This forces the planner to choose example *types* upstream instead
of leaving all example quality decisions to the article workflow.

For each essay, specify:

**EXAMPLE BURDEN**
What the opening example must prove. This should be a mechanism, not a topic.

Examples:
- "show continuity surviving without spectacle"
- "show older signals being reread as judgment"
- "show stewardship through an unglamorous maintenance surface"
- "show that the visible test arrives after the real preparation window"

**PREFERRED SIGNAL CLASS**
What kind of public surface should do the work best for this piece.

Examples:
- sponsorship or partnership thread
- feature retirement or update log
- recurring ritual or tournament
- hiring move or staffing signal
- support artifact, pricing page, or policy page
- funding round, acquisition, or launch only if the essay genuinely needs scale

**PRESTIGE TRAP TO AVOID**
Name the louder example class most likely to flatten the argument if chosen by
default.

Examples:
- "do not default to a funding round"
- "avoid celebrity founder quotes"
- "avoid conference-stage examples unless the piece is about spectacle itself"

**OPENING EXAMPLE JOB**
What the first example should make the reader feel or notice before the thesis
fully arrives.

**CONTRAST EXAMPLE JOB**
What kind of structurally different example should complicate the claim later in
the essay.

**RETURN REVEAL**
What the opening example should mean by the time it returns near the end. The
late return should reveal more than the opening, not merely defend the example
against a weaker reading.

**PUBLIC SURFACE CLASS** (optional but strongly recommended)
If the piece is about legibility, trust, seriousness, or institutional form,
name the exact kind of surface most likely to prove it.

Examples:
- security portal
- support center and dated changelog
- safety page or compliance surface
- procurement artifact
- community ritual or stewardship ritual
- privacy or policy language

**PRIMARY READER ENCOUNTER**
Name who is most likely to read the proof surface first: buyer, partner,
regulator, journalist, prospective hire, operator, investor, or community
stakeholder.

**SCOPE NOTE**
Whether the piece is universal or intentionally scoped to a subset such as
community-facing companies, infra companies, or post-raise startups. If scoped,
say so here so the narrowing is earned later.

**WHY THIS MONTH IS LOAD-BEARING**
One sentence on why this piece belongs specifically in this month rather than
merely sounding plausible here.

**DURABLE CORE / SEASONAL EDGE**
One sentence on what remains true in any month, and one sentence on what this
month makes sharper.

**HARDEST IMPLICATION**
The uncomfortable corollary the eventual draft should be able to reach if the
argument earns it.

### 7b. Design the Month's Anecdote Constellation

Before finalizing the issue plan, establish a constrained example universe 
for the month. This is not a list of examples to be used — it is a set of 
boundaries and threads that guide the example researcher across all four 
pieces, so that a reader who follows the full issue encounters a coherent 
world of reference rather than four unrelated case pools.

Define the following:

**ANCHOR DOMAIN**
One industry, geography, era, or company type that will appear across at 
least two pieces — not as repeated mention, but as a recurring interpretive 
ground. The reader should feel that the month is partly *about* this domain, 
even if it is never named as such.

Example: "early-stage African fintech in a post-raise quiet period" or 
"founder-led B2B companies navigating a first institutional investor."

**CONNECTIVE FIGURE OR MOMENT** (optional but recommended)
One real company, founder, publication, or historical moment that can 
appear in at least two pieces at different depths — once as the opening 
scene, once as a passing reference, once as a closing echo. The reader 
who notices the second appearance should feel rewarded, not manipulated.
IMPORTANT: Check previous months' plans to verify we are not reusing the same company across too many months. Anchor companies and connective figures must change from month to month to avoid the appearance of patronage.

**CONTRAST POLE**
One domain, geography, or type of company that will serve as the contrast 
reference across the month. It should be structurally different from the 
anchor domain — different scale, different market, different operating 
condition — so that the contrast earns its presence each time rather than 
feeling like geographic box-ticking.

Example: if the anchor is African fintech, the contrast pole might be 
late-stage Western SaaS at full documentation maturity.

**CLICHÉ BLACKLIST FOR THE MONTH**
Examples that are banned across all four pieces this month. Carry forward 
any entries from the previous month's blacklist unless explicitly retired.

**THREAD TO LEAVE OPEN**
One question, company situation, or interpretive tension that the month's 
essays will approach but not resolve — so that a reader finishes the issue 
with something still working in their mind, and a reason to keep watching 
the space the essays pointed at.

Agent ownership:
- `editorial_strategy` proposes the constellation
- `editor_in_chief` approves it before issue planning is finalized
- the constellation is passed as a constraint to `example-researcher.md` 
  in every article workflow run this month

## Output structure

# [Month Name] Editorial Plan

## Theme
[theme]

## Annual Alignment
[paragraph]

## Quarter Theme
[paragraph]

## Month Role In Quarter
[paragraph]

## Goal
[goal]

## Durable Core / Seasonal Edge
[paragraph]

## Why This Month Works
[paragraph]

## Current Month Context
[paragraph]

## Narrative Bridge from Last Month
[paragraph or "Not applicable"]

## Dominant Editorial Pillars
- [pillar]
- [pillar]
- [pillar]

## Core Topics Advanced This Month
- [topic]
- [topic]
- [topic]

## Topics Intentionally Backgrounded This Month
- [topic]
- [topic]

## Editorial Rhythm
[paragraph]

## Emotional Arc

**Dominant Emotional Thesis:** [one sentence]  
**Month Emotional Progression:** [one short paragraph on how the feeling moves
from essay 1 through essay 4]  
**Withheld Emotional Note:** [one sentence]  
**Emotional Excess To Avoid:** [one sentence]  
**Month Business Activation Goal:** [one sentence]

## Anecdote Constellation

**Anchor Domain:** [one sentence]  
**Connective Figure or Moment:** [name + one sentence on how it travels]  
**Contrast Pole:** [one sentence]  
**Month Cliché Blacklist:** [list]  
**Thread to Leave Open:** [one sentence]

Usage note: pass these five fields as constraints to the example researcher 
at the start of every article workflow this month. Do not allow individual 
pieces to source examples independently of this constellation.

## Month-Level Example Strategy

- **Signal-Class Mix:** [what kinds of public surfaces the month should draw
  from across the four pieces]
- **Low-Glamour Advantage:** [where quieter examples are likely to outperform
  more prestigious ones this month]
- **Prestige Traps to Avoid:** [month-wide list]
- **Calendar Load-Bearing Rule:** [when month references are truly earned this
  month and when they should stay atmospheric only]
- **Institutional Surface Bias:** [which trust, seriousness, or stewardship
  surfaces should be favored if relevant]
- **Market Asymmetry to Surface:** [if African and global examples are paired,
  what structural difference in proof burden or documentation should be named]
- **Example Selection Principle:** [one sentence on how examples should be
  chosen this month]
- **African Example Floor:** [one sentence on how every essay will satisfy it]
- **Annual Repetition Constraint:** [one sentence on how this month avoids
  overusing companies, sectors, or example classes already saturated this year]

## Piece List

For each piece include:
1. Title
2. Essay Type
3. Editorial Pillar
4. Purpose in the Month
5. Primary Visual Direction
6. Quarter Role
7. Core Topics Advanced
8. Primary Emotional Effect
9. Secondary Emotional Undertone
10. Business Activation Goal
11. Memory Surface
12. Core Tension
13. Why it belongs in this month
14. Conversation Link
15. Example Direction
16. Example Burden
17. Preferred Signal Class
18. Prestige Trap to Avoid
19. Opening Example Job
20. Contrast Example Job
21. Return Reveal
22. Public Surface Class
23. Primary Reader Encounter
24. African Example Direction
25. Scope Note
26. Why This Month Is Load-Bearing
27. Durable Core / Seasonal Edge
28. Hardest Implication

## Month-Level And Year-Level Balance Check
[brief confirmation]
