# Mitzie's Jerk Kitchen

Static website. No build step.

## Deploy to Hostinger

**Option A: Git deploy (recommended)**
1. hPanel → Websites → Manage → **Advanced → Git**.
2. Repository: `https://github.com/Mesumraza08-art/kitchen.git`, branch `main`, directory: leave empty (deploys to `public_html`).
3. Click **Create**, then **Deploy**. Enable **Auto Deployment** to redeploy on every push (add the webhook URL to GitHub → Settings → Webhooks).

**Option B: File Manager**
Upload `index.html`, `404.html`, `.htaccess`, `robots.txt` and `sitemap.xml` into `public_html`.

Then enable the free SSL certificate in hPanel → Security → SSL. `.htaccess` forces HTTPS.

## Files
- `index.html`: the full site (images inlined)
- `.htaccess`: HTTPS redirect, compression, caching, security headers
- `404.html`: not-found page
