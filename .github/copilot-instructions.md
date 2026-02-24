# Copilot Code Review Instructions — [Project Name]

## Project context

<!-- Replace with 1-2 sentences: what the project does, stack, architecture. -->

## Review priorities

1. **Security first** — flag hardcoded secrets, missing input validation, injection risks.
2. **Error handling** — never suppress errors silently. Every catch must log or return a meaningful error.
3. **Type safety** — flag any types, unsafe casts, missing validation at boundaries.
4. **No magic numbers** — constants should be named and documented.

## Code style

- Conventional commits: feat:, fix:, docs:, refactor:, test:, chore:.
- Comments explain *why*, never *what*. Flag narration comments.
- Prefer early returns over deep nesting.

## Patterns to flag

<!-- Add project-specific anti-patterns. Examples: -->
<!-- - Missing auth checks on endpoints -->
<!-- - Direct DB access outside service layer -->
<!-- - Unused imports or dead code -->

## Testing

<!-- Describe test framework, file conventions, coverage expectations. -->
