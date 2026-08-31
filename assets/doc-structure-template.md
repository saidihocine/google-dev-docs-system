# Documentation Structure Template

Use this skeleton when creating or restructuring product or feature documentation in the Google style.

## Product / Feature Documentation Skeleton

```
product-or-feature/
├── overview.md              # Required. Orients and routes.
├── concepts/
│   ├── overview.md          # Mental model and core ideas
│   └── key-concepts.md      # Deeper conceptual pages as needed
├── get-started/             # or quickstart/
│   └── quickstart.md        # Shortest path to first success
├── guides/                  # or how-to/
│   ├── common-task-1.md
│   ├── common-task-2.md
│   └── ...
├── reference/
│   ├── overview.md
│   └── ...                  # API reference, CLI, config, etc.
├── samples/
│   └── ...
└── resources/               # optional: pricing, quotas, support, etc.
```

## Single Page Template (Guide or Concepts)

```markdown
# Title in sentence case

One-paragraph orientation. What this page is for and who it helps.

## Before you begin
Prerequisites, permissions, setup.

## Main content sections
Clear H2/H3 hierarchy.
Prefer numbered lists for procedures.
Prefer short paragraphs and concrete examples.

## What's next
Links to the logical next pages or related tasks.
```

## Reference Page Notes
- Start with a short description of the resource or method.
- Include a minimal code sample near the top when useful.
- Document every parameter, field, and return value.
- Use present tense.
- Link related resources and methods.

## Voice Checklist (apply to every page)
- [ ] Second person ("you")
- [ ] Active voice
- [ ] Sentence case headings
- [ ] Descriptive links
- [ ] Conditions before instructions
- [ ] No pre-announcements
- [ ] Accessible and globally readable
