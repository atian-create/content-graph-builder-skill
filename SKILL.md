---
name: content-graph-builder
description: Build and maintain a personal or business content knowledge graph from chats, notes, project files, public content signals, and recurring ideas. Use when someone wants to turn scattered materials into a Markdown + wikilink graph, find content gaps, discover surprising connections, create weekly graph sync reports, or convert graph nodes into content, courses, products, or skills.
---

# Content Graph Builder

## Purpose

Help a user turn scattered thinking into a usable content graph.

The graph is not a passive archive. It should help answer:

- What are my current content boundaries?
- Which ideas, products, topics, and platforms are connected?
- Which ideas are repeated but not yet structured?
- Which nodes are isolated, overloaded, or missing a next action?
- Which distant nodes create a useful surprising connection?
- What can become a post, article, mini-course, product, Skill, or private archive?

## Best Fit

Use this skill when the user wants to:

- build a personal content brain
- make a knowledge graph from chats and notes
- map business ideas, accounts, products, and content assets
- review weekly content signals
- find content gaps and next actions
- convert a graph node into public content or a product workflow
- create a Markdown wiki that works with LLM Wiki, Obsidian, or other wikilink-aware tools
- create a lightweight visual graph JSON for the included static viewer

## Not For

Do not present this as:

- automated data extraction
- automatic traffic growth
- viral-copy cloning
- guaranteed content strategy

Use language like:

- content graph
- public content signals
- review
- judgment
- workflow
- content brain
- knowledge map
- surprising connections
- content gaps

## Default Project Shape

If the user has no existing project, create this shape:

```text
content-graph-project/
├── README.md
├── purpose.md
├── schema.md
├── raw/
│   └── sources/
└── wiki/
    ├── index.md
    ├── overview.md
    └── log.md
```

If the user asks for a visual graph, also create:

```text
graph-data.json
```

Use the JSON shape in `references/visual-viewer.md` so it can be imported into `viewer/graph-viewer.html`.

## Workflow

1. Inspect the user's current context and files. Do not infer private facts that are not present in provided or local materials.
2. Define graph purpose: content planning, business strategy, creator workflow, learning map, project map, or weekly review.
3. Normalize source material into short source summaries under `raw/sources/`.
4. Create or update wiki pages with frontmatter and `[[wikilink]]` links.
5. Classify nodes with stable types: `person`, `product`, `concept`, `platform`, `asset`, `gap`, `connection`, `deliverable`, `source`, `synthesis`.
6. Update `wiki/index.md`, `wiki/overview.md`, and `wiki/log.md`.
7. Produce at least one of:
   - content gap
   - surprising connection
   - deliverable recommendation
   - weekly sync report
8. If a visual graph is requested, export a viewer-ready JSON file with sanitized node labels, short descriptions, edge types, and next actions.

## Node Quality Bar

Every important node should include:

- core judgment
- connected nodes
- what it can become
- next action

Prefer updating existing pages over creating duplicate concepts.

## Weekly Sync

A useful weekly sync should name:

- new source signals
- node changes
- content boundary shifts
- content gaps
- surprising connections
- deliverables to create next

## Output Contract

When building a graph project, output:

```markdown
## Project Created
- path:
- graph purpose:
- source files used:

## Nodes Added Or Updated
- ...

## Content Gaps
- ...

## Surprising Connections
- ...

## Next Deliverables
- ...
```

## References

- `references/wiki-schema.md`
- `references/sync-workflow.md`
- `references/public-expression.md`
- `references/visual-viewer.md`
- `examples/sample-project/`
- `examples/sample-viewer-data.json`
- `templates/graph-project-template/`
- `viewer/graph-viewer.html`

## Public Sharing Boundary

When preparing a graph for public sharing, publish the reusable workflow and sample data, not private archives.

Remove:

- private file paths
- thread IDs
- unpublished client, business, or personal details
- raw diary or relationship material
- internal delegation notes
- claims about guaranteed growth, traffic, or viral outcomes
