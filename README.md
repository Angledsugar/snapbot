# SnapBot — Project Page

Project page for **SnapBot: Enabling Dynamic Human-Robot Interactions for Real-Time Computational
Photography** — a human-robot interaction system that detects face and pose for exposure and focus,
interactively controls a **UR3** arm for camera composition, and performs image scoring and
enhancement as an end-to-end pipeline. By Chanyeok Choi, Jeonghan Kim, Yunjae Nam, and Youngmoon Lee
(**Hanyang University ERICA**).

> **Late-Breaking Report**, *Companion of the 2024 ACM/IEEE International Conference on Human-Robot
> Interaction (HRI '24)*, Boulder, CO, USA, pp. 327–331.

- **Paper (ACM):** https://dl.acm.org/doi/10.1145/3610978.3640712 — `doi:10.1145/3610978.3640712`
- **Code:** https://github.com/Plan-Real/Snapbot
- **Demo video:** https://drive.google.com/file/d/13aQ0mCv9reuY-JInxXiSdqex67w7G5Ey/view
- **Live page:** https://angledsugar.github.io/snapbot/

## View locally

Static site — open `index.html`, or serve it (recommended, so the carousel/iframe work):

```bash
python3 -m http.server 8000   # then visit http://localhost:8000
```

## Deploy

Hosted from `github.com/Angledsugar/snapbot` (`main` branch, GitHub Pages from `/`) at
`https://angledsugar.github.io/snapbot/`. The `.nojekyll` file keeps `static/` served as-is. To
update: edit here and push to `main`. If you move the domain, update the `og:url`, `canonical`, and
`og:image` / `twitter:image` URLs near the top of `index.html`.

## Structure

```
index.html              # all page content (edit here)
static/css/             # Bulma + the template's index.css
static/js/              # carousel, BibTeX-copy, scroll-to-top (index.js)
static/images/
  teaser_fig1.jpg       # paper Fig. 1 — teaser (head-pose tracking, before/after)
  system_fig2.jpg       # paper Fig. 2 — system architecture
  composition_fig3.jpg  # paper Fig. 3 — camera composition (control)
  results_fig4.jpg      # paper Fig. 4 — component-wise comparison
  tracking.jpg          # pipeline 1 — perception (real detection photo)
  animegan.jpg          # pipeline 3 — scoring & enhancement (selection UI)
  gallery1..6.jpg       # "Live Deployment" carousel
  social_preview.png    # 1200×630 link-share card
  favicon.ico / apple-touch-icon.png
```

## Note on figures

Figures 1–4 are the actual paper figures, extracted from the ACM PDF. The paper PDF itself is **not**
redistributed here — the page links to it on the [ACM Digital Library](https://dl.acm.org/doi/10.1145/3610978.3640712).

## Credits

Page built on the [Academic Project Page Template](https://github.com/eliahuhorwitz/Academic-project-page-template)
(adapted from [Nerfies](https://nerfies.github.io)). Paper © 2024 ACM. Source code is MIT-licensed;
the website content is licensed under [CC BY-SA 4.0](http://creativecommons.org/licenses/by-sa/4.0/).
