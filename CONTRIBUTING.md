# Contributing to Resumio

Thanks for helping improve Resumio. It is a small, self contained, fully client side app, and good contributions start with respect for that.

## Design rules

- Follow `assets/md/DESIGN.md`. Resumio is a tool, not a marketing page, but it uses Discord's design language: deep indigo canvas, Blurple primary, magenta feature surfaces, green for the single high intent action, generous rounded corners.
- Never introduce long dash characters (em dash, en dash, box drawing). Use ASCII hyphens.
- Keep the app fully local. No server calls, no uploads, no tracking.
- Preserve accessibility: skip link, ARIA labels, keyboard focus, colour contrast.

## Code style

- One dependency free file, `index.html`, holding styles, markup and the engine.
- Use the existing patterns: CSS custom properties, plain functions, template literals.
- Do not add comments unless they explain something genuinely non obvious.

## How to work on it

1. Fork and create a branch.
2. Make your change, keeping the app working without a build step.
3. Verify your change. The project has no test runner: test in the browser at desktop and mobile widths, check print output, and confirm the JS block parses with `node --check`.
4. Update the CHANGELOG under Unreleased or the next version.
5. Open a pull request and describe what changed and why.

## Reporting issues

Open an issue with the steps to reproduce, expected behaviour and actual behaviour. If it is a visual issue, include a screenshot or a reduced case.