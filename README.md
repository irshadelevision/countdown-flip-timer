# Countdown Flip Timer

A lightweight, browser-based countdown timer with a flip-card animation effect for hours, minutes, and seconds.

## Demo

Open `index.html` in your browser to run the timer.

## Features

- 24-hour countdown target (from page load time)
- Flip animation for each changing digit
- Separate hour, minute, and second segments
- No build step or dependencies required

## Tech Stack

- HTML
- CSS
- Vanilla JavaScript

## Project Structure

```text
countdown-flip-timer/
├── index.html   # Markup for timer UI
├── styles.css   # Flip-card styles and animations
├── script.js    # Countdown logic and digit flipping
└── LICENSE      # Project license
```

## How It Works

1. The timer target is set to 24 hours from the current time.
2. Every 250ms, the remaining time is recalculated.
3. Hours, minutes, and seconds are split into digits.
4. Each digit updates with a flip animation when its value changes.

## Run Locally

1. Clone or download the repository.
2. Open `index.html` in any modern browser.

## Customization

- Change countdown length in `script.js`:
  - `new Date().setHours(new Date().getHours() + 24)`
  - update frequency by changing the `250` value in `setInterval(..., 250)`
- Adjust animation speed in `styles.css`:
  - `flip-top` and `flip-bottom` keyframe durations
- Update colors and typography in `styles.css`.

## Browser Support

Works in modern browsers that support:

- CSS keyframe animations
- ES6 JavaScript features
- DOM APIs used for element creation and events

## License

This project is licensed under the terms in the `LICENSE` file.
