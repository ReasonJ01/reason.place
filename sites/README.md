# Microsites

Each directory under `sites/` is a standalone `*.reason.place` site.

Suggested convention:

- `sites/scent/` → `scent.reason.place`
- `sites/books/` → `books.reason.place`

Each microsite should be deployable independently from Cloudflare Pages by selecting its directory as the build output directory.
