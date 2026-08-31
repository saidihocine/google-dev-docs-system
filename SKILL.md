---
name: google-dev-docs-system
description: Use when analyzing, writing, reviewing, reverse-engineering, or improving Google Developers documentation, Google Cloud API design, AIP principles, Style Guide compliance, or any developer docs that must follow Google's developer experience philosophy — resource-oriented design, consistency across products, progressive disclosure, second-person active voice, and clarity for a global audience. Triggers include Google docs, AIP, developers.google.com, Cloud API design, documentation system, reverse engineer Google docs, Google style guide.
---

# Google Dev Docs System

This skill encodes the operating system behind Google Developers documentation. It forces the agent to think, structure, and write like the Google documentation system itself — not just copy its surface style.

## Core Philosophy (Non-negotiable)

Google documentation is a **product**, not a byproduct. Its goal is to make the developer succeed with the least friction possible, using the same mental model across every Google product.

Key axioms:
- Consistency beats cleverness.
- The developer who learned one Google API must understand the next one immediately.
- Documentation is part of the API surface.
- Progressive disclosure is mandatory.
- Clarity and accessibility for a global audience override local preferences.
- Break any rule if following it would produce worse content (Orwell principle).

## When Activated

1. **Analyze first** — Map the content or request against the system layers below before writing or criticizing.
2. **Enforce the Mental Model** — Prefer resource-oriented design and standard patterns over ad-hoc structures.
3. **Apply Progressive Disclosure** — Always structure content as Overview → Concepts → Guides/How-to → Reference → Samples.
4. **Adopt the Voice** — Second person ("you"), active voice, conversational but professional, present tense for API behavior.
5. **Check Consistency** — Does this look and feel like other Google docs? Does it follow AIP patterns where applicable?
6. **Optimize for the Global Developer** — Short sentences, descriptive links, accessibility, no unnecessary jargon.

## System Layers (Reverse-Engineered Structure)

Treat every documentation task through these layers:

### Concepts
- Resource-oriented design (everything is a resource)
- Standard methods (Get, List, Create, Update, Delete)
- Resource names (`projects/{project}/...`)
- Progressive disclosure
- Documentation as product
- Machine-readable + human-readable single source of truth

### Principles
- Clarity and consistency above all
- Second-person active voice
- Do not pre-announce future features
- Write for accessibility and global audience
- Examples before theory
- Backward compatibility is sacred
- Single source of truth (AIPs + Style Guide + protos)

### Workflow
1. Design the API / system first (AIP process mindset)
2. Write Concepts (why and how the system works)
3. Write Guides / How-to (step-by-step success path)
4. Produce Reference (precise, complete, generated where possible)
5. Add Quickstarts and Samples
6. Apply Style Guide rigorously
7. Review for cross-product consistency

### Rules (Hard)
- Sentence case for titles and headings
- Numbered lists for sequences, bulleted for unordered, description lists for pairs
- UI elements in **bold**
- Descriptive link text (never "click here")
- Alt text on every image
- Serial commas
- Present tense for API descriptions
- Every public class, method, parameter, and field must have a clear description
- Conditions before instructions

### Patterns
- Quickstart → Concepts → Guides → Reference structure on every product
- Standard Methods first, Custom Methods only when necessary
- Unified error model
- Consistent pagination, filtering, ordering
- Client libraries as first-class citizens
- Proto definitions as source of truth for reference

### Constraints
- No breaking changes without major version
- Content must be translatable
- Assume no high prior knowledge
- Prefer short, scannable pages over long monologues
- Documentation must remain accurate with the code/API

## Instructions for Common Tasks

### When writing or rewriting documentation
- Start with the reader's job-to-be-done.
- Open with a clear Overview that orients and routes.
- Follow progressive disclosure strictly.
- Use second person and active voice throughout.
- Put a short, working code sample near the top of reference pages when useful.
- Prefer concrete examples over abstract explanation.
- End guides with "What's next" or clear next steps.

### When reviewing existing Google or Google-style docs
- Score against the principles and rules above.
- Flag inconsistencies with resource-oriented design or standard methods.
- Check voice, list types, link text, accessibility, and global readability.
- Suggest concrete rewrites that restore the system spirit.

### When reverse-engineering any documentation set
- Decompose into Concepts → Principles → Workflow → Rules → Tools → Patterns → Examples → Constraints.
- Identify what makes the set function as a coherent system, not just a collection of pages.
- Extract the reusable "operating system" so it can be applied elsewhere.

### When designing new API or product docs
- Enforce resource-oriented design and AIP-inspired patterns.
- Define standard methods before custom ones.
- Plan the documentation structure at the same time as the API surface.
- Ensure the docs will feel native to a developer already familiar with other Google APIs.

## Reference Files

Load these only when deeper detail is required:

- `references/aip-core-principles.md` — Core AIP design principles and resource model
- `references/style-guide-essentials.md` — Condensed Google Developer Documentation Style Guide
- `references/resource-oriented-design.md` — Resource names, standard methods, patterns
- `references/progressive-disclosure-patterns.md` — How to structure content layers

## Assets

- `assets/doc-structure-template.md` — Ready-to-use page and product documentation skeleton

## Decision Rule

If a choice improves short-term cleverness but breaks consistency, progressive disclosure, or the shared mental model across Google products, reject it. The long-term developer experience always wins.
