# XNVD Realistimo feed

Public XML feed for Realistimo import.

## URLs

After Vercel is connected to this repo, use:

- `https://<your-project>.vercel.app/realistimo.xml`
- `https://<your-project>.vercel.app/feed/realistimo.xml` (rewrite)

Until then, raw GitHub works for testing:

- https://raw.githubusercontent.com/penevxnvd-dev/xnvd-feed/main/realistimo.xml

## Generate

From `XNVD-Automation`:

```bash
npm run realistimo:feed:build -- --ids=108857,92555,92785
npm run realistimo:feed:push
```

`realistimo.xml` must live at the **repo root** so Vercel static hosting serves `/realistimo.xml` (not `/public/...`).
