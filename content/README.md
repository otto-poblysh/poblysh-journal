# Content Structure

Canonical editorial content now lives under:

`content/{year}/{month}/`

Examples:
- `content/2026/april/editorial-plan.md`
- `content/2026/april/essays/01-the-cost-of-private-traction.md`
- `content/2026/april/sequence-plans/01-the-cost-of-private-traction-sequence.md`

## Expected month layout

- `editorial-plan.md`
- `essays/`
- `sequence-plans/`
- `designs/` when needed

## Naming rules

- Use the calendar year as the first directory level.
- Use lowercase English month names as the second directory level.
- Keep essay filenames slugified and prefixed with their piece number.

## Migration note

The old `content/{month-year}` layout is no longer canonical.
All workflows and docs should assume `content/{year}/{month}`.
