# Content Graph Builder Skill

Build a personal or business content knowledge graph from chats, notes, project files, public content signals, and recurring ideas.

This Skill turns scattered material into a Markdown + `[[wikilink]]` graph that can be used with LLM Wiki, Obsidian, or other wikilink-aware tools.

## What It Does

It helps users:

- create a graph project folder
- normalize raw chats and notes into source summaries
- create wiki nodes with useful links
- find content gaps
- discover surprising connections
- generate weekly graph sync reports
- turn nodes into posts, articles, mini-courses, products, or Skills

## What It Is Not

This is not a traffic-growth tool or viral-copy machine.

It is a workflow for reviewing and connecting your own materials so you can see:

- what you keep talking about
- what has not become a method yet
- what can become a deliverable
- which ideas should be connected
- what to work on next

## Quick Start

Ask:

```text
Use $content-graph-builder to create a content graph from these notes.
```

Or:

```text
Use $content-graph-builder to review this week's notes and update my graph.
```

If no project exists, the Skill creates:

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

## Node Types

- `person`: person, role, account, or audience
- `product`: product, offer, service, or business capability
- `concept`: method, framework, boundary, or judgment
- `platform`: distribution channel or ecosystem
- `asset`: existing content or reusable material
- `gap`: missing piece, blank opportunity, or weak node
- `connection`: surprising cross-domain relationship
- `deliverable`: post, article, course, template, Skill, report, or product
- `source`: raw source summary
- `synthesis`: cross-source conclusion

## Repo Map

- [`SKILL.md`](SKILL.md): main skill instructions
- [`references/wiki-schema.md`](references/wiki-schema.md): node schema and page template
- [`references/sync-workflow.md`](references/sync-workflow.md): source intake, node updates, gap review, weekly sync
- [`references/public-expression.md`](references/public-expression.md): public wording boundaries
- [`examples/sample-project/`](examples/sample-project): small working example
- [`templates/graph-project-template/`](templates/graph-project-template): blank project template

## Attribution

This Skill was inspired by working with LLM Wiki-style Markdown graphs and `[[wikilink]]` knowledge maps. It is designed as a lightweight open workflow, not a replacement for any graph app.

## License

MIT
