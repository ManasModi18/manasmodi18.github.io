# Manas Modi — Portfolio

**DevOps Engineer** · 5+ years turning manual releases into automated, observable platforms.

Live site: _add your URL here once deployed_

## About this site

A single-page portfolio themed around DevOps/git concepts: career history is rendered as a `git log`, skills are declared as `stack.yaml`, metrics appear as `git diff --stat`, and the contact section is a terminal-style prompt. There is no framework and no build step, only plain HTML, CSS, and JavaScript.

The design and front-end engineering are adapted (MIT licensed) from [Praveen Kumar's portfolio](https://github.com/praveenraghav01/portfolio). All content, copy, and data on this site describe Manas Modi.

## Run it locally

```
npx serve .
```

Then open the printed `localhost` URL. In VS Code you can also right-click `index.html` and choose **Open with Live Server**.

Opening `index.html` directly via `file://` works, but some browsers restrict `localStorage` and clipboard access for local files, so theme memory and the one-click email copy only work over `http://`.

## Structure

```
index.html            Page markup and content
req/css/styles.css    All styles (theme tokens, layout, motion)
req/js/main.js        Nav, reveals, live clock, hero graph, stack/yaml hover-link
req/js/preloader.js   Boot-sequence loader
req/js/cursor.js      Custom cursor
req/fonts/            Self-hosted fonts
req/img/              Profile photo
req/img/fav/          Favicon set
assets/               Résumé PDF
robots.txt            Crawler rules
sitemap.xml           Sitemap
```

## Customise

| What | Where |
|---|---|
| Name, title, bio | `index.html` (hero, About, `<head>` meta tags, JSON-LD) |
| Career history | `index.html` → `#work` section |
| Skills | `index.html` → `#stack` section |
| Certifications and education | `index.html` → `#credentials` section |
| Contact details | `index.html` → `#contact` section and footer |
| Photo | `req/img/` (update the `src` and `og:image` paths) |
| Résumé | `assets/Manas_Modi_resume.pdf` |
| Domain | canonical and `og:` tags in `index.html`, `robots.txt`, `sitemap.xml` |

## Deploy

Any static host works:

- **GitHub Pages:** repo → Settings → Pages → deploy from the `main` branch, root folder.
- **Netlify** or **Cloudflare Pages:** connect the repo, leave the build command empty, and set the publish directory to `/`.

## Credits and license

Released under the MIT License. See [LICENSE](LICENSE). The original copyright notice from the upstream project must stay in that file; add your own line below it.

Design and front-end code adapted from [Praveen Kumar's portfolio](https://praveenraghav.com/), MIT licensed.
