# Gen AI

Gen AI is a free, open-source, browser-local text model chat experience. It runs in the browser, needs no account, and requires no backend. It is designed for text generation and next-token prediction, not web research.

## Live site

This repository is ready to publish as a static GitHub Pages site.

1. Open the repository settings.
2. Select Pages.
3. Set Source to: Deploy from a branch.
4. Select the `main` branch and the `/ (root)` folder.
5. Save.
6. Your public page will be available at:
   `https://<username>.github.io/gen-ai/`

## Features

- No account creation
- No backend required
- Runs directly in the browser
- Uses WebGPU when available, with CPU fallback for compatibility
- Local-only text generation
- Model selection: Gen 1.0 FAST and Gen 1.0 Thinking
- Works on mobile and desktop with browser support checks

## Supported browsers

Best results on:
- Chrome / Edge on desktop and Android
- Safari on recent iPhones, iPads, and recent macOS

Compatibility notes:
- WebGPU must be available
- HTTPS is required for WebGPU in the browser
- GitHub Pages provides HTTPS automatically
- If WebGPU is unavailable, Gen AI falls back to CPU-based WASM inference

## Important note

This app is an open-source browser-native text generation interface. It does not browse the web or do research. It predicts text based on local model weights and inference in the user's browser.

## Open source

This project is intended to be free and open source. The repository is a static site and can be published as a public page without any server-side code.

## Local testing

Open `index.html` directly in a modern browser, or serve it locally with any static file server.

Example:

```bash
python -m http.server 8000
```

Then open:

```text
http://localhost:8000
```
