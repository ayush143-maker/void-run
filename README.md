# void-run

**VOIDRUN** is an arcade-style browser game about dodging glitches and progressing through levels. The project consists of the single HTML page `index.html`, which includes on-screen instructions and score and level displays. Follow the instructions on the page to get started.

## Play locally

Open `index.html` in a browser, or start a local server from the project folder:

```sh
python -m http.server 8000
```

Then visit <http://localhost:8000>.

## Manual review checklist

These are actions to perform, not verified results. Record findings separately; this README does not report that the checks have passed.

- [ ] Open `index.html` and confirm the page loads with its on-screen instructions and score and level displays.
- [ ] Inspect `index.html` for image, media, stylesheet, script, and font references. Check that each referenced path or URL resolves. The listed project files include only `index.html` and this README; the page references externally hosted Inter and Space Grotesk font stylesheets.
- [ ] Follow the instructions shown on the page to try the game interactions. Observe the score and level displays as you play; do not assume behavior beyond what the page describes.
- [ ] Inspect the page at a narrow viewport and a wide viewport. Check that the instructions, game area, score, and level displays remain visible and usable; note overflow or layout issues.
- [ ] After a change, reload the page and repeat the checks affected by that change.

## Personalize the page

- Edit the visible title, instructions, and other page copy in `index.html`. Keep the score and level displays consistent with the instructions shown to players.
- Inspect `index.html` for the existing style rules before changing colors, typography, or layout; no separate stylesheet is listed in the project files.
- The page links to externally hosted Inter and Space Grotesk font stylesheets. Preserve those links if you want to retain the current font choices.
- Before moving or renaming anything, check `index.html` for local `href` and `src` references and keep their relative paths valid. No separate local asset files are listed.