# FieldPay Solutions — Website

Single-page marketing website for FieldPay Solutions LLC, an ag-tech platform built for farm labor contractors.

**Tagline:** From the field to the family. Payroll for the people who feed America.

## About FieldPay Solutions

FieldPay Solutions is a two-app platform for farm labor contractors:

- **FieldPay** — Mobile time, attendance, and data collection app for crew leaders and field supervisors.
- **ERP Suite by FieldPay Solutions** — Full HRIS and ERP platform for the back office.

The platform handles H-2A compliance, multi-state payroll, AEWR calculations, housing registries, farm invoicing, tax compliance, and financial automation.

## Structure

This is a single HTML file (`index.html`) plus an `images/` folder. No build step, no dependencies — just open it in a browser.

Fonts: **Cormorant Garamond** (display) + **Outfit** (body), loaded from Google Fonts.

## Files

```
fieldpay-website/
├── index.html
├── README.md
└── images/
    └── fieldpay-logo.png
```

## Deployment to GitHub Pages

1. Create a new GitHub repository (suggested name: `fieldpay-website` or `fieldpaysolutions`)
2. Upload `index.html`, `README.md`, and the `images/` folder to the repo
3. Go to **Settings → Pages**
4. Under **Source**, select **Deploy from a branch**
5. Choose `main` branch and `/ (root)` folder
6. Click **Save**
7. Wait 1–2 minutes — site will be live at `https://[username].github.io/[repo-name]/`

## Connecting a Custom Domain (e.g. fieldpaysolutions.com)

When ready to connect a custom domain via GoDaddy or another DNS provider:

1. In your DNS settings, add these records:
   - `A` records pointing `@` to the four GitHub Pages IPs:
     - `185.199.108.153`
     - `185.199.109.153`
     - `185.199.110.153`
     - `185.199.111.153`
   - `CNAME` record pointing `www` to `[username].github.io`
2. In the GitHub repo, go to **Settings → Pages**
3. Under **Custom domain**, enter your domain and save
4. Check **Enforce HTTPS** once the certificate provisions

## Customization Notes

The current site uses placeholder values for:
- **Email** — currently `info@fieldpaysolutions.com`
- **Phone** — not currently displayed (can be added if desired)

The form is currently a JavaScript alert demo — to make it functional, integrate with a service like Formspree, Netlify Forms, or a custom backend.

---

© 2026 FieldPay Solutions LLC. All rights reserved.
