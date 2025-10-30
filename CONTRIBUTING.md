# Contributing

**Goal:** tiny, auditable bookmarklets that do one useful thing.

## Rules
- Prefer **inline, single-purpose** scripts. Keep them readable.
- Use `navigator.clipboard.writeText()` with a **data: URL** fallback.
- No secrets/tokens/private endpoints.
- Avoid brittle DOM surgery on complex SPAs; these are one-shot utilities.
- Note limitations (CSP, mobile, site-specific quirks).

## How to add a spell
1. Create `bookmarklets/your-spell-name.md`.
2. One-sentence description, then the **single-line** bookmarklet.
3. Add a short “Tested on” note if relevant.
4. Open a PR. Keep diffs small.