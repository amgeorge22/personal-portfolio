# Alex George: Portfolio Site

A static site (plain HTML + CSS, no build step) ready for GitHub Pages.

## Publish on GitHub Pages

1. Create a new repository on GitHub. For a personal site named `<username>.github.io`, use exactly that repo name.
2. Upload everything in this folder to the repo root (`index.html` must be at the top level).
3. In the repo go to **Settings > Pages**, set **Source** to "Deploy from a branch", choose `main` and `/ (root)`, and save.
4. After a minute the site is live at `https://<username>.github.io/`.

A custom domain can be added later in the same Pages settings screen.

## Adding your pictures

Every picture slot currently shows a striped placeholder that tells you what goes there **and the exact file name it expects**, for example `assets/img/fsae-motor-mounting/03.jpg`.

Just drop a file with that name into that folder and the placeholder is replaced automatically. No HTML editing needed.

- Images: `assets/img/<project-name>/NN.jpg` (use `.jpg`)
- Project card thumbnail: `assets/img/<project-name>/00.jpg`
- Headshot on the home page: `assets/img/headshot.jpg`
- Videos: `assets/video/<project-name>-NN.mp4`

Tip: keep photos under about 1.5 MB each (export at ~2000 px wide) so pages load quickly.

## Links still to fill in

Buttons and links that point to files or URLs you haven't supplied yet are marked `data-todo="true"` (or `href="#"`) in the HTML. Search the project for those.

| Where | What it needs |
| --- | --- |
| Home | `assets/docs/resume-robotics.pdf`, `assets/docs/resume-mechanical.pdf` |
| Footer (every page) | LinkedIn URL, GitHub URL, email address |
| Automated Poker Dealer | Github pages URL, Github repository URL |
| Inverted Pendulum Controller | `assets/docs/inverted-pendulum-report.pdf` |
| FSAE Motor Mounting | `assets/docs/fsae-motor-mounting-breakdown.pdf` |
| Beam Deflection Calculator | `assets/docs/beam-deflection-report.pdf` |
| 3D Printing Variability Study | `assets/docs/3d-printing-variability-report.pdf` |
| Injection Keychain / Airpod Case / Treasure Box | `assets/docs/dfm-portfolio.pdf` |
| Sudoku Graph Coloring | Colab notebook URL |
| SoftDew Valley | project website URL |
| Poi Style Classifier | project website URL |

The footer is repeated in each HTML file, so use find-and-replace across the folder when you update the social links.

## Structure

```
index.html            home
mechatronics.html     category pages
mechanical.html
software.html
research.html
projects/*.html       one page per project
style.css             all styling (colors are variables at the top)
assets/               your images, videos and PDFs
```
