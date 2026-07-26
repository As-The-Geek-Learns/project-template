# Project: [PROJECT NAME]

[One or two sentences: what this project does and why it exists. Assume the reader
can see the filesystem — don't restate the tech stack or directory layout here.]

## Workflow

Follows the global **Ironclad Workflow** (`PLAN → EXECUTE → VERIFY → SHIP` — see
`~/.claude/CLAUDE.md`). Scaffold commands:

```bash
npm run verify        # typecheck + tests + AI review (needs GEMINI_API_KEY; verify.js explains if unset)
npm run ship:pr       # validate and create PR
```

## Gotchas

Spend this file's tokens here — non-obvious constraints, incident-derived rules,
edge cases a fresh session would miss. Genre examples: "types live in
`src/types.ts` and nowhere else", "the staging DB wipes nightly". Delete this
explainer once real entries exist.

- [none yet]

## Pointers

Link deep material instead of inlining it — specs, ADRs, mockups, skills:

- [none yet — e.g. `docs/adr/`]
