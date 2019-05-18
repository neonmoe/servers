# Servers I host
This is a catalog of my servers and what's running on them.

## Eevee - Raspberry Pi 2B
The "router" pi, mostly just running caddy.

### Services
- caddy (proxying, serving the following from git)
  - archive.neon.moe (big files from sylveon)
  - eevee,sylveon,leafeon.neon.moe
  - showoffhour.fyi
  - kalmotaiteelle.fi
  - neon.moe
- netdata (monitor.eevee.neon.moe, for monitoring)

## Sylveon - Raspberry Pi 3B+
The "storage" pi, mostly just serving big files with caddy.

### Services
- caddy (serving big files)
- netdata (monitor.sylveon.neon.moe, for monitoring)

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
- netdata (monitor.leafeon.neon.moe)
