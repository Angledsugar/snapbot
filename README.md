# SnapBot — Project Page

Source for the **SnapBot** project page: an autonomous robotic photographer that pairs a
human-tracking collaborative manipulator with generative (AnimeGAN) style transfer and on-the-spot
photo printing. Built by **[Plan-Real](https://github.com/Plan-Real)** (Hanyang University ERICA) and
demonstrated at the *2023 Korea SW Talent Festival (SW인재페스티벌)* and *2023 HYU ERICA Spring Festival*.

- **Project code:** https://github.com/Plan-Real/Snapbot
- **Demo video:** https://drive.google.com/file/d/13aQ0mCv9reuY-JInxXiSdqex67w7G5Ey/view

## View locally

It is a static site — open `index.html` directly, or serve it (recommended, so the carousel/iframe work):

```bash
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Deploy (GitHub Pages)

Push these files to a repo and enable Pages (the `.nojekyll` file is already included so the
`static/` assets are served as-is). The page currently assumes it will live at
`https://angledsugar.github.io/snapbot/` — if you host it elsewhere, update the `og:url`,
`canonical`, and `og:image` / `twitter:image` URLs near the top of `index.html`.

## Structure

```
index.html              # all page content (edit here)
static/css/             # Bulma + the template's index.css
static/js/              # carousel, BibTeX-copy, scroll-to-top (index.js)
static/images/
  overview.jpg          # teaser / system overview
  tracking.jpg          # pipeline 1 — human tracking & framing
  animegan.jpg          # pipeline 2 — AnimeGAN style transfer
  frame.jpg             # pipeline 3 — frame composition
  print.jpg             # pipeline 4 — instant printing
  gallery1..6.jpg       # "SnapBot in the Wild" carousel
  social_preview.png    # 1200×630 link-share card
  favicon.ico / apple-touch-icon.png
```

## Credits

Page built on the [Academic Project Page Template](https://github.com/eliahuhorwitz/Academic-project-page-template)
(adapted from [Nerfies](https://nerfies.github.io)). Project code is MIT-licensed; the website content
is licensed under [CC BY-SA 4.0](http://creativecommons.org/licenses/by-sa/4.0/).
