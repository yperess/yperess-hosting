# yperess-hosting

Source for [yperess.com](https://yperess.com), a static site served by GitHub Pages.

- `index.html` and `style.css` are the whole site (no build step).
- `CNAME` tells GitHub Pages to serve the site on `yperess.com`.
- `.nojekyll` skips Jekyll processing.

## DNS

At your registrar, for the apex domain `yperess.com`, add these A records:

    185.199.108.153
    185.199.109.153
    185.199.110.153
    185.199.111.153

Optionally add `www` as a CNAME to `yperess.github.io`.

Then in the repo's Settings > Pages, set the source to the `main` branch (root), enter `yperess.com` as the custom domain, and tick "Enforce HTTPS" once the certificate is issued.
