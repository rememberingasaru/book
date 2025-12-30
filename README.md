# PDF Book Viewer

A static, browser-based PDF viewer optimized for reading books. Features a realistic flipbook mode, continuous scrolling, print-bleed removal, and offline-capable PWA-style caching. Built with Vanilla JS, Mozilla PDF.js, and StPageFlip.

## Features

-   **Dual Modes**: Flipbook (spread view) and Vertical Scroll.
-   **Smart Cropping**: Removes print bleed/margins dynamically.
-   **Deep Linking**: Share exact page and view settings via URL.
-   **Privacy**: 100% Client-side; no servers.
-   **Mobile First**: Responsive design with touch support.

## Setup & Deployment (GitHub Pages)

1.  **Repository Setup**:
    -   Ensure this folder is a git repository.
    -   Place your PDF file at the root as `book.pdf`.

2.  **Enable GitHub Pages**:
    -   Push this code to GitHub.
    -   Go to **Settings** > **Pages**.
    -   Source: `Deploy from a branch`.
    -   Branch: `main` (or master) / folder: `/(root)`.
    -   Save.

3.  **Usage**:
    -   Visit your provided GitHub Pages URL.
    -   Settings panel allows adjusting crop (bleed removal).

## Configuration

Modify `assets/app.js`:

```javascript
const CONFIG = {
    pdfPath: '/book.pdf', // Path to your PDF file
    minZoom: 0.5,
    maxZoom: 3.0,
    baseScale: 1.5, // Increase for sharper text (costs performance)
};
```

## Credits

-   [PDF.js](https://mozilla.github.io/pdf.js/) by Mozilla
-   [StPageFlip](https://nodlik.github.io/StPageFlip/) by Nodlik
