### General

This repository is used to update the denverdevops.org website, it is deployed via github pages. 

### Who we are
The organization is affiliated with devopsdays.org/denver, which runs the annual DevOpsDays Rockies conference.


Below that is a "Connect With Us" tile section (Slack, Meetup, YouTube, Luma calendar, Wild Spaces, DevOpsDays Rockies) and a "What We're About" section. This existing tile pattern is a good starting point for the new "Get Involved" page (see Section 5).
The organization is affiliated with devopsdays.org/denver, which runs the annual DevOpsDays Rockies conference. The 2026 event is confirmed for September 22–23, 2026 at Bierstadt Lagerhaus, 2875 Blake St, Denver, CO 80205 — the 10th annual event.

### Testing locally

This is a plain HTML/CSS site with no build step — the site root is the `docs/` folder. To preview it:

```
cd docs
python3 -m http.server 8000
```

Then open `http://localhost:8000/` in a browser.

**Don't open the HTML files directly (double-click / `file://...`).** Every page uses root-relative paths (`/styles.css`, `/images/...`, `/get-involved`, etc.) so they resolve correctly no matter how deeply nested the page is. A `file://` URL has no concept of a site root, so those paths 404 under `file://` even though they work fine on GitHub Pages and when served locally via the command above.
