# reason.place

Monorepo for `reason.place` and small `*.reason.place` microsites.

The repository root is the home site for `https://reason.place/`. It currently links to `https://recipes.reason.place/` and is intentionally simple so more projects can be added later.

## Structure

- `/` — `reason.place` home
- `sites/<name>/` — standalone microsites such as `scent.reason.place`

`recipes.reason.place` remains in its own `ReasonJ01/Recipes` repository because it has its own build, content, and tests.

## Cloudflare Pages

For the home site:

- Repository: `ReasonJ01/reason.place`
- Production branch: `main`
- Framework preset: None
- Build command: leave blank
- Build output directory: `.`
- Custom domain: `reason.place`

For a microsite under `sites/<name>/`, create another Cloudflare Pages project from the same repository and use that directory as its build output directory. For example, `scent.reason.place` would publish from `sites/scent`.

No shared build system is required unless the microsites grow enough to justify one.
