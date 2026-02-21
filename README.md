# Iron Horse FC

Community-owned, cooperatively governed football club. Kitchener–Waterloo.

## Deploy

This is a single-page static site. It runs on [GitHub Pages](https://pages.github.com/).

1. Push to `main`
2. Go to **Settings → Pages → Source → Deploy from branch → `main` / `/ (root)`**
3. Site is live at `ironhorsefc.ca` (or `<username>.github.io/iron-horse-fc` before DNS)

## Custom domain

To use `ironhorsefc.ca`:

1. Buy the domain (Hover, Namecheap, etc.)
2. Add these DNS records at your registrar:

   | Type  | Name | Value                    |
   |-------|------|--------------------------|
   | A     | @    | 185.199.108.153          |
   | A     | @    | 185.199.109.153          |
   | A     | @    | 185.199.110.153          |
   | A     | @    | 185.199.111.153          |
   | CNAME | www  | `<username>.github.io`   |

3. In GitHub repo **Settings → Pages → Custom domain**, enter `ironhorsefc.ca`
4. Check "Enforce HTTPS"

The `CNAME` file in this repo handles the rest.

## Email

`contact@ironhorsefc.ca` — set up email forwarding at your domain registrar or use a service like Zoho Mail (free tier), Fastmail, or Migadu.

## Structure

```
index.html    ← the entire site
CNAME         ← custom domain config for GitHub Pages
README.md     ← this file
```
