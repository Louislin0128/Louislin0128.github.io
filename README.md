# Louis Lin Portfolio

Static multi-page portfolio built with plain HTML, CSS, and JavaScript. No backend or build step is required; it is structured for GitHub Pages.

## Pages

- `index.html` — the About page and site entry point: profile hero, Quick Facts, four-column skills, research timeline, education, contact actions, and English-resume download.
- `about.html` — compatibility redirect to `index.html` for old bookmarks.
- `honors.html` — independent award archive grouped by high school, university, and graduate school. Add each award in `data/awards.js` and place its certificate under `assets/awards/`.
- `journal.html` — independent journal/article-index template with clearly marked pending titles.

The interface supports Traditional Chinese and English, plus light/dark themes. GitHub and LinkedIn are represented by local SVG icon buttons in the navigation; they open the owner's profiles in a new tab. The supplied English resume is linked from the About page at `assets/resume/Louis_Lin_Resume_EN.pdf`.

## Preview locally

```sh
python3 -m http.server 8000
```

Then open `http://localhost:8000`.

## Replace pending content

- `assets/images/louis-portrait-focus.jpg` is a subject-focused, vertical crop of the portrait supplied by Louis Lin. The original is unchanged. Replace this file or update the image reference in `index.html` to use a new portrait.
- The scenic hero photograph is still a clearly labeled placeholder on `index.html`. Add an approved landscape image later and give it localized alt text.
- Add education photographs in `assets/images/education/` using `high-school.jpg`, `university.jpg`, and `graduate-school.jpg`; replace the marked placeholders in `index.html` with image elements and descriptive alt text.
- Add award certificates under `assets/awards/` and update `data/awards.js`. Confirm award wording and publication details against original certificates or official sources before describing them as verified.

The bilingual profile copy, Quick Facts, skill labels, career details, and education tags are in `index.html` and `script.js`. Research dates and achievement details follow the supplied English resume. Official NYCU and NKUST marks are stored in `assets/images/logos/`; their provenance is recorded in `ASSET-SOURCES.md`.

## Cat widget

The animated cursor-following cat is the local vanilla-JavaScript `oneko.js` widget by adryd. It is enabled on fine-pointer devices when reduced motion is not requested and can be hidden or shown. Its MIT license is included in `assets/vendor/oneko/LICENSE`; attribution appears in the footer.

## GitHub Pages

Publish the repository root or the `main` branch root in GitHub Pages settings. Links and assets are relative, so this project also works beneath a repository path such as `username.github.io/project-name/`.
