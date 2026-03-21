# 🔥 IgniShield Fire & Safety LLC — Dubai Landing Page

**Dubai's #1 DCD A+ Approved Fire & Safety Company**

A fully SEO-optimised, Vercel-ready static landing page for IgniShield — targeting high-intent fire and safety keywords across Dubai and the UAE.

---

## 🚀 Deploy to Vercel (3 Ways)

### Option 1 — Vercel CLI (Fastest)
```bash
# 1. Install Vercel CLI globally
npm install -g vercel

# 2. Login to your Vercel account
vercel login

# 3. From this project folder, deploy
cd ignishield
vercel

# 4. Follow prompts:
#    - Set up and deploy: Y
#    - Which scope: (your account)
#    - Link to existing project: N
#    - Project name: ignishield-fire-safety-dubai
#    - In which directory is your code located: ./
#    - Want to modify settings: N

# 5. Production deploy
vercel --prod
```

### Option 2 — GitHub + Vercel Auto-Deploy
```bash
# 1. Push to GitHub
git init
git add .
git commit -m "Initial deploy — IgniShield fire safety Dubai landing page"
git remote add origin https://github.com/YOUR_USERNAME/ignishield.git
git push -u origin main

# 2. Go to https://vercel.com/new
# 3. Import your GitHub repo
# 4. Vercel auto-detects static site:
#    - Framework Preset: Other
#    - Root Directory: ./
#    - Output Directory: public
#    - Build Command: (leave empty)
# 5. Click Deploy ✅
```

### Option 3 — Vercel Dashboard (No CLI)
1. Zip the entire `ignishield/` folder
2. Go to [vercel.com/new](https://vercel.com/new)
3. Drag & drop the zip file
4. Vercel auto-deploys in ~30 seconds ✅

---

## ⚙️ Vercel Configuration

`vercel.json` is pre-configured with:

| Setting | Value |
|---|---|
| Output directory | `public/` |
| Framework | Static (none) |
| Build command | None required |
| Clean URLs | `true` (no `.html` in URLs) |
| Trailing slash | `false` |
| Security headers | CSP, HSTS, XFO, XSS |
| Asset caching | 1 year immutable |
| HTML caching | 1hr browser / 24hr CDN |

---

## 🌐 Custom Domain Setup (ignishield.ae)

After deploy on Vercel:

1. Go to **Project → Settings → Domains**
2. Add `ignishield.ae` and `www.ignishield.ae`
3. Vercel shows DNS records — add to your domain registrar:

```
Type    Name    Value
A       @       76.76.21.21
CNAME   www     cname.vercel-dns.com
```

4. SSL certificate is **automatically provisioned** by Vercel ✅
5. Update these files once domain is live:
   - `public/index.html` → confirm `<link rel="canonical" href="https://ignishield.ae/">`
   - `public/sitemap.xml` → confirm all `<loc>` URLs use `https://ignishield.ae`
   - `public/robots.txt` → confirm `Sitemap:` URL

---

## 📁 Project Structure

```
ignishield/
├── public/                    # ← Vercel output directory
│   ├── index.html             # Main landing page (SEO optimised)
│   ├── 404.html               # Branded 404 error page
│   ├── sitemap.xml            # XML sitemap for Google Search Console
│   ├── robots.txt             # Search engine crawl rules
│   ├── manifest.json          # PWA web app manifest
│   ├── _headers               # Edge cache & security headers (fallback)
│   ├── _redirects             # URL redirect rules (fallback)
│   └── assets/
│       ├── favicon.svg        # SVG favicon (scalable, all devices)
│       ├── favicon-32.png     # 32×32 PNG favicon
│       ├── favicon-16.png     # 16×16 PNG favicon
│       ├── apple-touch-icon.png  # 180×180 iOS icon
│       ├── icon-192.png       # PWA icon 192×192
│       ├── icon-512.png       # PWA icon 512×512
│       └── og-image.jpg       # Open Graph image (1200×630)
├── vercel.json                # Vercel deployment config
├── package.json               # Project metadata + dev scripts
├── .gitignore                 # Git ignore rules
└── README.md                  # This file
```

---

## 🔍 SEO Overview

### Keywords Targeted

| Type | Keywords |
|---|---|
| **Primary** | fire and safety company in Dubai, fire fighting company in Dubai |
| **Longtail** | fire alarm system installation Dubai, fire sprinkler system Dubai, fire suppression system company Dubai, fire AMC annual maintenance contract Dubai, fire hydrant system installation Dubai, DCD approved fire contractor Dubai |
| **LSI / NLP** | FM200 fire suppression Dubai, Hassantuk fire alarm Dubai, Istifa certificate Dubai, Dubai Civil Defence fire compliance, clean agent fire suppression Dubai |
| **Service** | fire protection company Dubai, fire extinguisher company Dubai, fire safety inspection Dubai, fire detection system Dubai |

### Technical SEO Implemented
- ✅ `<title>` with primary + longtail keyword
- ✅ `<meta description>` under 160 chars with CTA
- ✅ `<link rel="canonical">` pointing to production domain
- ✅ **H1** → "Dubai's #1 Fire & Safety Company in Dubai"
- ✅ **H2 ×7** each targeting a distinct longtail keyword
- ✅ **H3 ×6** each targeting a service-specific longtail
- ✅ **LocalBusiness schema** with areaServed all 7 UAE Emirates
- ✅ **FAQPage schema** (JSON-LD + inline itemscope)
- ✅ **Offer Catalog schema** with 8 named services
- ✅ **Aggregate Rating schema** (4.9/5 · 187 reviews)
- ✅ **Open Graph** tags (Facebook, LinkedIn, WhatsApp preview)
- ✅ **Twitter Card** meta tags
- ✅ **Geo meta** tags (AE-DU region)
- ✅ **XML Sitemap** with priority weights
- ✅ **robots.txt** with sitemap declaration
- ✅ Keywords in footer anchor link text

### Post-Deploy Checklist
- [ ] Submit sitemap to [Google Search Console](https://search.google.com/search-console)
- [ ] Add `https://ignishield.ae` as a property in GSC
- [ ] Create and upload `og-image.jpg` (1200×630px) to `/public/assets/`
- [ ] Generate PNG favicons from `favicon.svg` and place in `/public/assets/`
- [ ] Connect [Vercel Analytics](https://vercel.com/analytics) (free, no cookie banner needed)
- [ ] Test with [PageSpeed Insights](https://pagespeed.web.dev/)
- [ ] Test with [Google Rich Results Test](https://search.google.com/test/rich-results)
- [ ] Test with [Open Graph Debugger](https://developers.facebook.com/tools/debug/)
- [ ] Register on [Google Business Profile](https://business.google.com/) with the same NAP (Name, Address, Phone)

---

## 💻 Local Development

```bash
# Install dev dependencies
npm install

# Run local preview server at http://localhost:3000
npm run dev
```

---

## 📞 Contact

**IgniShield Fire & Safety LLC**
Sheikh Zayed Road, Dubai, UAE
📞 +971 4 200 0000
✉️ info@ignishield.ae
💬 WhatsApp: +971 50 123 4567

---

*Built for maximum SEO performance and Vercel edge delivery. Replace placeholder phone numbers and domain before going live.*
