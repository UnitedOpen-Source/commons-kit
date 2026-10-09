# Contributing to Commons Kit

Thank you for considering a contribution. Commons Kit is at an early stage, so discussion and design feedback are as valuable as code.

## Opening an issue

- Search existing issues first.
- For a bug, describe what you expected, what happened, and how to reproduce it (browser, assistive technology and version, if relevant).
- For a proposal, describe the problem before the solution, and link any public standard or design system pattern you are drawing on.
- Accessibility problems are bugs. Please label them `accessibility`.

## Proposing a pull request

1. Comment on the issue you want to work on so others know it is taken. For anything not covered by an issue, open one first.
2. Fork the repository and create a branch from `main`.
3. Keep the pull request focused on one issue, and reference it in the description (`Closes #N`).
4. Use [Conventional Commits](https://www.conventionalcommits.org/) for commit messages (`feat:`, `fix:`, `docs:`, `chore:` and so on).
5. Include tests. Components need automated accessibility checks and a short note on keyboard and screen reader behaviour.
6. Add or update translations for every user-facing string in English, Brazilian Portuguese and Spanish. If you cannot translate a language, say so in the pull request and a maintainer will help.

## Architecture decisions

Structural decisions (choice of framework, build tooling, package boundaries, public API conventions, data formats) are recorded as Architecture Decision Records in `docs/adr/`, one decision per file, named `NNNN-short-title.md`, using the Michael Nygard format: context, decision, status, consequences. If your change makes or reverses such a decision, include an ADR in the same pull request.

## Code of Conduct

Everyone taking part in this project is expected to follow the [UnitedOpen-Source Code of Conduct](https://unitedopensource.org/code-of-conduct).

## License

By contributing, you agree that your contributions are licensed under the [Apache License, Version 2.0](LICENSE).
