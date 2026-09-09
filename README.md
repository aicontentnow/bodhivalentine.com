# Portfolio — Bodhi Valentine

Creative direction, brand systems and AI production pipelines.
Single-page site. No build step, no dependencies.

## Structure

    index.html                              the page
    reel-poster.jpg                         poster frame for the video
    still-1..6.jpg                          frame strip under the reel
    FRAMEZERO_PORTFOLIO_REEL_FINAL_web.mp4  the reel (38MB)
    .nojekyll                               serve files as-is, no Jekyll

## Local preview

    python3 -m http.server 8000
    # open http://localhost:8000

## Deploy

GitHub Pages: Settings -> Pages -> Source: Deploy from a branch -> main / (root)

## Notes

- The page is set `noindex, nofollow`. Search engines will not list it.
  Anyone with the link can open it. Remove that meta tag in index.html
  to make it publicly discoverable.
- The video is referenced by exact filename in index.html. Rename it and
  you must update the `<source src="...">` line.
