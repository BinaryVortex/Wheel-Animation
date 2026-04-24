# Wheel Animation

A small, visually pleasing wheel animation built with plain HTML, CSS and JavaScript.

![Preview](./Screenshot%202024-08-25%20201210.png)

## Demo

Open `index.html` in any modern browser to see the animation. No build step or dependencies required — this is a static demo.

If you prefer a local server:

- Python 3: `python -m http.server 8000`
- Node (serve): `npx serve .`

Then visit http://localhost:8000 in your browser.

## Features

- Pure HTML/CSS/JS implementation
- Procedurally generated spokes created by JavaScript
- Smooth, looping animation using CSS keyframes
- Easy to customize colors, spoke count and speeds

## How it works (short)

The page contains a single container element (`#app`) that the script populates with multiple `<i>` elements using the `render` function. Each spoke is styled using CSS custom properties (`--_bg`, `--_deg`, `--_del`) to set the color, rotation and animation delay. A CSS keyframe moves a small dot along each spoke, creating the wheel animation.

## Customize

- Change the number of spokes by editing the first argument to the `render` calls in `index.html`.
- Change colors by editing the color arguments passed to `render` (e.g. `#643A6B`).
- Tweak animation duration in the CSS (`@keyframes move` or the `animation` property on the pseudo-element).

## Files

- `index.html` — the demo and the source for the animation
- `Screenshot 2024-08-25 201210.png` — preview image used in this README

## License

This project is provided under the MIT License. Feel free to reuse and adapt.
