# void-run

**VOIDRUN** is a canvas survival game about dodging pursuing glitches and pruning them with ink trails. Move to set your target; while moving during play, draw trails to cut weeds. A weed is removed when its hit points are depleted, increasing the pruned count and growing a plant at its position. Weeds pursue the player, can wind up and dash, may split when pruned, and can damage plants. Being caught ends the run.

## Play locally

Open `index.html` in a browser, or start a local server from the project folder:

```sh
python -m http.server 8000
```

Then visit <http://localhost:8000>.

## Controls and progression

Pointer movement sets the player’s target and, during play or a level transition, creates trail segments; releasing the pointer stops drawing. Space or Enter starts or restarts a run, as does clicking or tapping the start/game-over overlay. The HUD shows the current level, progress toward its pruning goal, and an ink meter.

Ink holds up to 100 units. Drawing drains 58 units per second; not drawing regenerates 32 per second. Trail segments expire after 0.75 seconds, with at most 600 segments kept. Use drawing deliberately: running out of ink limits the ability to cut weeds until it regenerates.

The first level requires pruning 8 weeds; the goal increases by 4 for each level. Meeting it advances the level, clears weeds and pending spawns, and restores up to 55 ink. The game-over screen reports the run’s pruned total, level reached, and best run.

## Storage and browser behavior

The best total is stored as `voidrun.best.v1` in localStorage. If storage access fails, the game uses an in-memory fallback, which does not survive a page reload. When the document becomes hidden during play, the game clears active weeds and pending spawns and grants 1.4 seconds of grace with a toast; it does not pause the run. Keep this behavior in mind when switching tabs.

Plants, weeds, stars, trails, and effects are generated or drawn in the browser; there are no external image assets or gameplay API calls in the source. Audio is generated with the Web Audio API, and pruning or dying can trigger `navigator.vibrate` where available. Canvas scaling adapts to the viewport and caps device-pixel ratio at 3. Inter and Space Grotesk load from jsDelivr’s Fontsource CDN. No build step is documented.