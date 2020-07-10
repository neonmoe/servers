# Servers I host
This is a catalog of my servers and what's running on them, so I don't
forget.

Currently the architecture is very ad-hoc: the server software is
installed via AUR and run via systemd units. The plan is to wrap
everything up into Docker containers, and then possibly make the whole
thing into a Kubernetes cluster.

## Eevee - Raspberry Pi 2B
The "router" pi, mostly just running caddy.

### Services
- caddy
  - static pages in /var/lib/caddy/
    - blog.neon.moe (static page, files hosted here)
    - cv.pitkanen.dev (static page, files hosted here)
    - goaccess.neon.moe (static page, files hosted here)
    - moe.neon.moe (static page, files hosted here)
    - reclaimani.me (static page, files hosted here)
    - neon.moe (static page, files hosted here)
  - proxies
    - activity.neon.moe (proxied to sylveon)
    - archive.neon.moe (proxied to sylveon)
    - fedi.neon.moe (proxied to flareon)
    - git.neon.moe (proxied to leafeon)
    - miniflux.functional.technology (proxied to leafeon)

## Sylveon - Raspberry Pi 3B+
The "storage" pi, mostly just serving big files with caddy. This is
the only Pi connected to an external hard-drive.

### Services
- activity-graph (activity.neon.moe)
- caddy (archive.neon.moe)

## Leafeon - Raspberry Pi 3B+
The "jack of all trades" pi, running all kinds of light loads.

### Services
- miniflux2 (miniflux.functional.technology)
- gitea (git.neon.moe)
- roguesque (for roguesque leaderboards)
- postgresql (for gitea and miniflux2)

## Flareon - Raspberry Pi 3B+
The "social media" pi. I've hosted irc, xmpp and matrix here at
various times, or tried to, but currently it's just Pleroma.

### Services
- pleroma (fedi.neon.moe)
