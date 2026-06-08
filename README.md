# SnapBot — Project Page

Project page for **SnapBot: Enabling Dynamic Human-Robot Interactions for Real-Time Computational
Photography** (Chanyeok Choi, Jeonghan Kim, Yunjae Nam, Youngmoon Lee — Hanyang University).

> Late-Breaking Report, *Companion of the 2024 ACM/IEEE International Conference on Human-Robot
> Interaction (HRI '24)*, Boulder, CO, USA, pp. 327–331.

- **Paper:** https://dl.acm.org/doi/10.1145/3610978.3640712 — `doi:10.1145/3610978.3640712`
- **Live page:** https://angledsugar.github.io/snapbot/

## View locally

```bash
python3 -m http.server 8000   # then visit http://localhost:8000
```

## Deploy

Hosted from `github.com/Angledsugar/snapbot` (`main` branch, GitHub Pages from `/`). The `.nojekyll`
file keeps `static/` served as-is. To update: edit `index.html` and push to `main`.

## Structure

```
index.html              # all content
static/images/
  teaser_fig1.jpg       # Fig. 1 — head-pose tracking / camera composition
  composition_fig3.jpg  # Fig. 3 — camera composition (Method)
  results_fig4.jpg      # Fig. 4 — component-wise comparison (Results)
  social_preview.png · favicon.ico · apple-touch-icon.png
static/css · static/js  # Bulma + template assets
```

Figures are from the ACM paper; the page links to the PDF on the ACM Digital Library. Built on the
[Academic Project Page Template](https://github.com/eliahuhorwitz/Academic-project-page-template)
(Nerfies); content under [CC BY-SA 4.0](http://creativecommons.org/licenses/by-sa/4.0/).
