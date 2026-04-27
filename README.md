# Phish or Legit? - Phishing Awareness Game

A small browser game that helps users practice spotting phishing emails.

Players review example emails and classify each one as **Phish** or **Legit**. After each answer, the game shows immediate feedback, red flags, and a short safety tip.

## Features

- Start screen and guided game flow
- 6 email scenarios (mixed phishing and legitimate examples)
- Instant feedback after each guess
- Red-flag breakdown for phishing samples
- End-of-game score summary and replay
- Mobile-friendly single-page layout

## Tech Stack

- HTML/CSS/JavaScript (vanilla)
- Webpack 5
- webpack-dev-server
- html-webpack-plugin
- copy-webpack-plugin

## Project Structure

```text
email_phish/
  index.html               # Main app UI and game logic (inline script)
  js/
    app.js                 # Webpack entry file (currently empty)
    vendor/
  css/
    style.css
  img/
  webpack.common.js
  webpack.config.dev.js
  webpack.config.prod.js
  package.json
```

## Getting Started

### 1) Install dependencies

```bash
npm install
```

### 2) Run in development mode

```bash
npm run start
```

This starts the webpack dev server and opens the app in your browser.

### 3) Create a production build

```bash
npm run build
```

Production files are generated in `dist/`.

## Available Scripts

- `npm run start` - run local development server
- `npm run build` - build production bundle into `dist/`
- `npm test` - placeholder script (not implemented yet)

## Notes

- Most game logic is currently inside `index.html`.
- `js/app.js` is defined as the webpack entry point but is empty right now.
- If you plan to extend the game, a good next step is moving inline JavaScript from `index.html` into `js/app.js`.

## License

See `LICENSE.txt`.

