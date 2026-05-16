# aashishchakravarty.com

Personal portfolio site for Aashish Chakravarty — Senior Software Engineer.

🔗 **Live:** [aashishchakravarty.com](https://aashishchakravarty.com)

## Stack

Single-file static site. No build step, no framework.

- HTML, CSS, vanilla JavaScript
- [Geist](https://vercel.com/font) + Geist Mono via Google Fonts
- [GSAP](https://gsap.com) + ScrollTrigger for reveal animations
- [Lenis](https://github.com/darkroomengineering/lenis) for smooth scroll
- Hosted on GitHub Pages with a custom domain

## Local development

It's one file. Open it.

```bash
# any static server works
python3 -m http.server 8000
# then visit http://localhost:8000
```

Or just double-click `index.html`. The CDN dependencies (GSAP, Lenis, Google Fonts) require an internet connection.

## Deployment

GitHub Pages serves the `master` branch automatically. Push to deploy.

```bash
git add .
git commit -m "update"
git push origin master
```

The `CNAME` file pins the custom domain to `aashishchakravarty.com`. DNS for the apex domain points to GitHub Pages' IPs; `www` is a CNAME to `aashishchakravarty.github.io`.

## Structure

```
.
├── index.html        # The entire site
├── 404.html          # Custom 404 page
├── CNAME             # Custom domain pin
├── robots.txt        # Crawler hints
├── sitemap.xml       # SEO sitemap
├── .nojekyll         # Skip Jekyll processing
├── README.md         # This file
└── old/              # Archive of previous versions
```

## License

Source code is MIT. Content (resume, project descriptions, photos) is © Aashish Chakravarty — please don't copy verbatim for your own portfolio.
