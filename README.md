# void-run

**VOIDRUN** is an arcade-style browser game about dodging glitches and progressing through levels. Open `index.html` for the game instructions and score and level displays.

## Play locally

Open `index.html` in a browser, or start a local server from the project folder:

```sh
python -m http.server 8000
```

Then visit <http://localhost:8000>.

## Files and external resources

The supplied project-file list includes `index.html` and `README.md`; no separate local assets or build scripts are listed. The page links to Inter and Space Grotesk stylesheets hosted on jsDelivr, so those font requests depend on network access.

Before moving or renaming files, inspect `index.html` for local references and preserve or update their relative paths.

## Deployment-readiness checklist

The supplied files establish that `index.html` is the entry page. They do not establish a deployment provider, deployment configuration, or a completed deployment. Treat the following as recommendations to check for the deployment method you choose:

- [ ] Set the published output or root directory to the project directory containing `index.html`, so the entry page is at the published root. No build scripts or separate output directory are listed in the supplied project files.
- [ ] Inspect `index.html` for local asset references. Keep referenced files at the expected relative locations, or update the paths if files are moved. The supplied project-file list does not include separate local assets.
- [ ] Account for the external jsDelivr font stylesheets. Confirm the published page remains legible if those requests are unavailable.
- [ ] Keep passwords, API keys, tokens, and other secrets out of browser-delivered markup and scripts. The supplied project-file list does not establish any configuration or secret-management mechanism.
- [ ] After publishing, open the resulting page in a browser and preview the actual published version. Check that it loads, review the on-screen instructions and game area, observe score and level displays, and check the layout at narrow and wide viewport sizes.

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
