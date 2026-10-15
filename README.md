# Debt Tracker

A calm, single-page web app for tracking paying off one total debt. No frameworks, no backend, no build step. Everything is saved in your browser.

## Features

- **The big number:** what you still owe, front and center
- **Log a payment:** type an amount and the total counts down
- **Payment history:** every payment with its date and time; remove one logged by mistake
- **Sound:** a soft chime on each payment (can be turned off)
- **Zero celebration:** confetti and a bigger sound when you hit $0.00
- **Saves automatically:** your total and history stay in `localStorage` between visits
- Progress bar, edit the starting amount (typos or interest), dark mode, works offline

## Use it

**Online (GitHub Pages):** In your repo, go to **Settings → Pages**, set **Source** to *Deploy from a branch*, pick `main` and `/ (root)`, and save. The app will be live at `https://<your-username>.github.io/<repo-name>/` in a minute or two.

**Locally:** Download `index.html` and open it in Chrome, Safari, Edge or Firefox.

## Privacy

Your numbers never leave your browser. Nothing is sent to a server. Data is stored per browser and per site, so the GitHub Pages version and a local copy keep separate histories, and clearing your browser data erases it.

## Tech

One file, `index.html`, with inline HTML, CSS and JavaScript:

- Money is stored as whole cents to avoid rounding errors
- Sounds are made with the Web Audio API, so there are no audio files
- Confetti is drawn on a plain `<canvas>`, with no library
- Respects `prefers-reduced-motion` and `prefers-color-scheme`

## License

MIT. See [LICENSE](LICENSE).
