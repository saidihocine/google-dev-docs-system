# Google Dev Docs System

A skill that encodes the **operating system** behind Google Developers documentation.

It forces an AI agent to think, structure, and write documentation the way Google does — not just copy surface style.

## What this skill does

When activated, the agent:

- Analyzes any documentation task through the full system layers (Concepts → Principles → Workflow → Rules → Patterns → Constraints)
- Enforces **resource-oriented design** and standard methods
- Applies strict **progressive disclosure** (Overview → Concepts → Guides → Reference → Samples)
- Uses Google’s official voice: second person, active voice, conversational but professional
- Prioritizes consistency across products over clever one-off solutions
- Writes for a global, accessible audience

## Core Philosophy

Google documentation is a **product**, not a byproduct.

Key axioms:
- Consistency beats cleverness
- The developer who learned one Google API must understand the next one immediately
- Documentation is part of the API surface
- Progressive disclosure is mandatory
- Clarity and accessibility for a global audience override local preferences
- Break any rule if following it would produce worse content (Orwell principle)

## Repository Structure

```
google-dev-docs-system/
├── SKILL.md                              # Main skill instructions
├── references/
│   ├── aip-core-principles.md            # Condensed AIP design principles
│   ├── style-guide-essentials.md         # Google Developer Documentation Style Guide essentials
│   ├── resource-oriented-design.md       # Resource model and standard methods
│   └── progressive-disclosure-patterns.md # Content layering patterns
└── assets/
    └── doc-structure-template.md         # Ready-to-use documentation skeleton
```

## How to use

### Inside Grok / xAI environment
Place the skill folder in your skills directory. The agent will automatically load it when the task matches the description triggers.

### As a reference for humans or other agents
Read `SKILL.md` first. Load the reference files only when deeper detail is needed.

### When writing or reviewing documentation
Apply the Decision Rule at the end of `SKILL.md`:

> If a choice improves short-term cleverness but breaks consistency, progressive disclosure, or the shared mental model across Google products, reject it. The long-term developer experience always wins.

## Origin

This skill was reverse-engineered from the real system that powers Google Developers documentation, AIP (API Improvement Proposals), the official Style Guide, and the consistent experience across Cloud, Workspace, Maps, and other Google products.

---

Built to make documentation feel like a coherent system, not a collection of pages.
