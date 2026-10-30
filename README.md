# void-run

**VOIDRUN** is an arcade-style browser game about dodging glitches and progressing through levels. The project centers on `index.html`, which includes on-screen instructions and score and level displays. Follow the instructions on the page to get started.

## Play locally

Open `index.html` in a browser, or start a local server from the project folder:

```sh
python -m http.server 8000
```

Then visit <http://localhost:8000>.

## Asset and loading review checklist

These are review steps, not verified results. Record findings separately; this README does not claim that the checks have passed or that performance has been measured.

- [ ] Inspect `index.html` for local image, audio, video, font, stylesheet, and script references. Confirm each referenced local file exists and each relative path resolves. The listed project files include `index.html` and this README; no separate local asset files are listed.
- [ ] Review any media referenced by the page for unnecessarily large files or dimensions. Keep only assets that are actually used, and remove an asset only after confirming there are no remaining references to it.
- [ ] Review the page’s external dependencies and confirm each is intentional. The listed external links are jsDelivr stylesheets for Inter (400, 600, 800) and Space Grotesk (500, 700). Check that the page uses these fonts, that the links resolve when online, and that text remains readable if they do not load. No external script URLs are listed in the supplied link inventory; inspect `index.html` for any additional references.
- [ ] Open the page with network access unavailable or the font requests blocked. Check that the game remains usable and that fallback typography is legible.
- [ ] After changing references or assets, reload the page and repeat the checks affected by the change.

## Gameplay and layout review checklist

These are manual checks to perform, not reported results.

- [ ] Open `index.html` and check the on-screen instructions, game area, and score and level displays.
- [ ] Follow the instructions shown on the page to try the game interactions. Observe the score and level displays as you play; do not assume behavior beyond what the page describes.
- [ ] Check the page at narrow and wide viewport sizes. Look for overflow and confirm the instructions, game area, score, and level displays remain visible and usable.

## Accessibility review checklist

These are future review checks, not claims of accessibility or verified results.

- [ ] Use only the keyboard to reach and operate each interactive control and to play using the on-screen instructions. Check that the interaction order is understandable and keyboard use does not get trapped.
- [ ] Check that focused controls have a clearly visible focus indicator.
- [ ] Check that interactive elements have accessible names that describe their actions and that instructions identify the input needed to play.
- [ ] Review text and control contrast against their backgrounds, including instructions and score and level values, in relevant game states.
- [ ] If `index.html` references images, check that informative images have useful text alternatives and decorative images are not announced as meaningful content. If there are no images, this check is not applicable.
- [ ] If the game uses motion effects, check behavior with the operating system’s reduced-motion preference enabled and consider reducing nonessential motion.

## Personalize the page

- Edit the visible title, instructions, and other page copy in `index.html`. Keep the score and level displays consistent with the instructions shown to players.
- Inspect the existing style rules in `index.html` before changing colors, typography, or layout; no separate stylesheet is listed in the project files.
- The page’s listed external font stylesheets are for Inter and Space Grotesk. Keep them if those font choices are intentional; otherwise update the references and check the fallback typography.
- Before moving, renaming, or removing assets, inspect `index.html` for local `href` and `src` references and confirm the assets are unused.