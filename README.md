# ValarAI documentation

The source for the [ValarAI](https://valarhq.ai) documentation site, built with [Mintlify](https://mintlify.com). Pages are MDX files with YAML frontmatter; site configuration lives in `docs.json`.

## Development

Install the Mintlify CLI and run a local preview from the repo root (where `docs.json` lives):

```bash
npm i -g mint
mint dev
```

The preview is served at `http://localhost:3000`.

## Validation

```bash
mint validate        # strict build validation
mint broken-links    # check internal links
mint a11y            # accessibility checks
```

## Deploying

Changes merged to `main` deploy to production automatically via the connected Mintlify GitHub app.

## Structure

- `docs.json` — navigation, theme, and API reference configuration
- `*.mdx` — documentation pages
- `api-reference/` — endpoint pages generated from `openapi.json`
- `openapi.json` — the ValarAI API specification
- `logo/`, `favicon.svg` — brand assets
