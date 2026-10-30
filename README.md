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

## Accessibility review checklist

These are future review checks, not claims of accessibility or verified results. Record issues and any follow-up separately.

- [ ] Use only the keyboard to reach and operate each interactive control and to play using the instructions shown on the page. Check that the interaction order is understandable and that keyboard use does not get trapped.
- [ ] Tab through the page and check that every focused control has a clearly visible focus indicator, including against the game area and surrounding backgrounds.
- [ ] Inspect the interactive elements in `index.html`. Check that controls have accessible names that describe their actions and that the on-screen instructions explain the keys or input needed to play.
- [ ] Check text and control contrast against their backgrounds, including instructions and score and level values. Review relevant states during play as well as the initial screen.
- [ ] If `index.html` includes images, check that informative images have useful text alternatives and decorative images are not announced as meaningful content. If there are no images, note that this check is not applicable.
- [ ] If the game uses animation or other motion effects, check how it behaves with the operating system's reduced-motion preference enabled. Consider reducing nonessential motion while keeping gameplay and state changes understandable.

## Personalize the page

- Edit the visible title, instructions, and other page copy in `index.html`. Keep the score and level displays consistent with the instructions shown to players.
- Inspect `index.html` for the existing style rules before changing colors, typography, or layout; no separate stylesheet is listed in the project files.
- The page links to externally hosted Inter and Space Grotesk font stylesheets. Preserve those links if you want to retain the current font choices.
- Before moving or renaming anything, check `index.html` for local `href` and `src` references and keep their relative paths valid. No separate local asset files are listed.