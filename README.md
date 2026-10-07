# corsinvest.github.io

Root of `https://corsinvest.github.io/`: the page that lists the documentation sites of the open source software by Corsinvest. Each site is published by its own repository under `/<name>/`.

One static page in the style of [corsinvest.it](https://corsinvest.it/en/), with no build: GitHub Pages serves the files of the `main` branch as they are.

| File | What it is |
|---|---|
| `index.html` | The list of the documentation sites, one section for each platform (Proxmox VE, Visual Studio), with groups inside |
| `styles.css` | Colours, type and spacing of corsinvest.it, on its dark ground |
| `fonts/`, `wordmark-white.svg`, `favicon.svg` | Barlow (SIL Open Font License, see `fonts/OFL.txt`) and the Corsinvest marks |
| `og.png` | The image shown when the page is shared |
| `robots.txt` | The sitemap of every documentation site. A site in a subfolder cannot have its own `robots.txt`, so they are listed here |
| `google*.html` | Ownership check of Google Search Console for the whole host. Do not remove it: the property stops being verified |

The product icons are not copied here: each card loads `/<name>/icon-dark.svg` from the documentation site of that product.

## Adding a documentation site

1. A card in `index.html`, in the right section and group, with the description the site carries in its own config. The description is a copy: when it changes in the site, change it here too.
2. A `Sitemap:` line in `robots.txt`.
3. The sitemap submitted in Google Search Console, in the property `https://corsinvest.github.io/`.
