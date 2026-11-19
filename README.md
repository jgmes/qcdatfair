# QCD at FAIR — Astro website

A responsive, multi-page Astro starter site for the QCDatFAIR initiative. It is intentionally static and dependency-light.

## Run locally
```bash
npm install
npm run dev
```
Then open the local URL printed by Astro.

## Build
```bash
npm run build
npm run preview
```

## Deploy to GitHub Pages
1. Create a GitHub repository and push the contents of this folder to its root.
2. In `astro.config.mjs`, set `site` to your public domain. If deploying to `https://USER.github.io/REPO/`, also set `base: '/REPO'`.
3. In GitHub: **Settings → Pages → Build and deployment → GitHub Actions**.
4. Add `.github/workflows/deploy.yml` (or use the included workflow) and push to `main`.

For a custom domain such as `qcdatfair.eu`, configure DNS at your provider and add a `public/CNAME` file containing the domain.

## Content to customise
- `src/pages/index.astro`: homepage narrative and featured science.
- `src/pages/science.astro`: research themes.
- `src/pages/facilities.astro`: facility and experiment overview.
- `src/pages/community.astro`: collaboration and participation.
- `src/pages/resources.astro`: publications and links.
- `src/pages/contact.astro`: replace the placeholder contact address.
- `src/styles/global.css`: visual identity, colours, typography and layout.

The initiative description and research topics are based on the QCDatFAIR White Paper, *Hadron Physics Opportunities at FAIR*, arXiv:2512.15986. Please review all institutional wording, timelines and contact details before publishing.

## Logo and scientific content
The supplied QCD at FAIR logo (`public/images/qcdatfair-logo.png`) is used in the site header and footer. Slide photographs, plots, and other extracted presentation images have been removed. The science page retains text-only summaries of selected physics opportunities, with attribution to the DPG 2026 presentation.

- `public/images/qcdatfair-framework.png`: central QCDatFAIR framework diagram supplied for the website. It is featured prominently on the homepage.

## Dark-theme artwork
The supplied QCDatFAIR logo has a transparent background and a light wordmark for the dark navy header/footer. The central framework diagram has been adapted for dark presentation: white canvas areas are transparent and dark typography is lightened while its coloured research domains are retained. The figure is shown on a deep teal/navy panel.

## Contact and presentations
The public contact page lists info@qcdatfair.eu as the initiative contact. The Resources page includes selected talks and workshops linked to their public Indico/conference pages; availability of slide files depends on the event organisers.

## Community contribution portal
A dedicated `/contribute/` page invites community members to submit talks, publications, and workshops by email to info@qcdatfair.eu. This is intentionally a curated email workflow rather than an automated public upload or publishing form; submissions are reviewed before appearing on the site.

## Password-protected introduction
The site displays a QCD at FAIR welcome screen and asks for the password `atgsi` before showing the website. Successful access is remembered in the browser's localStorage. This is a lightweight visitor gate only: because Astro is deployed as a static site and the password check runs in client-side JavaScript, it is not secure access control and does not protect the underlying pages or assets from someone who inspects the source. Do not use it for confidential content.


## GitHub Pages deployment

Configured for https://jgmes.github.io/qcdatfair/ using Astro `base: "/qcdatfair/"`. No custom domain or CNAME is required.
