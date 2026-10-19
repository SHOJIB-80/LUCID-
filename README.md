# LUCID-

Preview link - https://shojib-80.github.io/LUCID-/

---

## Overview

This project is a static, responsive one-page landing theme named "LUCID" built with HTML, CSS and JavaScript. The system provides a ready-made landing page template with animated sections for features, device previews, pricing tables, testimonials, contact form (static), and interactive visual effects (particles and water ripple). The project is intended to be deployed as a static site (for example via GitHub Pages) or served from any static web host.

## Features

- Responsive one-page landing layout (header, feature sections, device section, details, testimonials, pricing, contact, map, footer)
- Animated entrance effects using WOW.js and AOS
- Particle background support (particles.js)
- Water ripple effect support (jquery.ripples) for demo sections
- Testimonials carousel using Owl Carousel
- Animated counters (counterUp)
- Preloader and scroll-to-top progress indicator
- Pricing sections with counters and order buttons (static)
- Contact form markup (no backend action provided)

## Technology Stack

| Technology | Purpose |
|---|---|
| HTML | Static page structure (index.html and demo pages) |
| CSS | Styling (css/style.css, css/media.css, animate.css, owl carousel themes) |
| JavaScript | Client-side interactivity and animations (jQuery, plugins) |
| Bootstrap 5 | Responsive layout and components |
| jQuery plugins | Owl Carousel, ripples, particles.js, counterUp, WOW.js, AOS |

## Project structure

```
LUCID-/
├── Counter-Up-master/                      # vendor/demo or plugin files for counterUp
├── WOW-master/                             # vendor demo files for WOW.js animations
├── auto-hiding-sticky-navbar/              # vendor/demo for sticky navbar behavior
├── jQuery-Plugin-For-Water-Ripple-Animation-ripples/  # jquery.ripples plugin & demo
├── particles.js-master/                    # particles.js library demo files
├── css/                                    # project styles (style.css, media.css, animate.css, owl carousel css)
├── images/                                 # image assets used by the template
├── js/                                     # JS plugins and initialization scripts (owl, wow, particles, ripples, counterUp)
├── index.html                              # main one-page landing HTML
└── README.md                               # this file
```

Notes:
- index.html is the single-page entry point that wires all styles and scripts.
- The repository includes several third-party/demo packages (particles.js, ripples, WOW, Counter-Up, etc.) under top-level directories.

## How the system fits together

The application is a static site. At runtime the browser loads index.html and fetches static assets from css/, js/, and images/. JavaScript initializes visual plugins (particles, ripples, carousel, counters) to produce interactive effects on the client. There is no server-side code, database, or API implemented in this repository.

## How to run

Serve the site locally or open the page directly in a browser.

From a clone you can run a simple static server (recommended to avoid mixed-content or CORS issues with some plugins):

```bash
# from repository root
# using Python 3
python -m http.server 8000
# open http://localhost:8000/index.html in a browser
```

Or simply open index.html in any modern browser.

## Configuration

No environment files or server configuration are required. All behavior is driven from index.html and the static assets in css/ and js/.

## Database

This project does not use a database. All content is static HTML and assets.

## Contact form and external integrations

The contact form exists in the markup but has no server-side handler (the form `action` attribute is empty). The Google Map is embedded via an iframe in the map section. No API keys or server integrations are present in this repository.

## Demo & Vendor pages

The repository includes demo/example pages for included third-party libraries under their respective folders (for example the ripples demo under `jQuery-Plugin-For-Water-Ripple-Animation-ripples/` and the particles demo under `particles.js-master/`). These demos are standalone examples of the plugins used on the main page.

## Application usage

- Open the landing page (index.html) in a browser.
- Use the navigation at the top to jump to sections (Home, Features, About, Testimonials, Pricing, Contact).
- The testimonials section is an Owl Carousel instance; pricing counters animate using the counterUp plugin.
- The contact form fields are static; pressing SEND submits nothing by default.
- Visual effects (particles and ripples) are initialized via the scripts included at the end of index.html.

## API

There are no application APIs exposed by this repository.

## Authentication and authorization

This project does not implement authentication or authorization.

## Testing

There are no automated tests in this repository.

## Known limitations

- Static template only: the contact form has no backend and will not send messages as-is.
- Several text blocks contain placeholder text (Lorem ipsum) and demo content (example client names/images).
- Some third-party demo directories are included verbatim; they may contain their own licensing and example files.

## Security considerations

- This is a static front-end template. Any production use that accepts user input (e.g., a contact form) requires adding a secure, server-side handler and input validation.
- Do not embed secrets or API keys in static files; none are present in this repository.

## License

Copyright (c) SHOJIB-80

All rights reserved. This project is provided under the copyright of the repository owner (SHOJIB-80).

## Author

SHOJIB-80

---

Preview link - https://shojib-80.github.io/LUCID-/
