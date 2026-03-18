---
task: Draft the four April 2026 Poblysh Journal essays from content/april-2026/editorial-plan.md
completion_criteria:
  - content/april-2026/essays/01-why-the-market-keeps-meeting-an-older-company.md exists and matches Piece 1
  - content/april-2026/essays/02-return-windows-are-judgment-windows.md exists and matches Piece 2
  - content/april-2026/essays/03-narrative-lag-hits-commercial-teams-first.md exists and matches Piece 3
  - content/april-2026/essays/04-silence-keeps-the-old-story-in-the-room.md exists and matches Piece 4
  - Each essay follows the Poblysh voice and create-article workflow constraints
  - Each essay is reviewed for structure, continuity, and markdown cleanliness
max_iterations: 4
---

## Requirements

Loop through Piece 1 to Piece 4 from `content/april-2026/editorial-plan.md`.

For each piece:
- use `.agent/workflows/create-article.md`
- finish drafting, review, and revision before moving to the next piece
- preserve Poblysh Journal tone and operator-native specificity
- preserve continuity inside the April issue and quietly set up the next
  month's systems logic
- let April appear through return, witness, memory, re-entry, and resumed
  judgment rather than explicit calendar labeling
- use subtle Africa-first examples with global contrast and deeper intellectual
  pairings when useful

## Constraints

- No generic startup content
- No beginner PR framing
- No product-led answers
- No bullets in the final essays
- No exclamation marks
- Respect the existing repo worktree and do not touch unrelated changes
