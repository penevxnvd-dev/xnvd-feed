# XNVD public feeds

Static feeds for portal advertising channels.

## URLs

- Realistimo XML: https://xnvd-feed.vercel.app/realistimo.xml
- alo.bg JSON: https://xnvd-feed.vercel.app/alo.json

Raw GitHub fallbacks:

- https://raw.githubusercontent.com/penevxnvd-dev/xnvd-feed/main/realistimo.xml
- https://raw.githubusercontent.com/penevxnvd-dev/xnvd-feed/main/alo.json

Root files (`realistimo.xml`, `alo.json`) are required for Vercel static hosting.

## Generate (from XNVD-Automation)

```bash
npm run realistimo:feed:build -- --ids=108857,92555,92785
npm run realistimo:feed:push

npm run alo:feed:build -- --from-realistimo --ids=108857,92555,92785
npm run alo:feed:push
```
