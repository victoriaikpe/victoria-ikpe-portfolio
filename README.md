# Victoria Ikpe — Sales Portfolio

A complete responsive sales portfolio with two visual directions:

- **Premium editorial portfolio:** `index.html` — elegant green palette, editorial typography, skills, experience, results, sales samples and contact.
- **Corporate SaaS portfolio:** `saas.html` — product-led layout for SaaS teams, concise capabilities, metrics and experience.

## Files

- `index.html`, `style.css`, `script.js` — premium portfolio
- `saas.html`, `saas.css`, `saas.js` — alternate SaaS-style version
- `api/contact.js` — Vercel serverless endpoint that securely sends contact messages through Resend
- `assets/images/profile-placeholder.svg` — labelled illustration; no portrait photo was supplied
- `assets/icons/favicon.svg` — brand favicon
- `.nojekyll` — GitHub Pages compatibility

## Preview and deployment

GitHub Pages can serve the static portfolio and alternate design at:

- `https://victoriaikpe.github.io/victoria-ikpe-portfolio/`
- `https://victoriaikpe.github.io/victoria-ikpe-portfolio/saas.html`

The GitHub Pages static site cannot run the `api/contact.js` backend. To enable server-side email, deploy the same repository on Vercel (the `/api/contact.js` file follows Vercel's Node serverless function convention), then configure these project environment variables in Vercel:

- `RESEND_API_KEY` — secret API key from your Resend account; store only in the hosting dashboard, never in browser code or Git.
- `CONTACT_FROM` — sender address verified with Resend, e.g. `Portfolio <portfolio@your-verified-domain.example>` (replace with an address on a domain you control and have verified).
- `CONTACT_TO` — recipient email; defaults to `victoriaikpe88@gmail.com` if omitted.

Redeploy after adding environment variables. The form posts to `/api/contact`; therefore use the Vercel-hosted URL (or a custom domain pointed to Vercel) for the working backend. On GitHub Pages the static site remains viewable, but `/api/contact` is not available; visitors still have the direct email link as an alternative. No email credentials are included in this repository.

## Add Victoria's real portrait later

No photo was attached, so the site uses a clearly labelled, non-photographic placeholder. When Victoria provides an approved portrait, upload an optimized JPG or WebP to `assets/images/` and change the placeholder `img` source in both `index.html` and `saas.html` to that exact image path. Keep a descriptive alt text. A square or portrait crop around 900 × 1100 pixels is suitable; export an optimized WebP/JPG.

## Contact

- Email: victoriaikpe88@gmail.com
- LinkedIn: https://www.linkedin.com/in/victoria-ikpe-72a877412/

Content and achievements follow the supplied brief; the listed tools are not accompanied by unconfirmed certification or proficiency claims.


