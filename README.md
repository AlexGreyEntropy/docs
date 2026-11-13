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
| `index.mdx` | Landing page with live numbers |
| `overview/` | What Thaler is, architecture, custody and policy, track record |
| `strategies/` | The three legs and the six risk profiles |
| `vault/` | Create, yield and claims, Yield Upfront, close, fees |
| `security/` | Principal safety, structural floor, incident response, risk disclosure |
| `glossary.mdx` | Every Thaler term, in dictionary format |
| `faq.mdx` | Frequently asked questions |
| `images/` | Strategy diagrams and update graphics |
| `docs.json` | Site configuration, navigation and theme |
| `logo/` | Light and dark Thaler wordmark |

## Editing rules

- Keep it simple. Plain markdown only: headings, short paragraphs, lists, tables, images. No blockquotes, no raw HTML or JSX components, no diagrams.
- Write in second-person voice ("you", "your vault").
- Active voice, direct language.
- Sentence case for headings.
- No buzzwords, no marketing copy, no AI terminology.
- Do not publish strategy parameters, position sizes or operational thresholds.
- All code blocks need a language tag.
- All internal links use root-relative paths without file extensions: `/strategies/index`.
- Define terms in dictionary format, in plain markdown: `### term`, then `*(noun)* · *pho · net · ic*`, a one-line definition, and `*e.g.: ... **term** ...*`. Add every term to `glossary.mdx`.
- Date every published number ("as of 13 November 2026"). Numbers are snapshots, never forecasts.
- Do not describe the structural floor or principal safety as guarantees until the on-chain reserve is live.

## Publishing

Push to `main`. Mintlify auto-deploys.
