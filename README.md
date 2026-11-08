# Engineering Portfolio — Juan Sebastian Betancourt Lasso

A self-contained, responsive **static site** intended for GitHub Pages. No build tools, APIs, packages, or external font dependencies are required. The published site will be **public**.

## Publish at `https://sbet18.github.io/`

1. Sign in to GitHub as `SBet18`.
2. Create a **public repository** named exactly `sbet18.github.io` (lowercase is required for a username containing capital letters). This is a **new** repository; leave the existing ESP32 repository alone.
3. Upload the **contents** of this folder to the root of the new repository. Preserve the `assets/` and `projects/` subfolders. The top-level file should be `index.html`.
   - Using Git on your computer: `git init && git add . && git commit -m "Add engineering portfolio" && git branch -M main && git remote add origin https://github.com/SBet18/sbet18.github.io.git && git push -u origin main`
   - Or upload the files via GitHub's **Add file → Upload files** interface, ensuring directories are preserved.
4. Open **Settings → Pages → Build and deployment → Source → Deploy from a branch**, choose `main` and `/(root)`, then save.
5. Visit `https://sbet18.github.io/` after GitHub publishes it. The URL is a proposed final URL, **not confirmed live yet**.

## Edit content

- `index.html`: homepage, project cards, experience and skills.
- `projects/*.html`: individual case-study pages.
- `assets/css/styles.css`: colors, spacing, layout and responsive rules.
- `assets/js/main.js`: mobile menu behaviour.
- `assets/img/`: all images sourced from supplied project screenshots or supplied PDF figures.
- `assets/reports/`: English Abaqus summary and original French collaborative report.

To test locally, open `index.html` in a browser. Most content works directly; embedded PDFs can be browser-dependent when opened as `file://`. For a local server: run `python -m http.server 8000` from the repository root, then visit `http://localhost:8000`.

## Review before making public

- **Confidentiality:** Verify that BFR Systems EuroCri permits publishing its conveyor component images and description outside Upwork; do not publish sensitive dimensions, supplier prices, or proprietary files without permission.
- **Collaborative coursework:** The original French Abaqus PDF includes the second student's and course instructor's names. Obtain relevant consent or remove that PDF if publishing it would be inappropriate. The website otherwise describes the work as collaborative.
- **Personal data:** The supplied CV is **not included** in this site, and your phone number is not published. The email address shown in the site is the contact address from the CV; remove the `mailto:` link if you prefer to be contacted only on LinkedIn.
- **Technical claims:** The Abaqus 0.39% figure is *change between mesh refinements*, not a verified absolute error. The 63% figure is against an initial supplier quote, not total costs.
- **Project separation:** Electric Formula SAE at UTP (listed in the Experience section) is **distinct** from the wall-mounted race car display fixture at ENIM.
- **Website status:** Nothing is uploaded automatically. Publishing on GitHub is a separate user action.

## Project sources

- ESP32 source: https://github.com/SBet18/esp32-soil-irrigation-controller
- Abaqus: user-supplied EN/FR PDF reports (2026).
- Display fixture and conveyor: user-supplied project descriptions and CAD/FEA images.
- Profile: user-supplied CV for the Alpine PFE candidature.

Site content is in English and can be expanded to French later.
