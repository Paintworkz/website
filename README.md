# PaintWorkz Pro — Marketing Site

This is the public-facing marketing website for **PaintWorkz Pro**, spray shop software for cabinet and joinery finishing businesses.

**Live site:** [paintworkzpro.com.au](https://paintworkzpro.com.au) (also [paintworkzpro.com](https://paintworkzpro.com), which sends each visitor to their own country's page)
**App:** [app.paintworkzpro.com.au](https://app.paintworkzpro.com.au)

## What's in this repo

### Main pages (Australia)
| File | Purpose |
|---|---|
| `index.html` | Australian home page |
| `pricing.html` | Australian pricing (AUD, ex GST) |
| `privacy.html` | Privacy policy (all regions) |
| `terms.html` | Terms of service (all regions) |
| `refund.html` | Refund policy (all regions) |
| `reset.html` | Password reset page |
| `review.html` | "Leave a review" page for existing users (hidden from search engines) |

### Regional sites
Each folder has its own `index.html` (home page) and `pricing.html`, with local prices, units, tax and spelling. New sign-ups from each region start with matching app settings (`?region=` on the app link).

| Folder | Region | Prices (Solo / Pro, per month) |
|---|---|---|
| `/` | Australia | A$49 / A$99 ex GST |
| `us/` | United States | US$35 / US$69 |
| `uk/` | UK & Ireland | £27 / £55 ex VAT (Ireland €32 / €65) |
| `nz/` | New Zealand | NZ$65 / NZ$129 ex GST |
| `ca/` | Canada | C$52 / C$105 |

### Guides
| File | Topic |
|---|---|
| `guides.html` | List of all guides |
| `how-to-price-2-pac-cabinet-doors.html` | Pricing per m², per door or per linear metre |
| `how-much-2-pac-paint-per-square-metre.html` | Paint coverage and mixing |
| `spray-shop-scheduling-lead-times.html` | Scheduling, cure times and lead times |
| `tracking-parts-in-a-spray-shop.html` | Labels, dockets and part tracking |
| `uk/how-to-quote-a-kitchen-respray.html` | Quoting kitchen resprays (UK) |
| `us/how-to-price-cabinet-painting.html` | Pricing cabinet painting (US) |

### Other files
| File | Purpose |
|---|---|
| `sitemap.xml` | Sitemap for Google Search Console and Bing Webmaster Tools — add new pages here |
| `CNAME` | Custom domain config for GitHub Pages |
| `og-image.png` | Picture shown when the site is shared on social media |
| `favicon-32.png`, `icon-180.png`, `icon-192.png` | Browser and phone icons |
| `.well-known/` | Domain verification files |

## Hosting
Hosted on **GitHub Pages** with a custom domain via **Cloudflare DNS**. Deploys automatically when files are uploaded to `main`.

**paintworkzpro.com** redirects by visitor country (Cloudflare → paintworkzpro.com → Rules → Redirect Rules): Australia → `/`, New Zealand → `/nz/`, Canada → `/ca/`, UK & Ireland → `/uk/`, everyone else → `/us/`.

## Uploading tips
- Go **into** the folder on GitHub first (the header shows e.g. `website / us`), then **Add file → Upload files → choose your files**.
- Files with the same name (`index.html`, `pricing.html`) exist in several folders — always check which folder you're in before uploading.
- After adding a new page, add it to `sitemap.xml` and resubmit the sitemap in Google Search Console.

## Payments
Subscriptions are handled by **Paddle** (Merchant of Record), with a fixed price for each country (see the table above). Other countries pay the Australian price converted at checkout. Free plan: 3 jobs, no card. Solo includes a 7-day free trial.

## Built by
Colin Bedford — Victoria, Australia
ABN 90 419 649 257
