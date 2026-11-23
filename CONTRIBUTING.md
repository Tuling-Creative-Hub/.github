# Contributing Guide

Thank you for contributing to **Tuling Creative Hub**. These standards keep codebases predictable, reviewable, and safe in production.

## 1. Branches & Commits
- Always branch off `main` using clear prefixes:
  - `feat/<scope>-<short-description>`
  - `fix/<scope>-<short-description>`
  - `chore/<scope>-<short-description>`
  - `docs/<scope>-<short-description>`
- Write concise, descriptive commit messages that explain what changed and why.
- Keep pull requests focused on a single concern rather than mixing unrelated refactors or formatting churn.

## 2. Code & Architecture Standards
- Respect module boundaries and keep business/domain logic separate from transport/UI layers.
- Ensure configuration, permissions, and validation rules are explicit and testable.
- Never commit secrets, API keys, credentials, private certificates, or real personal/institutional data.

## 3. Data & Migration Safety
- Treat database migrations, schema changes, and data imports/backfills as high-risk operations.
- Run read-only diagnostic checks and dry runs first, and review row/record counts before applying changes to live or shared environments.
- Make migrations and scripts idempotent and reversible wherever practical.

## 4. Pull Request Checklist
Before requesting review or merging:
- Code builds cleanly and passes existing lint, type, and test checks.
- Edge cases, error states, and permission checks are handled.
- Documentation, environment examples, or API specs are updated when behavior changes.
- All items in the Pull Request template are completed accurately.
