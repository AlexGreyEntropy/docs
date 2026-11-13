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
| `snippets/term.mdx` | The `<Term>` dictionary-entry component |
| `images/` | Strategy diagrams and update graphics |
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
- Define terms with the `<Term>` component in dictionary format: headword, part of speech, phonetic, plain definition, and an `e.g.:` example that uses the word. Add every new term to `glossary.mdx` too.
- Date every published number ("as of 13 November 2026"). Numbers are snapshots, never forecasts.
- Do not describe the structural floor or principal safety as guarantees until the on-chain reserve is live.

## Publishing

Push to `main`. Mintlify auto-deploys.
