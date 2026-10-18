# Solve My Cube

Interactive 3D website that teaches extreme beginners to solve a 3x3 Rubik's Cube with the layer-by-layer (daisy) method.

**v1**
- **Learn:** an intro lesson ("Meet your cube") plus 7 stages: daisy, white cross, white corners, middle layer, yellow cross, yellow face, finish the last layer. Each stage shows the goal, demos its algorithm on the 3D cube, then walks through a real example scramble step by step. You can **Watch** (animated, with a pink arrow and plain-language captions like "Right ↑") or **Try it** (you swipe the cube yourself; wrong moves are undone automatically).
- **Play:** a free virtual cube. Swipe stickers to turn layers, scramble at five difficulty levels (Tiny 3 moves → Full 25 moves), undo, and a timer that starts on your first turn and stops when the cube is solved.
- **Timer:** time solves on your real cube, with scrambles, best time, average of 5 and average of 12.
- Lesson progress, times and settings are saved in this browser (localStorage). Standard move letters (R U R′ U′) can be switched on in Settings. Light and dark themes.

The example solutions come from a built-in solver that follows the same beginner method, so every step on screen is something a beginner would actually do.

## Run it

It's a single page with no build step. Open `index.html` in a browser, or serve the folder:

```
python3 -m http.server 8000
```

Three.js 0.160 loads from the jsDelivr CDN, so you need an internet connection. To host it, turn on GitHub Pages for the `main` branch (root folder).

## Roadmap (v2)

- Scan your own cube with the phone camera, with tap-to-fix for misread stickers (plus manual entry)
- Coach mode: solve your real cube step by step with the same method
- Mistake recovery: "go back one move" and "I messed up, rescan"
