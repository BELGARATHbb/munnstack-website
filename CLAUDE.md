# munnstack.com — LIVE WEBSITE

**Pushing to `main` deploys to production immediately via GitHub Pages.** Be careful — this is the real munnstack.com.

## Stack
- Static HTML/CSS/JS (single `index.html`)
- GitHub Pages hosting
- Custom domain: munnstack.com (CNAME file)
- Logo: `munnstack-logo-dark-highres.png`

## Files
| File | Purpose |
|------|---------|
| `index.html` | The entire website |
| `404.html` | Custom 404 page |
| `CNAME` | GitHub Pages custom domain config — **do not delete** |
| `.nojekyll` | Tells GitHub Pages to skip Jekyll processing — **do not delete** |
| `robots.txt` | Search engine crawling rules |
| `sitemap.xml` | SEO sitemap |

## Deployment
Pushing to `main` auto-deploys via GitHub Pages. There is no build step.

```bash
ga . && gc -m "description of change" && gp origin main
# Site is live within ~60 seconds
```

## Git
- Repo: `BELGARATHbb/munnstack-website`
- Branch: `main` (deploys immediately)
- **No testing branch** — this is a simple static site, what you push is what's live

## Rules
- **Test changes locally first** — open `index.html` in a browser before pushing
- Never delete `CNAME` or `.nojekyll`
- Keep the site fast — it's a single HTML file, no frameworks
