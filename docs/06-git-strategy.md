## Purpose
The purpose of this document is to write a set of rules to follow when developing to ensure that git commits are clean and meaningful.

## Branching Strategy
1. main: Stable and deployable branch. Only merged changes should exist here.
2. feature/xxx: Used for developing new features
3. docs/xxx: Used for documentation updates
4. fix/xxx: Used for bug fixes
5. refactor/xxx: Used for code improvements without changing functionality

## Development Flow
1. Create issue
2. Move issue to Ready
3. Create a branch from main
4. Work on the task
5. Commit changes incrementally
6. Perform self-review of code
7. Use AI for review and refinement if needed
8. Push branch to repository
9. Perform manual testing (and automated tests when available)
10. Merge into main
11. Mark issue as Done

## Commit Message Rules
Use clear and consistent prefixes:

- feat: add new feature
- fix: fix a bug
- docs: update documentation
- chore: setup or maintenance tasks
- refactor: improve code without changing functionality

Format:
<type>: short description

Example:
feat: implement investment validation logic
fix: handle pool cap overflow case
docs: update project charter scope

## Definition of Done
1. Requirements of the issue are fully implemented
2. Code is reviewed (self-review and AI-assisted review)
3. No obvious bugs or logical errors
4. Code is committed and pushed to a branch
5. Changes are merged into main
6. Issue is marked as Done

## Rules to Prevent Bad Habits
1. No coding without a defined issue
2. No large or messy commits
3. No skipping self-review before asking for help
4. No jumping between multiple tasks at the same time
5. No direct commits to main
