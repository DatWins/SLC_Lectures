# Essential Chess Lectures

A one-page [Hugo](https://gohugo.io/) site (theme: [hugo-scroll](https://github.com/zjedi/hugo-scroll)) with 259 chess lecture videos,
organized into 7 topics plus a "By Lecturer" section:
Openings, MiddleGame, Endgame, Game Analysis, Tactics, Positional Play, Calculation.

- Side menu on desktop, sticky scrolling menu on phones and tablets. Wood-toned colors.
- Each section is one file in `content/en/homepage/` (`01-openings.md` ... `08-by-lecturer.md`).
  Add a lecture by adding a `- [Title - 12:34](https://youtube.com/...)` line. A video can appear in more than one section.
- Cover text and picture: `content/en/_index.md` and `assets/images/cover-image.jpg`.
- Colors and style tweaks: `layouts/partials/custom_head.html`.

## Run locally

Needs Hugo **extended** 0.147 or newer. Clone with submodules (the theme is a submodule):

```
git clone --recurse-submodules https://github.com/DatWins/SLC_Lectures
cd SLC_Lectures
hugo server
```

## Deploy

Pushing to `main` publishes to GitHub Pages through `.github/workflows/hugo.yaml`.
In the repo's Settings → Pages, set the source to "GitHub Actions".
