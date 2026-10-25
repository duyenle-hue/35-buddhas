# Thirty-Five Buddhas website

A learning website about the 35 Confession Buddhas (Tam Thập Ngũ Phật), built from Duyen's set of 35 Tibetan-style cards with Vietnamese captions.

## Who it is for
- Main audience: curious people who do NOT speak Vietnamese and may know nothing about Buddhism.
- Second audience: Vietnamese visitors. The site is fully bilingual (English / Tiếng Việt).
- Keep language plain. Explain every Buddhist word the first time it appears.

## How the site is built
- Everything is in ONE file: `index.html` (HTML + CSS + JavaScript). No build step, no frameworks.
- Images: `img/01.jpg` … `img/35.jpg` (painting, 720px wide) and `img/01t.jpg` … `img/35t.jpg` (round thumbnail, 200px).
- To preview: double-click `index.html` to open it in a browser. Refresh after each change.

## Sections of the page
1. Language switch (English | Tiếng Việt), saved in the browser.
2. Header + four "ways in" buttons: Tour, Explore the map, Practice, Matching game.
3. The map: Shakyamuni (#1) in the center, 34 Buddhas on 8 compass spokes, plus "Above" and "Below" rows.
4. "Start from a habit" chips (anger, pride…) that highlight the matching Buddha.
5. Four steps of letting go (regret, refuge, remedy, resolve).
6. List of all 35.
7. Detail popup for each Buddha (`#dlg`), Practice full screen (`#prac`), Matching game full screen (`#game`), Tour panel (`#coach`).

## Where the data lives (inside the `<script>`)
- `B` — one row per Buddha: `[number, English name, Sanskrit, Vietnamese name, Chinese, direction, world (vi), world (en), what the painting shows (en), what it purifies (en), habit key]`
- `GLOSS_VI`, `LOOK_VI`, `CAP_VI` — Vietnamese meaning of the name, painting description, and the card's own caption. Index = Buddha number.
- `STATIC` — every fixed sentence on the page, in `en` and `vi`. HTML elements show them through `<span data-i="key">`.
- `T` — sentences built by JavaScript (tour steps, game feedback…), in `en` and `vi`.
- `DIR`, `ANG`, `RAD` — directions and how the map is drawn.

## Rules when changing things
- Every new piece of text needs BOTH English and Vietnamese. Never add English-only text.
- Keep the colors as CSS variables in `:root` (light) and the two dark-mode blocks. Test in light and dark mode.
- Must work on a phone (about 390px wide) with no sideways scrolling.
- Keep the order of the 35 Buddhas and their directions exactly as on the cards. Do not invent new facts about the Buddhas; ask Duyen first.
- Captions on the cards are devotional. Present them as "traditionally said to purify…", not as guaranteed results.

## Still open
- Credit the publisher of the card set (footer says "publisher to be credited").
- A native speaker / teacher should check the Vietnamese meanings (`GLOSS_VI`) and painting descriptions (`LOOK_VI`), and the English world names.
- Decide whether to add a 36th figure (A Di Đà closes the Vietnamese Hồng Danh chant). Traditionally there are 35.
- Research notes: `../35 Buddhas - Research Notes.txt`.
