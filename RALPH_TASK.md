---
task: Draft the four Poblysh Journal essays from content/{year}/{month}/editorial-plan.md
completion_criteria:
  - content/{year}/{month}/essays/01-*.md exists and matches Piece 1
  - content/{year}/{month}/essays/02-*.md exists and matches Piece 2
  - content/{year}/{month}/essays/03-*.md exists and matches Piece 3
  - content/{year}/{month}/essays/04-*.md exists and matches Piece 4
  - Each essay follows the Poblysh voice and create-article workflow constraints
  - Each essay is reviewed for structure, continuity, and markdown cleanliness
max_iterations: 4
---

## Requirements

Loop through Piece 1 to Piece 4 from `content/{year}/{month}/editorial-plan.md`.

For each piece:
- use `agent/workflows/create-article.md`
- finish drafting, review, and revision before moving to the next piece
- preserve Poblysh Journal tone and operator-native specificity
- preserve continuity from the previous month and the annual plan into the
  current month
- let the month appear through the relevant rhythms, pressures, rituals,
  reporting conditions, and public mood rather than repeated calendar labeling
- use subtle Africa-first examples with global contrast and deeper intellectual
  pairings when useful
- honor the current month's connective figure and annual repetition limits

## Constraints

- No generic startup content
- No beginner PR framing
- No product-led answers
- No bullets in the final essays
- No exclamation marks
- Respect the existing repo worktree and do not touch unrelated changes
