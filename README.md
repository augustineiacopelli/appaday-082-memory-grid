# AppADay 082 &middot; Memory Grid

A tap-to-flip matching game. Turn cards two at a time to find every pair, with a live move counter and a timer tracking each run.

**Live:** https://augustineiacopelli.github.io/appaday-082-memory-grid/

**Portfolio:** https://augustineiacopelli.github.io/appaday/

## What it does

Memory Grid is the classic concentration game. Cards start face down. Tap one to flip it, then tap a second: if the symbols match, the pair locks in place; if not, both flip back. Clear the whole board and the game reports your time and moves, keeping your fastest run per difficulty.

## Play

Pick a difficulty, then flip pairs until the board is clear.

- **Easy** is a 4 by 4 grid of 8 pairs.
- **Medium** is a 4 by 6 grid of 12 pairs.
- **Hard** is a 6 by 6 grid of 18 pairs.

The timer starts on your first flip and stops when the last pair is found. Moves count each two-card attempt. Best times are saved on your device, one per difficulty. A sound toggle turns the generated flip and match tones on or off, and the choice is remembered.

## Notes

Single self-contained file of vanilla HTML, CSS, and JavaScript. No build step and no dependencies beyond Google Fonts (Fredoka). Card faces are drawn from Unicode symbols escaped in the source to keep the file ASCII-clean, so there is no image or dictionary payload. The flip and match sounds are generated with the Web Audio API rather than loaded from files. Layout scales from a 375px phone to a wide desktop, and card flips are disabled when the viewer prefers reduced motion. Best times and the sound preference are stored in `localStorage`, wrapped so a blocked store never breaks play.

Part of AppADay: one complete, functional, mobile-friendly web app shipped every day.
