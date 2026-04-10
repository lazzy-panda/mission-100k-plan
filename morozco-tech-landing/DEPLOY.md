# Deploy morozco.tech landing

Single `index.html`, dark, scroll-driven Three.js space scene over a
monochrome content overlay. Three.js loaded from `unpkg.com` CDN via
ESM import map — no build step, no `node_modules`, drag-and-drop deploy.
Static fallback for `prefers-reduced-motion` and `<noscript>`.

## Option A — Cloudflare Pages (recommended)

If you bought the domain through Cloudflare Registrar (or transferred it to Cloudflare), this is the fastest path. Everything stays in one dashboard.

1. Install wrangler once: `npm install -g wrangler` (or `bun add -g wrangler`)
2. Login: `wrangler login` (opens browser, auth with your Cloudflare account)
3. From this directory: `wrangler pages deploy . --project-name=morozco-tech`
4. First deploy: wrangler creates the project, gives you `morozco-tech.pages.dev` URL
5. Bind custom domain: `dash.cloudflare.com` → Pages → morozco-tech → Custom domains → Add `morozco.tech` and `www.morozco.tech`
6. DNS records get created automatically by Cloudflare if the domain is in the same Cloudflare account

Time: ~5 minutes after domain is registered.

## Option B — Vercel

If you prefer Vercel (you already use it for greek-app):

1. `npm install -g vercel` (or `bun add -g vercel`)
2. `vercel login`
3. `vercel --prod` from this directory
4. In Vercel dashboard → Settings → Domains → add `morozco.tech`
5. Vercel gives DNS instructions: either change nameservers to Vercel, or add A/CNAME records at Cloudflare pointing to Vercel

Time: ~10 minutes, one extra DNS step than Option A.

## Option C — Netlify Drop (zero CLI)

1. Open https://app.netlify.com/drop in browser
2. Drag this entire `morozco-tech-landing` folder onto the page
3. Netlify deploys to `random-name.netlify.app`
4. In Netlify dashboard → Domain settings → add `morozco.tech`
5. Same DNS step as Vercel

Time: ~5 minutes, no CLI, but Netlify branding until custom domain binds.

## Verification

- `curl -I https://morozco.tech` returns `200 OK`
- Open in browser, see the page
- Click `kirill@morozco.tech` link, email client opens composing a message

## After deploy

Update `cert_cca_f.md` Step 0.75 from `[ ]` to `[x]`.
Use `https://morozco.tech` in the Partner Network form Website field.
