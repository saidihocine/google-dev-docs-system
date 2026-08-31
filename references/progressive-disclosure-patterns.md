# Progressive Disclosure Patterns

Google documentation almost always follows a layered revelation of information. The reader should never be forced to absorb everything at once.

## Canonical Layer Order

1. **Overview / Landing**
   - What the product or feature is
   - Who it is for
   - What problem it solves
   - Clear next steps and navigation

2. **Concepts**
   - Mental model
   - Core objects and relationships
   - Key principles and constraints
   - Architecture or data model when needed

3. **Guides / How-to**
   - Task-oriented, step-by-step
   - Shortest path to a working result
   - Common scenarios
   - Troubleshooting when relevant

4. **Reference**
   - Complete, precise, machine-oriented where possible
   - Every public surface documented
   - Code samples close to the definitions

5. **Samples & Quickstarts**
   - Minimal working examples
   - Copy-paste ready when possible
   - Language-specific when the audience needs it

## Practical Rules
- Never dump full reference material into a concepts page.
- Never hide the "why" inside a long how-to.
- Every page should have a clear primary job.
- Use "What's next" or equivalent navigation at the end of guides.
- Keep pages scannable: short paragraphs, clear headings, lists.

## Structure Test
If a new reader lands on a random page, can they quickly understand:
- Where they are in the overall system?
- What this page is for?
- Where to go next?

If not, the progressive disclosure has failed.
