# Commit Practices — Broadcast Baseball

This document defines the commit conventions for **Broadcast Baseball**.

The goal is to keep project history readable, searchable, and contributor-friendly,
without introducing unnecessary process or ceremony.

---

## Commit Message Standard

This project uses **Conventional Commits**.

### Format

```
<type>: <short, imperative summary>
```

Examples:
- `docs: finalize core vision and roadmap`
- `feat: add pitch-by-pitch at-bat simulation`
- `fix: correct count progression on foul balls`

---

## Commit Types

Use these types consistently:

- `docs:` Documentation changes only
- `feat:` New functionality (user-visible behavior)
- `fix:` Bug fixes that correct behavior
- `refactor:` Internal changes that do not alter external behavior
- `test:` Tests only
- `chore:` Tooling, configuration, and repository maintenance

If unsure:
- If it changes *what the program does*, use `feat:` or `fix:`
- If it changes *how the code is organized*, use `refactor:`
- If it changes the development environment, use `chore:`
- If it changes documentation, use `docs:`

---

## Message Style Rules

### Use imperative, present-tense language

Write commit summaries as commands:
- “add”, “fix”, “remove”, “update”

Good:
- `docs: add Phase 1 TODO checklist`
- `feat: emit structured PitchEvent records`

Avoid:
- `docs: added some things`
- `feat: working on at-bat logic`

---

### One commit = one idea

Each commit should represent a single, coherent change.

Avoid bundling:
- unrelated refactors
- code and docs unless inseparable
- multiple features in one commit

Smaller commits are easier to review, revert, and understand.

---

## Branching Practices

Keep branching lightweight and predictable:

- `main` is always stable
- Early development may happen directly on `main`
- Use short-lived branches for larger or experimental work:
  - `feat/one-at-bat-engine`
  - `docs/core-docs-refresh`

Avoid long-lived branches that drift from `main`.

---

## Documentation and Commit Boundaries

This project distinguishes between stable documentation and working notes:

- `docs/` contains **authoritative, intentional documents**
- `TODO.md` contains **tactical, short-lived work tracking**

If a TODO item persists for more than a few days, consider whether it belongs in `docs/`
as a design decision.

---

## Repository Signals

Broadcast Baseball aims to be easy to fork and contribute to.

Recommended baseline files:
- `README.md`
- `LICENSE` (MIT or Apache-2.0 recommended)
- `CONTRIBUTING.md` (short and welcoming)
- `CODE_OF_CONDUCT.md` (standard template)

These files reduce contributor friction and clarify expectations.

---

## Tooling Expectations

The project intentionally uses a small, modern toolchain:

- Python 3.12+
- `src/` layout
- Ruff for formatting and linting
- Pytest for testing
- `.venv` for local environments

Avoid overlapping tools unless there is a clear benefit.

---

## Practical Examples

Documentation changes:
```bash
git commit -m "docs: update radio-first principles"
```

New feature:
```bash
git commit -m "feat: add deterministic pitch outcome resolver"
```

Bug fix:
```bash
git commit -m "fix: treat foul balls as strikes only with fewer than two strikes"
```

Tooling:
```bash
git commit -m "chore: add pre-commit hooks"
```

---

## Why This Matters

A clean commit history:
- reduces cognitive load for maintainers
- improves review quality
- makes regressions easier to identify
- helps contributors understand project evolution quickly

If someone runs:

```
git log --oneline
```

They should be able to follow the story of the project without additional context.
