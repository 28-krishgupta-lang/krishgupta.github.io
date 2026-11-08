# Krish Gupta — Portfolio

A static portfolio site for GitHub Pages. The site is served directly from the repository root; there is no build step or package manager.

## Repository structure

```text
.
├── index.html                 # Main portfolio page, styles, and interactions
├── img/                       # Photos and project-study visuals used by index.html
├── files/                     # Downloadable PDF reports linked from the portfolio
├── features/
│   └── copilot/plans/          # Standalone feature page
└── README.md
```

## Run locally

Open `index.html` in a browser, or serve the repository root with any static HTTP server. Keep asset paths relative to the root page when changing the portfolio.

## Deployment

The site is compatible with GitHub Pages when Pages is configured to publish the repository root from the default branch.

## Maintenance notes

- Keep images and PDFs that are referenced by `index.html`; removing them can create broken links or images.
- Before deleting a file, search all HTML and scripts for its path. Some media is referenced from JavaScript data rather than markup.
- The portfolio currently loads GSAP and Lenis from CDNs, so those interactions require a network connection.
