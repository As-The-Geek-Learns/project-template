# Project: [PROJECT NAME]

## Overview

Brief description of what this project does and its purpose.

## Tech Stack

- **Language:** JavaScript/TypeScript/Python (update as needed)
- **Framework:** (if applicable)
- **Dependencies:** (list key dependencies)

## Project Structure

```
src/
├── index.js          # Entry point
└── ...               # Other source files
```

## Development Workflow

This project uses the **Ironclad Workflow**:

1. **PLAN** - Create a plan document before coding
2. **EXECUTE** - Implement planned tasks
3. **VERIFY** - Run tests + AI code review
4. **SHIP** - Create PR with verification evidence

### Key Commands

```bash
npm run verify        # Full verification with AI review
npm run ship:pr       # Validate and create PR
```

### Human Checkpoints

- Plan approval required before coding
- Verification approval required before shipping
- Human approves final merge

## Security Considerations

- All user inputs must be validated
- No secrets in code (use environment variables)
- Run `npm audit` before shipping

## Code Conventions

- (Add your coding conventions here)
- (Naming patterns, file organization, etc.)

## Environment Variables

| Variable | Required | Description |
|----------|----------|-------------|
| `GEMINI_API_KEY` | For AI review | Google Gemini API key |

## Current Status

- **Phase:** (PLAN / EXECUTE / VERIFY / SHIP)
- **Active Session:** (link to session document if any)
