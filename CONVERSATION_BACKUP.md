# 30 Best Prompts - Deployment Backup

## Date: 2026-07-10

## Live URLs

- **GitHub Pages**: https://ucfzem.github.io/30-best-prompts/
- **Vercel**: https://30-best-prompts.vercel.app/
- **Cloudflare Pages**: https://30-best-prompts.pages.dev/

## Repository

- **GitHub**: https://github.com/ucfzem/30-best-prompts
- **Branch**: gh-pages

## What Was Fixed

1. **Broken navigation links** - All 30 prompts properly linked
2. **Wrong fonts** - Changed to Cairo (Arabic), Outfit (body), Playfair Display (headings)
3. **JS syntax error** - `b.textContent={(i-1)*10+1}+'–'+i*10;` → `b.textContent=((i-1)*10+1)+'–'+(i*10);`
4. **Missing prompts** - Rebuilt with all 30 prompts (n:1 through n:30)

## File Structure

- `index.html` - Single page with 30 prompts, 3-tab pagination, search, categories, light/dark mode, 4 languages
- `.nojekyll` - Prevents Jekyll processing on GitHub Pages

## Deployment Details

### GitHub Pages
- Branch: gh-pages
- Status: built
- No custom domain needed

### Vercel
- Project: 30-best-prompts
- Domain: 30-best-prompts.vercel.app
- Framework: None (static)

### Cloudflare Pages
- Project: 30-best-prompts
- Domain: 30-best-prompts.pages.dev
- Hash algorithm: BLAKE3 (not SHA-256!)

## Important Notes

- Cloudflare Pages requires BLAKE3 hash for content-addressed storage
- Vercel needs "target": "production" in deployment payload
- GitHub Pages can take 24-48h to propagate on some ISPs
