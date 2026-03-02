# Bicycle Animation

A bicycle-riding animation built with the HTML5 Canvas API.  
A stick-figure cyclist rides from **"Hard Work"** to **"Success"**, ending with a motivational message.

## How to Run

Open `Bicycle Animation/index.html` in any modern browser and click **Start**.

## Project Structure

```
Bicycle Animation/
├── index.html                  ← entry point (hash-based routing)
├── css/
│   └── styles.css              ← all styling
└── js/
    ├── app.js                  ← routing & UI event handling
    ├── AnimationController.js  ← animation phases & timing
    ├── Bicycle.js              ← bicycle frame, wheels, drivetrain
    ├── Rider.js                ← stick-figure rider & pedalling
    └── Scene.js                ← background, labels, messages
```

## Features

- **Start / Rerun** buttons with hash-based routing (`#/`, `#/animation`)
- Two-phase animation: plain sketch → colourful styled ride
- Motivational "hard work → success" theme
- Clean OOP structure — easy to extend (slopes, obstacles, etc.)
- `requestAnimationFrame` with frame-rate throttling

## Customisation

Edit the constants at the top of `js/Scene.js` to change the displayed messages:

```js
const PHASE1_LEFT_TEXT  = 'HARD WORK';
const PHASE1_RIGHT_TEXT = 'SUCCESS';
const PHASE2_HEADING    = 'SUCCESS';
const FINAL_MESSAGE     = "Hard work beats talent when talent doesn't work hard!";
```
