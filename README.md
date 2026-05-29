# Ultra Health Care

Static website for [Ultra Health Care](https://ultrahealthcare.com.au), a bulk-billing medical centre in Cheltenham, Victoria. The site was exported from Webflow and is served as plain HTML, CSS, and JavaScript — no build step or backend required.

## Tech stack

- HTML pages exported from Webflow
- CSS (`css/ultra-health-care.webflow.shared.72e2ab2b5.css`)
- JavaScript (jQuery + Webflow runtime in `js/`)
- Google Fonts (Poppins) loaded from CDN

## Prerequisites

- A modern web browser
- A local HTTP server (recommended for development)

No Node.js, npm, or database setup is required to run the site.

## Running locally

From the project root:

```bash
cd ultra-health-care
```

Start a local server using one of the options below.

### Option 1: Python (recommended)

```bash
python3 -m http.server 8080
```

Open [http://localhost:8080](http://localhost:8080).

### Option 2: Node.js

```bash
npx serve .
```

Open the URL shown in the terminal (typically [http://localhost:3000](http://localhost:3000)).

Stop the server with `Ctrl+C`.

> **Tip:** Use a local server instead of opening `index.html` directly in the browser. Serving over HTTP avoids issues with asset paths and navigation between pages.

## Pages

| Page | Path |
|------|------|
| Home | `index.html` |
| About Us | `about.html` |
| Services | `services.html` |
| Contact | `contact.html` |
| Our Doctors | `doctors-templates/doctors-template-1.html` |

## Project structure

```
ultra-health-care/
├── index.html              # Homepage
├── about.html
├── services.html
├── contact.html
├── css/                    # Webflow stylesheets
├── js/                     # jQuery and Webflow scripts
├── images/                 # Logos, icons, and page assets
└── doctors-templates/      # Doctor profile pages
```

## External services

- **HotDoc** — Online appointment booking links to [HotDoc](https://www.hotdoc.com.au/medical-centres/cheltenham-VIC-3192/ultra-health-care/doctors)
- **Google Fonts** — Typography loaded at runtime
- **Webflow CDN** — Some icons and assets reference `cdn.prod.website-files.com`

## Deployment

This site can be deployed to any static hosting provider, for example:

- GitHub Pages
- Netlify
- Vercel
- AWS S3 + CloudFront
- Cloudflare Pages

Upload the project files as-is. No build command is needed.

## Notes

- The contact form on the homepage is static and does not submit to a backend in this repository.
- Content changes are typically made in Webflow and re-exported, or edited directly in the HTML files.
- Designed and developed by [Obsydian Technologies](https://obsydiantechnologies.com).
