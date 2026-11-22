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
| `index.mdx` | What Thaler is, at a glance |
| `how-it-works.mdx` | Staking, lending loop, hedge, and how it earns in each market |
| `create-vault.mdx` | Sign in, fund, pick a risk profile, open a vault |
| `yield.mdx` | Auto-claim, auto-compound, claiming early |
| `yield-upfront.mdx` | Yield Upfront |
| `closing.mdx` | Closing a vault |
| `fees.mdx` | Fees |
| `safety.mdx` | Custody, audit, risks |
| `docs.json` | Site configuration, navigation and theme |
| `glossary/` | Definition card images shown when you hover a term |
| `style.css` | Hover card styling, one line per term |
| `logo/` | Light and dark Thaler wordmark, from the landing site |

## Editing rules

- Keep it simple. Plain markdown only: headings, short paragraphs, lists, tables. No images, blockquotes, raw HTML, JSX components or diagrams. The one exception is glossary terms, below.
- Write for someone who has never used DeFi. Wrap the first use of any new term on a page in `<span className="term term-<slug>" tabIndex={0}>term</span>`. Hovering (or tapping) it shows that term's definition card from `glossary/<slug>.webp`.
- To add a term: make its card in thaler-drafts at `/update` (Definition style, Rock background), export it as `glossary/<slug>.webp`, and add a `.term-<slug>::after` line to `style.css`.
- Write in second-person voice ("you", "your vault").
- Active voice, direct language.
- Title case for page titles and sidebar groups ("Create a Vault"). Sentence case for headings inside a page.
- No buzzwords, no marketing copy, no AI terminology.
- Do not publish strategy parameters, position sizes or operational thresholds.
- All code blocks need a language tag.
- All internal links use root-relative paths without file extensions: `/strategies/index`.
- No live numbers (TVL, APR, vault counts, volume). They go stale. Link to the app at `app.thaler.finance` instead. Fixed history, like closed rounds and past events, is fine.
- Do not describe the structural floor or principal safety as guarantees until the on-chain reserve is live.

## Publishing

Push to `main`. Mintlify auto-deploys.
