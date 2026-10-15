# Odooers Forum

Odoo community Q&A forum for the Odooers marketplace (https://odooers.razs.dev).

- Technical name: `odooers_forum`
- Odoo version: 19.0 (Community)
- Scope: `tenant` (odooers) -- installable only in the Odooers database. Placement
  under `user/tenants/odooers/` declares this and `tenancy_guard` enforces it at
  install time (see the project root `CLAUDE.md`, "Addon scope hierarchy").
- License: LGPL-3 (GNU Lesser General Public License v3, see `LICENSE`), the same
  licence as Odoo Community. Open source; contributions welcome.

## Status

Scaffold only -- no functionality yet. The module depends only on `base` and is
intentionally independent of the other Odooers addons; dependencies (for example
Odoo's native `website_forum`) are added when the approved design calls for them.

## Planned scope

A public, Odoo-specific question-and-answer community: authenticated users ask,
answer and comment; tags, search, voting and accepted answers; moderation and
spam protection; SEO-friendly public questions; reputation without invented
credentials; and integration points with Odooer profiles, expertise and
marketplace opportunities. The design is proposed and approved through OpenSpec
before implementation.

## Development

- Odoo addon at `odooers_forum/`; this wrapper is its own Git repository.
- Spec-driven changes live in `openspec/` (run OPSX from this directory).
- Commits follow `action(scope): description` (one file or logical unit per commit).
