# Vendored third-party assets

Served from this site instead of `cdn.jsdelivr.net`, which is slow or unreachable on many
mainland-China networks — when it fails, formulas stay as raw LaTeX.

| Path | Package | Version | License |
| --- | --- | --- | --- |
| `mathjax/` | [`mathjax`](https://www.npmjs.com/package/mathjax) (`tex-chtml.js`, `a11y/`, `input/`, `ui/`, `sre/`) | 4.1.3 | Apache-2.0 (`mathjax/LICENSE`) |
| `mathjax-fonts/mathjax-newcm-font/` | [`@mathjax/mathjax-newcm-font`](https://www.npmjs.com/package/@mathjax/mathjax-newcm-font) (`chtml.js`, `chtml/`) | 4.1.3 | Apache-2.0 |

`sre/mathmaps/` keeps only `base`, `en`, `euro` and `nemeth`; other speech locales were dropped.

Update: `npm pack mathjax@<v> @mathjax/mathjax-newcm-font@<v>`, copy the same files over, then bump
the `?v=` query in `handbook/index.html`.
