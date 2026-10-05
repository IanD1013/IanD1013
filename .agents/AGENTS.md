# AGENTS.md

These instructions apply across all agent scenarios.

## Writing and Formatting

- Never use em dashes.
- Use plain hyphens instead.
- When writing commit messages, never auto-add your agent name as a co-author.
- Preserve normal Markdown structure.
- Never manually modify `CHANGELOG.md` files.
- Never manually modify files marked as auto-generated.
- Always respond in Simplified Chinese. This applies regardless of whether the user communicates in English, Chinese, or a mix of both. Keep code, identifiers, commands, file paths, API names, and other syntax-sensitive content in their original form when appropriate.

## Engineering Principles

- Do not preserve backward compatibility.
- Remove obsolete paths instead of adding compatibility layers, fallbacks, or migrations.
- Choose the simplest implementation that fully meets the current requirements.
- Avoid speculative abstractions, configuration, and indirection.
- Keep components modular and concerns clearly separated.
- Grow the system in layers.
- Start from the smallest version that works end to end.
- Add each new capability on top of a product that already works.
- Never trade a working product for unfinished complexity.
- Prefer established, well-maintained libraries when they reduce overall complexity or improve reliability.
- Do not reimplement common functionality without a clear reason.
- Lean on the dependencies already in the project before writing your own implementation or adding packages.
- Do not assume a library lacks a capability without checking its documentation and types.
- Make architectural decisions for the long term.
- Do not accept a stopgap that only works for now and is meant to be replaced later.
- Study how established products solve the problem before designing a solution.
- Adopt proven patterns and conventions rather than inventing an approach from scratch.

## Quality Standards

- When making technical decisions, do not give much weight to development cost.
- Prefer quality, simplicity, robustness, scalability, and long term maintainability.
- Apply a high standard to engineering excellence.
- Fix lint failures, test failures, and test flakiness when you see them, even if they are not caused by the current task.

## Bug Fixes

- When doing bug fixes, always start by reproducing the bug in an end-to-end setting.
- Reproduce the bug as closely aligned with the end user experience as possible.
- This helps ensure you find the real problem and that the fix actually solves it.

## End-to-End Testing

- When end-to-end testing a product, be picky about the UI you see.
- Be obsessed with pixel perfection.
- If something clearly looks off, try to get it fixed along the way, even if it is not directly related to the current task.
