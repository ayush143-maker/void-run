# void-run

**VOIDRUN** is an arcade-style browser game about dodging glitches and progressing through levels. Open `index.html` for the game instructions and score and level displays.

## Play locally

Open `index.html` in a browser, or start a local server from the project folder:

```sh
python -m http.server 8000
```

Then visit <http://localhost:8000>.

## Contributor handoff

- Keep changes scoped to the intended update.
- Preserve existing filenames and relative references. Before moving or renaming files, inspect `index.html` for paths and confirm they still resolve afterward.
- In your handoff, describe what changed, including any visible page or gameplay updates.
- Manually review the result before publishing. The checklist below is for review; it does not claim these checks have been completed.

### Manual review checklist

- [ ] Open `index.html` and check the on-screen instructions, game area, and score and level displays.
- [ ] Follow the page instructions to try the game and observe the displayed values.
- [ ] Check that the page remains usable at narrow and wide viewport sizes.
- [ ] Review browser console and network diagnostics for errors or failed requests.
- [ ] The page links to Inter and Space Grotesk stylesheets hosted on jsDelivr. Check that text remains legible if those external font requests are unavailable.