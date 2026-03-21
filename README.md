# Calculator

A browser-based calculator with a dark, iOS-style layout. Built with plain HTML, CSS, and JavaScript—no build step or dependencies.

## Features

- **Arithmetic**: addition, subtraction, multiplication, and division
- **Decimal input** via the `.` key
- **Persistent display**: the current expression is saved in `localStorage` and restored when you reopen the page
- **Clear**: resets the expression and storage
- **Responsive layout**: smaller buttons and text on narrow screens (under 500px width)

## Project structure

| File            | Role                                              |
| --------------- | ------------------------------------------------- |
| `index.html`    | Markup, button grid, and script/style includes    |
| `Calculator.js` | Expression string, `updateCalculation`, display |
| `Calculator.css`| Layout, theming, and mobile breakpoints           |

## Deployment
Live at:

   ```

2. Optional: serve the folder with any static server if you prefer (for example `npx serve .` or Python’s `python3 -m http.server`).

## Usage

Click number and operator buttons to build an expression. Press **=** to evaluate it; the result becomes the new value you can continue from. **Clear** empties everything.

## Technical note

Evaluation uses JavaScript’s `eval()` on the built string. That is acceptable for a local, single-page toy app, but it would be unsafe if this pattern were reused with untrusted input on a server or in a shared environment.


