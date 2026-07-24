# cbhrcom.com

Public CBHR site for **Terms** and **Privacy**.

## Important

Your deploy succeeded, but Cloudflare put the site on:

**https://cbhrcom.absolondesigns.workers.dev**

`cbhrcom.com` still has **no DNS records** for the apex (NXDOMAIN).  
`n8n.cbhrcom.com` already works — leave it alone.

## Attach cbhrcom.com to the Worker (fixes NXDOMAIN)

1. Open Cloudflare Dashboard → **Workers & Pages** → **`cbhrcom`**
2. Go to **Settings** → **Domains & Routes** (sometimes under **Triggers**)
3. Click **Add** → **Custom Domain**
4. Enter: **`cbhrcom.com`**
5. Confirm — Cloudflare will create the apex DNS records automatically
6. Wait 1–5 minutes, then open:
   - https://cbhrcom.com/
   - https://cbhrcom.com/terms/
   - https://cbhrcom.com/privacy/

Optional: also add **`www.cbhrcom.com`** the same way.

## Build settings (if you redeploy from Git)

| Field | Value |
|--------|--------|
| Deploy command | `npx wrangler deploy` |
| Root directory | `/` |
| Build command | leave empty |

Do **not** point this at the Absolon Designs repo. This project is **`thurnix01/cbhrcom`**.

## Devvit URLs (after custom domain is active)

- Terms: `https://cbhrcom.com/terms/`
- Privacy: `https://cbhrcom.com/privacy/`
