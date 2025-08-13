# 🎩 Animated GIF Puzzle Boxes

A small HTML + CSS + JavaScript project that takes an animated GIF, splits it into a grid of small boxes, and reassembles them to display the full animation — like a moving jigsaw puzzle.

---

## 📌 How It Works

### 1. HTML — The Stage
The HTML provides an empty container (`#boxes`) for our boxes and a button to trigger effects.
### 2. CSS — Styling the Boxes
We style each .box so it:

Uses the same animated GIF as its background.

Shows only part of the GIF by adjusting background-position.

Has a fixed size of 125×125px.

Is set up to be arranged in a grid.
### 3. JavaScript — Building the Puzzle
JavaScript dynamically creates 4×4 = 16 boxes, each showing a different part of the GIF.
Here’s the trick:

-j * 125px → shifts the background left to show the correct column.

-i * 125px → shifts the background up to show the correct row.

Put together, all 16 boxes display different parts of the GIF, forming the full animation.

### 4. Why the Animation Still Works
Even though we split the GIF visually:

All .box elements use the same GIF file.

Browsers animate all instances of the GIF in sync.

The result: a perfectly synced animated “puzzle” effect.

### 🛠️ How to Run
Clone or download the project.

Open index.html in your browser.

Watch the animated puzzle come to life!
