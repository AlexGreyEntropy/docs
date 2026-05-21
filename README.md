# Thaler Finance documentation

Public documentation for [Thaler Finance](https://thaler.finance). The site is published to `docs.thaler.finance` via Mintlify.

## Local preview

```bash
npm install -g mint
mint dev
```

Mintlify watches the local files and rebuilds on save. The dev server runs on `localhost:3000`.

## Structure

| Path | What lives here |
|------|------------------|
| `index.mdx` | Landing page |
| `overview/` | What Thaler is, architecture, custody and policy |
| `strategies/` | The three pillars and the per-tier strategy family |
| `vault/` | Create, claim, close, fees |
| `security/` | Principal protection, yield floor, risk disclosure |
| `faq.mdx` | Frequently asked questions |
| `docs.json` | Site configuration, navigation and theme |
| `logo/` | Light and dark Thaler wordmark |

## Editing rules

- Write in second-person voice ("you", "your vault").
- Active voice, direct language.
- Sentence case for headings.
- No buzzwords, no marketing copy, no AI terminology.
- Do not publish strategy parameters, position sizes or operational thresholds.
- All code blocks need a language tag.
- All internal links use root-relative paths without file extensions: `/strategies/index`.

## Publishing

Push to `main`. Mintlify auto-deploys.
