# matteverard.com

A single-file static personal site. No build step, no framework, no dependencies. Edit `index.html` directly.

## Files

- `index.html` — the entire site
- `404.html` — friendly not-found page
- `robots.txt` — tells search engines they can crawl everything

## Deploy

Pick whichever you like. All three are free, fast, and connect to a custom domain in a few clicks.

### Netlify (easiest)

1. Go to https://app.netlify.com/drop
2. Drag this whole folder onto the page
3. Get a temporary URL like `random-name.netlify.app` instantly
4. Add your domain in Site settings → Domain management

### Vercel

1. `npm i -g vercel`
2. From this folder, run `vercel`
3. Follow the prompts; add your domain in the dashboard

### GitHub Pages

1. Create a public repo named `matteverard.github.io`
2. Drop these files in, push to `main`
3. Site goes live at `https://matteverard.github.io`
4. Add custom domain in repo Settings → Pages

## Custom domain

Point `matteverard.com` (and `www.matteverard.com`) at your host's nameservers or A/CNAME records. Each host has a one-page guide. Use Cloudflare in front for free HTTPS + CDN if you want.

## What to update before you ship

- [ ] Email address (currently `matt@matteverard.com` — change if different)
- [ ] LinkedIn URL (currently `linkedin.com/in/matt-everard` — placeholder)
- [ ] GitHub URL (currently `github.com/matteverard` — placeholder)
- [ ] First real blog post (the Writing section currently says "coming soon")
- [ ] Long-form About page (the homepage links to `/about` which doesn't exist yet)

## Editing

It's just HTML. Open in any editor. The CSS is embedded in `<style>` at the top.

To change colors, edit the CSS variables in `:root` near the top. There's a dark mode that auto-activates based on the visitor's OS preference.

The page-load animation respects `prefers-reduced-motion`, so visitors who've disabled motion won't see it.
