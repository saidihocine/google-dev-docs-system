# Resource-Oriented Design Patterns

This is the dominant mental model in Google APIs and documentation.

## Core Idea
Treat the API as a collection of resources (nouns) that users can create, read, update, and delete. Actions are methods on those resources.

## Resource Names
- Hierarchical and hierarchical-looking paths.
- Example pattern: `projects/{project}/locations/{location}/services/{service}`
- Resource IDs should be stable and user-friendly when possible.
- Users should store the full resource name as the canonical identifier.

## Standard Methods Preference Order
1. Get
2. List
3. Create
4. Update
5. Delete

Only introduce custom methods when the standard five cannot express the needed behavior cleanly.

## Common Supporting Patterns
- Pagination on List methods
- Filtering and ordering using consistent query parameters
- Long-running operations for expensive work
- Consistent error responses
- Parent-child resource relationships expressed in the name hierarchy

## Documentation Implications
- Document resources first, then the methods that operate on them.
- Show the resource name format early and clearly.
- In guides, walk the user through creating → using → managing the resource.
- In reference pages, keep method descriptions tightly focused on what the method does to the resource.

## Consistency Test
Ask: "If a developer already knows the Cloud Storage or Pub/Sub resource model, will this feel familiar?" If the answer is no, redesign.
