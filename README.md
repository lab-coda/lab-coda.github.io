# lab-coda.github.io

Lab website for the CODA Lab at UBC, built with [Hugo](https://gohugo.io/) using the [hugo-scroll](https://github.com/janraasch/hugo-scroll) theme.

## Local development

```bash
hugo server --renderStaticToDisk
```

> **Note:** Do not use plain `hugo server`. Static files (including CSS) may not sync on startup, causing styles to appear broken until you manually save a file in `static/`. The `--renderStaticToDisk` flag serves static files directly from disk and avoids this issue. This is a know Hugo quirk according to Claude.

## Adding a new lab member

Please submit as a pull request.

1. Add a headshot to `assets/images/people/<first-name-last-name>.png` (square crop recommended).
2. Copy the template block from the comment in `content/en/homepage/people.md` and fill in the details.
3. Use `![profile-photo](images/people/<first-name-last-name>.png)` as the image line — the `profile-photo` alt text is required for the circular crop and two-column layout CSS to apply.

## Deployment

The site deploys automatically to GitHub Pages on push to `main`.
