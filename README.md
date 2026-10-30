# void-run

**VOIDRUN** is an arcade-style browser game about dodging glitches and progressing through levels. Open `index.html` to view the game instructions and score and level displays; follow the on-page guidance to play.

## Play locally

Open `index.html` in a browser, or start a local server from the project folder:

```sh
python -m http.server 8000
```

Then visit <http://localhost:8000>.

## Files and resources

The supplied project-file list includes `index.html` and `README.md`; no separate local assets or build scripts are listed. The page links to Inter and Space Grotesk stylesheets hosted on jsDelivr, so those fonts depend on network access. Check that text remains legible if the external font requests are unavailable.

Before moving or renaming files, inspect `index.html` for local references and preserve or update their relative paths.

## Publishing notes

No deployment provider, deployment configuration, or separate build output is documented. For a static publication, use the project directory containing `index.html` as the published root. Preview the published page and check that it loads, then review the instructions, game area, score and level displays, and layout at narrow and wide viewport sizes. The supplied files do not establish a separate build step or deployment status.