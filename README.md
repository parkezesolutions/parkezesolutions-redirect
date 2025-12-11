# parkezesolutions-redirect

Redirect my.parkezesolutions.com to my.parkeze.com with a message saying it's been permanently moved.

## Features

- HTTP 301 (Permanent) redirect message
- Professional styled page matching parkeze.com branding
- 5-second countdown with automatic redirect
- Manual redirect button for immediate access
- Works on GitHub Pages, Netlify, Vercel, and Apache servers

## GitHub Pages Deployment

1. Go to repository Settings → Pages
2. Under "Source", select the branch (e.g., `main` or `copilot/redirect-subdomain-to-new-url`)
3. Click Save
4. Configure your DNS to point `my.parkezesolutions.com` to GitHub Pages:
   - Add a CNAME record pointing to `<username>.github.io`
   - Or add A records pointing to GitHub Pages IPs
5. Add `my.parkezesolutions.com` as a custom domain in GitHub Pages settings

## Files

- `index.html` - Main redirect page with styled 301 message
- `404.html` - Fallback page (copy of index.html) for GitHub Pages
- `.nojekyll` - Disables Jekyll processing on GitHub Pages
- `_config.yml` - GitHub Pages configuration
- `.htaccess` - Apache server configuration
- `netlify.toml` - Netlify configuration
- `vercel.json` - Vercel configuration
- `_redirects` - Netlify/Vercel redirects file
