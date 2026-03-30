# Workflow States

Use these exact states across the editorial system.

## Issue States

1. `theme_approved`
2. `issue_map_approved`
3. `essay_brief_approved`
4. `ready_for_drafting`
5. `issue_ready_for_assembly`

## Article States

1. `essay_brief_approved`
2. `drafting`
3. `reader_critique`
4. `developmental_edit`
5. `style_edit`
6. `fact_integrity_review`
7. `sequence_planning`
8. `final_qa`
9. `ready_for_issue_assembly`

## State Rules

- A piece should never skip `reader_critique`.
- A piece should never reach `final_qa` before `fact_integrity_review`.
- `sequence_planning` should only begin when the text is structurally stable.
- `ready_for_issue_assembly` means the text and sequence are both approved.
