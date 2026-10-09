# Agent and contributor rules

BugLens is a folder-based monorepo. Keep work inside the package that owns the concern.

## Package boundaries

- `frontend/` — web UI (React, TypeScript, Vite). Do not use Next.js.
- `backend/` — API and data (Ruby on Rails, PostgreSQL).
- `extension/` — browser-only code (WXT, TypeScript, Manifest V3).
- `docs/` — repository documentation, not runtime code.

Do not add dependencies, scaffolding, or tooling unless the user asked for it.

## Secrets

Do not commit secrets, credentials, or `.env` files. Use `.env.example` for non-secret names only.

## Issues and pull requests

Write GitHub issue and pull request bodies in English. Prefer the bug, feature, or task forms; blank issues are allowed when no form fits.

## Internationalization

When application UI exists, do not hardcode user-facing strings. Use the same message keys for `en`, `ja`, and `ko`. English is the source locale. See [`docs/i18n.md`](docs/i18n.md). Do not add i18n libraries until a later task.

## AI-assisted development workflow

- For non-trivial work, propose a plan first and implement only after the user approves.
- Split changes into small, reviewable units.
- Inspect existing code before modifying it.
- After implementing, explain what changed and why.
- Run relevant tests and report the results.
- If a test could not be run, say so clearly and why.
- Do not commit or push unless the user explicitly asks.
- Explain new Rails concepts in Korean (한국어). Repository docs in this file stay in English; only the Rails explanations in chat/PR discussion should be Korean.

## Learning and code review

- Explain the reasoning behind non-obvious technical decisions.
- When introducing unfamiliar concepts, explain them in Korean.
- Do not modify unrelated files.
- Before writing tests, identify the expected behaviors and edge cases.
- After implementation, summarize the changes and highlight anything requiring manual review.
- Do not claim a task is complete if validation has not been performed.
