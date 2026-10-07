[![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
# HTML Landing Page

A responsive landing page, originally built for GitLab Pages.

> **Note:** this repository's page file is named `README.md` but contains
> an HTML document. Rename it to `index.html` to serve it directly.

## Table of contents

- [Requirements](#requirements)
- [Usage](#usage)
- [Deployment](#deployment)
- [Accessibility](#accessibility)
- [License](#license)

## Requirements

A modern web browser. No build step, no dependencies, no server required.

## Usage

```bash
git clone https://github.com/the-jodingo/html-file.git
cd html-file
python3 -m http.server 8000
```

Open <http://localhost:8000>. You can also open `index.html` directly.

## Deployment

Any static host works — Netlify, GitHub Pages, Cloudflare Pages, S3, or nginx.
The page is a single file with no build step, so you can drag the folder in.

## Accessibility

- semantic landmarks and a logical heading order
- all text meets WCAG AA contrast
- keyboard-navigable, with visible focus states
- responsive layout, usable from 320 px wide
- CI runs an axe-core scan and HTML validation on every push

## License

[MIT](LICENSE) © Joash Odingo
