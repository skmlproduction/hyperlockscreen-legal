# HyperLock — static legal pages (HTTPS publish kit)

Identical copies of in-app assets for Google Play Privacy Policy / Terms URLs.

| File | Source of truth |
|------|-----------------|
| `privacy.html` | `feature/settings/src/main/assets/legal/privacy.html` |
| `terms.html` | `feature/settings/src/main/assets/legal/terms.html` |
| `index.html` | Hand-maintained Pages landing (not overwritten by sync) |

## Sync after editing in-app HTML

```bash
bash scripts/sync-legal-https.sh
```

## Publish (example paths)

```
https://<your-domain>/hyperlock/privacy.html
https://<your-domain>/hyperlock/terms.html
```

See `docs/LEGAL_HTTPS_HOSTING.md` for GitHub Pages / Cloudflare steps and Play Console checklist.

**Do not** put a real production domain in the app until HTTPS returns 200 and text matches these files.
