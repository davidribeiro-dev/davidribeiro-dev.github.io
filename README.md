# davidribeiro - portfolio site

![Website](https://img.shields.io/website?down_color=red&down_message=offline&up_color=brightgreen&up_message=live&url=https%3A%2F%2Fdavidribeiro-dev.github.io)
![License](https://img.shields.io/badge/license-All%20Rights%20Reserved-red)
![Last Commit](https://img.shields.io/github/last-commit/davidribeiro-dev/davidribeiro-dev.github.io)
![Top Language](https://img.shields.io/github/languages/top/davidribeiro-dev/davidribeiro-dev.github.io)

This is the source code for [davidribeiro-dev.github.io](https://davidribeiro-dev.github.io/) — a static personal portfolio website built from scratch and hosted on GitHub Pages.

The site presents selected projects, earned certifications, and contact information for David Ribeiro, a CIS student at Blue Hills Regional Technical School pursuing IT and cybersecurity internships.

## Copyright and License Information

All source code, content, design, and assets in this repository are © 2025–2026 David Ribeiro. All rights reserved. See [License](#license) below for full details.

## Contents

- [Overview](#overview)
- [Site Sections](#site-sections)
- [Tech Stack](#tech-stack)
- [Project Structure](#project-structure)
- [Local Development](#local-development)
- [Deployment](#deployment)
- [Status](#status)
- [Acknowledgements](#acknowledgements)
- [License](#license)

## Overview

The site is a single-page application written in HTML, CSS, and vanilla JavaScript. It uses no frameworks, no build pipeline, and no preprocessors. Styling is handled by a single hand-written stylesheet (`css/style.css`); interactive behavior is implemented in inline scripts within `index.html`.

The design is desktop-first. Layout, navigation, and animations are tuned for screens 1024 px wide and larger.

## Site Sections

The site is divided into the following sections, navigable via anchor links in the top menu:

1. **Home** — landing hero with name, brief tagline, and a downloadable academic résumé.
2. **About** — short biography, current education at Blue Hills Regional Technical School, and a list of personal interests.
3. **Projects** — a grid of three featured project cards, each with a description, image, and reference notes:
   - *Pi Game 3.0* — Unity / C# multiplayer game (3D physics, grappling mechanics)
   - *Arduino Automation Program* — C++ automation for bulk Chromebook OU enrollment
   - *WLAN Network Configuration* — Cisco Packet Tracer lab covering WPA2, SSIDs, and VLAN segmentation
4. **Certifications** — a grid of six earned credentials: CompTIA ITF+, ITS Device Configuration & Management, ITS Cybersecurity, Google Cybersecurity, ITS Networking, and Cisco CCNA: Introduction to Networks. Includes a link to the full certifications repository.
5. **Contact** — personal and academic email addresses.

## Tech Stack

| Layer        | Technology                                                          |
| ------------ | ------------------------------------------------------------------- |
| Markup       | HTML5                                                               |
| Styling      | CSS3 (single stylesheet, no preprocessor)                           |
| Scripting    | Vanilla JavaScript (inline in `index.html`)                         |
| Typography   | [Google Fonts — Poppins](https://fonts.google.com/specimen/Poppins) |
| Icons        | [Font Awesome 4.7](https://fontawesome.com/v4.7/icons/)             |
| Hosting      | GitHub Pages                                                        |
| Build system | None                                                                |

## Project Structure

```
davidribeiro-dev.github.io/
├── css/
│   └── style.css           # Site-wide stylesheet
├── images/                 # Project thumbnails, logo, profile image
├── js/
│   └── scripts.js          # Reserved — interactive logic currently inlined in index.html
├── pages/
│   └── resume.html         # Reserved — placeholder for future résumé page
├── pdf/
│   └── Academic Resume.pdf # Downloadable résumé linked from the hero
├── index.html              # Single-page application entry point
└── README.md               # This file
```

## Local Development

The site is fully static and requires no installation, build, or compilation step.

### Option 1 — Open `index.html` directly

```bash
git clone https://github.com/davidribeiro-dev/davidribeiro-dev.github.io.git
cd davidribeiro-dev.github.io
# Then open index.html in your browser
```

This works for all sections except for the résumé download, which requires the file to be served over HTTP.

### Option 2 — Run a local HTTP server

For full fidelity to the production environment, serve the directory over a local web server.

Using Python's built-in server:

```bash
python -m http.server 8000
```

Using Node.js:

```bash
npx http-server -p 8000
```

Then open [http://localhost:8000](http://localhost:8000) in any modern browser.

## Deployment

Deployment is handled automatically by **GitHub Pages**. Any commit pushed to the `main` branch is published to the live site within approximately one minute.

The live URL is:

> [https://davidribeiro-dev.github.io/](https://davidribeiro-dev.github.io/)

GitHub Pages configuration can be reviewed in **Repository Settings → Pages**.

## Status

The site is **active**. Structure and styling are stable; content is updated as new projects ship and new certifications are earned. The site is currently desktop-first.

## Acknowledgements

This site uses the following open-source resources:

- [Google Fonts — Poppins](https://fonts.google.com/specimen/Poppins) by Indian Type Foundry, distributed under the [SIL Open Font License 1.1](https://scripts.sil.org/OFL).
- [Font Awesome 4.7](https://fontawesome.com/v4.7/icons/) — icons under [SIL OFL 1.1](https://scripts.sil.org/OFL), CSS under [MIT](https://opensource.org/license/mit).

The *"How to Make Grappling Gun in Unity"* tutorial by **DanisTutorials** and the **Cisco NetAcad CCNA: Switching and Wireless Essentials** curriculum are referenced in specific project descriptions on the site.

## License

All source code, content, and design assets in this repository are © 2025–2026 David Ribeiro. All rights reserved.

This repository is published publicly for portfolio and recruiting purposes only. No license is granted to copy, modify, redistribute, or use any portion of this code or its assets without prior written permission.
