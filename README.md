# SeaThrough website

The landing page for SeaThrough, the Android app blocker with no forced lockout: set a limit for an app, and when time is up the sea floods in over it.

`index.html` is a single self-contained page (React 18 + htm, Framer Motion, GSAP ScrollTrigger and SplitText, Lenis, a WebGL water shader). Libraries load from pinned CDN URLs with SRI hashes; there is no build step to serve it.

The page is generated from the app repository (`web/site.src.html` and `node web/build.mjs`), which copies in the code-drawn fish, clock and feed pictures from the Play listing kit. Edit it there and copy the built `index.html` here.

Serve locally: `python -m http.server` and open http://localhost:8000. GitHub Pages can serve it from the root of `main` as is.
