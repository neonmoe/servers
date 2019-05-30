# Servers I host
This is a catalog of my servers and what's running on them, so I don't
forget.

## Eevee - Raspberry Pi 2B
The "router" pi, mostly just running caddy.

### Services
- caddy (proxying, serving the following from git)
  - archive.neon.moe (big files from sylveon)
  - eevee,sylveon,leafeon.neon.moe (proxy for sylveon & leafeon)
  - showoffhour.fyi
  - kalmotaiteelle.fi
  - neon.moe
- netdata (monitor.eevee.neon.moe, for monitoring)

## Sylveon - Raspberry Pi 3B+
The "storage" pi, mostly just serving big files with caddy.

### Services
- funkwhale (funk.neon.moe)
- caddy (serving big files and the status page, sylveon.neon.moe)
- netdata (for monitoring, monitor.sylveon.neon.moe)

## Leafeon - Raspberry Pi 3B+
The "jack of all trades" pi, running all kinds of light loads.

### Services
- metadata-manager (metadata.functional.technology)
- miniflux2 (miniflux.functional.technology)
- gitea (git.neon.moe)
- roguesque (for roguesque leaderboards)
- postgresql (for gitea and miniflux2)
<!-- Email -->
- dovecot (for email, mail.neon.moe)
- postfix (for email, mail.neon.moe)
- opendkim (for email)
- spamassassin (for email)
<!-- /Email -->
- caddy (status page, leafeon.neon.moe)
- netdata (monitor.leafeon.neon.moe)

## Flareon - Raspberry Pi 3B+
The currently unused pi.

### Services
- caddy (flareon.neon.moe)
- netdata (monitor.flareon.neon.moe)
