# BugLens

BugLens helps teams capture and report bugs with a web app, a browser extension, and Gemini-assisted analysis.

This repository is a folder-based monorepo. Application packages are placeholders; do not expect `npm install` or `bin/rails` to work until each package is scaffolded in a later task.

## Stack

| Area | Planned stack |
| --- | --- |
| Frontend | React, TypeScript, Vite |
| Backend | Ruby on Rails, PostgreSQL |
| Browser extension | WXT, TypeScript, Manifest V3 |
| AI | Gemini API |

## Layout

| Path | Role |
| --- | --- |
| [`frontend/`](frontend/) | Web UI (React + TypeScript + Vite) |
| [`backend/`](backend/) | API and persistence (Rails + PostgreSQL) |
| [`extension/`](extension/) | Browser extension (WXT + Manifest V3) |
| [`docs/`](docs/) | Repository documentation |

Contributor and agent rules live in [`AGENTS.md`](AGENTS.md). Localization plans live in [`docs/i18n.md`](docs/i18n.md).

## Locales

Product UI will support English (`en`), Japanese (`ja`), and Korean (`ko`). Repository docs and GitHub templates are English-only for now.

## Contributing

Use the GitHub issue forms (bug, feature, or task) or a blank issue when none of those fit. Pull requests should follow [`.github/PULL_REQUEST_TEMPLATE.md`](.github/PULL_REQUEST_TEMPLATE.md).
