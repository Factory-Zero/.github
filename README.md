# Factory Zero &middot; `.github`

The GitHub organisation profile for [Factory Zero](https://factory0.ventures).

- **[`profile/README.md`](profile/README.md)** — the page shown at
  [github.com/Factory-Zero](https://github.com/Factory-Zero). GitHub only
  renders it from this exact path in this exact repo.
- **[`assets/logo.svg`](assets/logo.svg)** — the open ring, the source of truth
  for the mark. Its geometry matches `assets/favicon.svg` on the site, scaled
  from `r=9` to `r=150` with the same stroke ratio. `logo.png` is rendered from
  it at 1024&times;1024 for the organisation avatar, which has to be uploaded
  through the GitHub web UI (there is no REST API for it).
- **[`assets/org-banner.png`](assets/org-banner.png)** — the banner at the top
  of the profile, rendered at 2x from `tools/org-banner.html`.

Images in the profile README are referenced by absolute `raw.githubusercontent`
URL, because relative paths do not resolve for viewers of the org page.

```bash
./tools/render.sh    # regenerate the banner and the avatar (needs Chrome)
```

Venture facts on the profile page are duplicated from `assets/fz-data.js` in
[Factory-Zero/website](https://github.com/Factory-Zero/website), which is the
single source of truth. **Update them there first**, then mirror the change
here.
