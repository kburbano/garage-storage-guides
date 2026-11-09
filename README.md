# Garage Storage Guides

Static HTML site for long-tail garage storage & organization comparisons. Built for **GitHub Pages** (no build step).

**Live URL (after Pages is on):** https://kburbano.github.io/garage-storage-guides/

Suggested repo name: `garage-storage-guides`

## Pages

| File | Purpose |
|------|---------|
| `index.html` | Home + links to guides |
| `garage-slatwall-proslat-vs-gladiator.html` | Slatwall: Proslat vs Gladiator vs StoreWALL (2026) |
| `overhead-garage-racks-low-ceilings.html` | Best overhead racks for low ceilings (2026) |
| `motorized-garage-storage-lift-worth-it.html` | Motorized garage storage lift: Garage Gator vs GarageSmart vs Auxx-Lift vs ONRAX (2026) |
| `garage-bike-storage-without-drilling-concrete.html` | Bike storage without drilling concrete (2026) |
| `garage-ladder-storage-wall-vs-ceiling.html` | Ladder storage, wall vs ceiling mounts (2026) |
| `styles.css` | Shared mobile-friendly CSS |
| `robots.txt` | Allow crawl + sitemap pointer |
| `sitemap.xml` | Basic sitemap (update base URL if repo/user changes) |
| `topic-research.md` | Running log of topics considered |

## Affiliate disclosure

Amazon product and search links use Associates tracking ID `garagestor0be-20` (`tag=garagestor0be-20`). Each page includes: “As an Amazon Associate I earn from qualifying purchases.”

Keep a known ASIN when the page already links to that product. If there is no ASIN, link to an Amazon search URL (`https://www.amazon.com/s?k=...&tag=garagestor0be-20`). Do not invent ASINs. Amazon links use `rel="sponsored nofollow noopener"` and `target="_blank"`.

## Publish on GitHub Pages (@kburbano)

1. Create a public repo named `garage-storage-guides` under **@kburbano** (or your GitHub account).
2. Push this folder to the repo root (these files at the top level of `main`, not nested in a subfolder).
3. On GitHub: **Settings → Pages**.
4. Under **Build and deployment**:
   - **Source:** Deploy from a branch
   - **Branch:** `main`
   - **Folder:** `/ (root)`  
   (Use `/docs` only if you move the site into a `docs/` folder instead.)
5. Save. After a minute or two, open:  
   `https://kburbano.github.io/garage-storage-guides/`
6. If the username or repo name differs, update:
   - `robots.txt` Sitemap URL
   - `sitemap.xml` `<loc>` values
   - `<link rel="canonical">` on each HTML page

### Quick push (after `gh` / git is authenticated)

```bash
cd garage-storage-site
git init
git add .
git commit -m "Initial Garage Storage Guides site"
gh repo create garage-storage-guides --public --source=. --remote=origin --push
# then enable Pages as above (Settings → Pages → main / root)
```

Or create the empty repo on github.com first, then:

```bash
git remote add origin https://github.com/kburbano/garage-storage-guides.git
git branch -M main
git push -u origin main
```

## Local preview

Open `index.html` in a browser, or from this folder:

```bash
python3 -m http.server 8080
```

Then visit http://localhost:8080/

## Honest timing

Months 1–2 are indexing and content. Re-check live prices before anyone buys.
