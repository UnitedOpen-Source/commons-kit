# Commons Kit

Reusable building blocks for transparent digital public services.

> Status: incubating. The project is starting now. Nothing here is released or ready for production use yet.

## Why

Public services increasingly run as web forms, and the people who use them often cannot choose an alternative. Two problems show up again and again:

- **Accessibility is uneven.** Teams rebuild the same buttons, fields and error messages, and each rebuild is a new chance to break keyboard access, focus handling or screen reader output.
- **Transparency is an afterthought.** People are asked for personal data without being told why, services change without a public record of what changed, and outages are announced, if at all, somewhere other than the service itself.

Mature government design systems such as the [GOV.UK Design System](https://design-system.service.gov.uk/), the [U.S. Web Design System](https://designsystem.digital.gov/) and the [Gov.br Design System](https://www.gov.br/ds/) show that shared, well-researched components work. Commons Kit aims to offer a small, openly licensed, framework-level kit that any public-interest team can adopt, with transparency treated as a first-class component rather than a policy page.

## What it is

- A set of TypeScript packages, planned as:
  - `@commons-kit/tokens`: design tokens (color, spacing, typography, focus) published as CSS custom properties.
  - `@commons-kit/ui`: accessible React components, starting with Button, Field and ErrorSummary.
  - `@commons-kit/forms`: schema-driven forms (validated with [Zod](https://zod.dev/)) that follow the "one thing per page" pattern.
  - `@commons-kit/transparency`: components that explain a service to the people using it, such as a "why we ask for this" note per personal-data field, a public change log and, later, a status page.
- Internationalised from the start: English, Brazilian Portuguese (pt-BR) and Spanish (es).
- Targeting [WCAG 2.2](https://www.w3.org/TR/WCAG22/) level AA as a minimum for every component.

## What it is not

- Not a replacement for a national design system. If your government already has one, use it; Commons Kit aims to be useful where none exists or where its transparency components can sit alongside one.
- Not a visual brand. Tokens are meant to be overridden.
- Not a backend, identity provider or case-management system.
- Not a compliance certificate. Using the components does not by itself make a service accessible or lawful; services still need testing with real users and legal review.

## Planned scope for v0.1.0

The v0.1.0 scope is tracked in the [v0.1.0 milestone](https://github.com/UnitedOpen-Source/commons-kit/milestone/1):

- Monorepo, build and CI foundation
- ADR on the component stack (React and CSS custom properties, versus alternatives)
- Design tokens package
- Accessible Button, Field and ErrorSummary
- Step-by-step form pattern driven by a schema
- "Data purpose" component: why each personal field is requested
- Public change log JSON Schema
- i18n message catalogs for en, pt-BR and es
- Documentation site with automated accessibility checks

## Principles

1. **Accessible by default, verified by tests.** Every component ships with automated axe checks and a written note on keyboard and screen reader behaviour. Automated checks are a floor, not proof of conformance.
2. **Explain every request for personal data.** A form field that collects personal data should be able to say, in plain language, why it is needed, who will see it and how long it is kept.
3. **Changes to a service are public.** Decisions and changes that affect users belong in a machine-readable, human-readable change log.
4. **One language is not enough.** No user-facing string is hard-coded; every string goes through the message catalog.
5. **Decisions are written down.** Structural choices are recorded as Architecture Decision Records in `docs/adr/`.

## Getting involved

- Look for issues labelled [`good first issue`](https://github.com/UnitedOpen-Source/commons-kit/labels/good%20first%20issue) or [`help wanted`](https://github.com/UnitedOpen-Source/commons-kit/labels/help%20wanted).
- Read [CONTRIBUTING.md](CONTRIBUTING.md) before opening a pull request.
- Participation is governed by the [UnitedOpen-Source Code of Conduct](https://unitedopensource.org/code-of-conduct).

## License

Licensed under the [Apache License, Version 2.0](LICENSE).
