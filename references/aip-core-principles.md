# AIP Core Principles (Condensed)

API Improvement Proposals (AIPs) are the living design constitution for Google APIs. They ensure consistency so that learning one Google API makes the next one easier.

## Foundational Goals
- Simple
- Intuitive
- Consistent across the entire Google API corpus

## Resource-Oriented Design (AIP-121)
- APIs expose resources (nouns), not just actions.
- Users create, retrieve, and manipulate resources.
- Resources have unique names that users store as canonical identifiers.

## Resource Names (AIP-122)
- Format follows URI path schema without leading slash.
- Example: `projects/{project}/locations/{location}/datasets/{dataset}`
- Use `/` to separate segments.
- Prefer DNS-compatible characters; avoid upper-case in IDs.
- Full resource names can cross API boundaries when needed.

## Standard Methods
- Get (AIP-131)
- List (AIP-132)
- Create (AIP-133)
- Update (AIP-134)
- Delete (AIP-135)

Prefer these over custom methods. Custom methods (AIP-136) are allowed only when the standard set is insufficient.

## Key Supporting Rules
- Versioning and backward compatibility are strict (AIP-180, AIP-185).
- Errors follow a unified model (AIP-193).
- Standard fields and naming conventions are enforced (AIP-148, AIP-190).
- Documentation is considered part of the API surface (AIP-192).

## Design Review Mindset
Review every surface from the perspective of a naïve user who already knows other Google APIs. Ask:
- Is this consistent with existing patterns?
- Is the resource model clean?
- Will this surprise a developer who has used Cloud Storage or Pub/Sub?

Consistency is not optional. It is the product.
