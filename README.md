# Relation — a word chart for reading Glissant

A small bilingual (English / French) vocabulary trainer for reading Édouard Glissant's *Poétique de la Relation* (*Poetics of Relation*, trans. Betsy Wing, 1997).

It covers 38 terms in two sets:

- **Philosophy toolkit** — ontology, epistemology, teleology, dialectic, alterity and other words Glissant assumes you know.
- **Glissant's own terms** — Relation, opacity, creolization, errantry, rhizome, Tout-monde, and more.

Each term has its French form (with gender and adjective where useful), a plain definition, and a note on how Glissant uses it.

## Features

- Three practice modes: word → meaning, meaning → word, flashcards
- Show words in English, French, or both
- Every correct answer charts an island on a small archipelago map; islands link up as you learn
- Progress saved in the browser (localStorage)
- Light and dark mode, works on phones, installable to a home screen

## Run it

It is a single static page with no build step. Open `index.html` in a browser, or publish with GitHub Pages:

1. Push this folder to a new repository.
2. Go to **Settings → Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**, branch `main`, folder `/ (root)`, and save.
4. The site appears at `https://<your-username>.github.io/<repo-name>/` after a minute or two.

## Files

```
index.html             the whole app (HTML, CSS, JS, word list)
manifest.webmanifest   lets phones install it as an app
icons/                 favicon and home-screen icons
.nojekyll              tells GitHub Pages to serve files as-is
```

## Editing the word list

The terms live in the `TERMS` array near the top of the `<script>` in `index.html`. Each entry looks like:

```js
{id:"opacity", cat:"glissant", en:"Opacity", fr:"l'opacité (f.)",
 def:"...", note:"..."}
```

`cat` is `"toolkit"` or `"glissant"`. `adj` is optional. Give each entry a unique `id`; the map places islands automatically.

## Licence

Code released under the MIT Licence (see `LICENSE`). Definitions and notes are original summaries written for study; no text from Glissant's books is reproduced.
