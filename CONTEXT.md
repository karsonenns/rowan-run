# rowan.run

A small, deliberately mysterious public landing page: the word "rowan", drifting ember particles that lean toward the pointer, rotating cryptic lines, and a footer showing the Pacific time. Static HTML in `site/index.html`, served by nginx.

- **Live:** https://rowan.run and https://www.rowan.run. Let's Encrypt certificates come from Coolify's Traefik.
- **Domain:** Namecheap account karsonenns, bought 2026-09-26, order 215131469, US$3.68 on personal Visa ••4898.
  - **Auto-renew is OFF.** It renews at US$28.98, over Karson's $20 cap, so decide before 2027-09-26.
  - Free domain privacy is on.
  - DNS: A records for @ and www point to 149.56.111.214, set via the Namecheap API.
- **Hosting:** the With Awesome Coolify at portal.withawesome.co (OVH VPS-4), Root Team, project `rowan-run`, application uuid `25qovkntnur42pf7kznzuv8j`, on server `localhost`, built from the `Dockerfile`. Health check `/healthz`.
- **Repo:** github.com/karsonenns/rowan-run, public, since the page source is public anyway and Coolify's GitHub App source only covers the WithAwesome org. Pushes go through the karson-bot GitHub App credential helper. Commits are authored as Karson.
- **Deploy:** push to main, then trigger a redeploy in Coolify (no webhook yet).
- **Gotcha:** the first Let's Encrypt attempt fails if DNS hasn't propagated. Restarting the app makes Traefik retry.

## Change log
- 2026-09-26: created and live.
