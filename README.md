# cbhrcom.com

Public CBHR site for **Terms** and **Privacy** pages used by Devvit and related apps.

This is **not** the Absolon Designs portfolio. Visitors use **cbhrcom.com** only.

## URLs (after Cloudflare Pages + custom domain)

- https://cbhrcom.com/
- https://cbhrcom.com/terms/
- https://cbhrcom.com/privacy/

## Cloudflare Pages setup

1. [Cloudflare Dashboard](https://dash.cloudflare.com) → account that owns **cbhrcom.com**
2. **Workers & Pages** → **Create** → **Pages** → **Connect to Git**
3. Select repo: **`thurnix01/cbhrcom`**
4. Build settings:

| Field | Value |
|--------|--------|
| Framework preset | None |
| Build command | *(leave empty)* or `echo "static site"` |
| Build output directory | `/` |
| Root directory | `/` |

5. **Save and Deploy**
6. **Custom domains** → add **`cbhrcom.com`**
7. Confirm Cloudflare DNS for the apex
8. Leave **`n8n.cbhrcom.com`** unchanged

## Devvit

In [developer settings](https://developers.reddit.com/apps/pb-content-intel/developer-settings) use:

- Terms: `https://cbhrcom.com/terms/`
- Privacy: `https://cbhrcom.com/privacy/`
