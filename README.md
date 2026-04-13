# Xianix Website

The product website for **Xianix** — an AI-Driven Lifecycle (AI-DLC) agent platform built by [99x](https://99x.io). The site introduces the Xianix agent team, explains the shift from traditional Agile to AI-DLC, and covers pricing and enterprise options.

## About

This is a simple static website built with plain HTML and CSS — no frameworks, no build steps, no dependencies. It can be served directly from the filesystem or with any basic web server.

## Running locally

Because the site is plain HTML/CSS with no build process, you can open it using any of the following methods:

### IDE live server

Most modern editors have a built-in or extension-based live server:

- **VS Code / Cursor** — Install the [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) extension, then right-click `index.html` and select **Open with Live Server**.
- **WebStorm / IntelliJ** — Open `index.html` and click the browser icon in the top-right corner of the editor.

### Simple HTTP servers

Run one of these from the project root:

```bash
# Python (built-in)
python3 -m http.server 8000

# Node.js (npx, no install needed)
npx serve .

# PHP (built-in)
php -S localhost:8000
```

Then open [http://localhost:8000](http://localhost:8000) in your browser.

### Open the file directly

You can also just open `index.html` directly in a browser. Note that some icon rendering (Lucide via CDN) requires a network connection.

## Project structure

```
.
├── index.html          # Main page
├── style.css           # All styles
├── img/                # Images and logos
│   ├── 99xlogo.svg
│   ├── aidlc.png
│   ├── aidlc-redesigned.png
│   └── legacy-agile.png
└── .github/
    └── workflows/
        └── deploy.yml  # GitHub Pages deployment
```

## Deployment

The site is automatically deployed to GitHub Pages via the workflow in `.github/workflows/deploy.yml` on pushes to the main branch.
