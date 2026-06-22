# Wiki Schema Reference

Use Markdown files and `[[wikilink]]` links.

## Page Types

- `person`
- `product`
- `concept`
- `platform`
- `asset`
- `gap`
- `connection`
- `deliverable`
- `source`
- `synthesis`

## Page Template

```markdown
---
type:
title:
created:
updated:
sources:
related:
status:
---

## Core Judgment

## Connects To

## Can Become

## Next Step
```

## Rules

- Keep node names stable.
- Prefer updating existing pages over creating near-duplicates.
- Use `[[wikilink]]` links for every important relationship.
- Mark weak claims as hypotheses.
- Every important node should have a next action.
- If a source contains many ideas, summarize it first, then split durable concepts into their own pages.
