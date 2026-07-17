# suntwal.com

A small, dependency-free academic website for Sandeep Suntwal.

## Preview locally

From this directory, run:

```sh
python3 -m http.server 8181
```

Then visit <http://localhost:8181>.

## Structure

- `index.html` — home page
- `research.html` — research page
- `teaching.html` — teaching page
- `publications.html` — publications page
- `presentations.html` — presentations page
- `styles.css` — layout, responsive behavior, and print styling
- `favicon.svg` — browser icon
- `assets/` — photographs and other static files

The site uses only HTML and CSS, so it can be hosted on nearly any static web host.

## Deployment

The production site is published with GitHub Pages from the `main` branch and
uses `suntwal.com` as its custom domain. The `CNAME` file, `.nojekyll`, sitemap,
robots file, and custom 404 page are committed with the site.

Namecheap DNS should contain these records:

| Type | Host | Value |
| --- | --- | --- |
| A | `@` | `185.199.108.153` |
| A | `@` | `185.199.109.153` |
| A | `@` | `185.199.110.153` |
| A | `@` | `185.199.111.153` |
| CNAME | `www` | `shuntucodes.github.io` |

Remove conflicting parking, redirect, or wildcard records for `@` and `www`.
