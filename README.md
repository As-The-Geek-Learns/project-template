# Project Name

> Brief description of what this project does.

## Quick Start

```bash
# Install dependencies (if any)
npm install

# Run the project
npm start
```

## Ironclad Workflow

This project uses the **Ironclad Workflow** — a structured 4-phase development process:

```
PLAN -> EXECUTE -> VERIFY -> SHIP
```

### Starting New Work

1. **Create a plan:**
   ```bash
   mkdir -p .workflow/sessions/SESSION-$(date +%Y-%m-%d)-feature-name
   cp .workflow/templates/plan-template.md .workflow/sessions/SESSION-$(date +%Y-%m-%d)-feature-name/plan.md
   ```

2. **Get plan approval** before writing code

3. **Execute** the planned tasks

4. **Verify** with AI code review:
   ```bash
   npm run verify
   ```

5. **Ship** when verification passes:
   ```bash
   npm run ship:pr
   ```

### Workflow Commands

| Command | Description |
|---------|-------------|
| `npm run verify` | Full verification with AI review |
| `npm run verify:skip-ai` | Verify without AI review |
| `npm run ai-review` | Run AI review only |
| `npm run ai-review:diff` | Review git changes only |
| `npm run ship` | Validate integrity |
| `npm run ship:pr` | Validate and create PR |

### Environment Setup

Copy `.env.example` to `.env` and add your Gemini API key:

```bash
cp .env.example .env
# Edit .env and add your GEMINI_API_KEY
```

## Project Structure

```
.
├── src/                    # Source code
├── scripts/                # Ironclad workflow scripts
├── .workflow/              # Workflow documents
│   ├── templates/          # Plan, session, PR templates
│   ├── checklists/         # Security and verification checklists
│   ├── sessions/           # Active session documents
│   └── state/              # Verification state files
├── .cursor/rules           # Cursor IDE workflow enforcement
├── CLAUDE.md               # AI assistant context
└── package.json
```

## License

MIT
