# Coloring Book

A tiny, ad-free coloring book web app. Load any image, it becomes an outline drawing, tap regions to color them. Everything runs locally in the browser: one HTML file, no dependencies, no network.

## Usage

Open `index.html` in a browser, or serve the folder (e.g. `python -m http.server`) and open it on your tablet.

- **Load an image:** "Open image", drag & drop, or paste from the clipboard. A sample drawing loads at startup.
- **Paint:** pick a color from the palette (or the full color picker) and tap a region to fill it.
- **Pick:** switch to the 💧 tool and tap a region to take its color; the app then returns to Paint.
- **Undo / redo:** 60 steps, via buttons or Ctrl+Z / Ctrl+Y.
- **Zoom / pan:** pinch and drag on a tablet, mouse wheel and drag on desktop. "Fit" resets the view.
- **Save PNG:** exports the colored picture with outlines.

## Tuning the drawing

Under "⚙ Drawing":

- **Detail:** how many edges are picked up.
- **Line thickness:** bolder outlines; also closes small gaps that let color leak.
- **Simplify:** merges tiny areas into their neighbors (useful for photos).

Changing a slider regenerates the drawing and clears your colors. Simple images, cartoons and line art work best; photos need some tuning.

## Notes

Progress is not saved between sessions.
