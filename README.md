# void-run

**VOIDRUN** is an arcade-style browser game about dodging glitches and progressing through levels. The project consists of the single HTML page `index.html`, which includes on-screen instructions and score and level displays. Follow the instructions on the page to get started.

## Play locally

Open `index.html` in a browser, or start a local server from the project folder:

```sh
python -m http.server 8000
```

Then visit <http://localhost:8000>. To review a change, edit `index.html`, reload the page, and follow its on-screen instructions.

## Personalize the page

- Edit the visible title, instructions, and other page copy in `index.html`. Keep the score and level displays consistent with the instructions shown to players.
- Inspect `index.html` for the existing style rules before changing colors, typography, or layout; no separate stylesheet is listed in the project files.
- The page links to externally hosted Inter and Space Grotesk font stylesheets. Preserve those links if you want to retain the current font choices.
- Before moving or renaming anything, check `index.html` for local `href` and `src` references and keep their relative paths valid. No separate local asset files are listed.