# Servers I host
This is a catalog of my servers and what's running on them, so I don't
forget.

## Eevee - Raspberry Pi 2B
The "router" pi, mostly just running caddy. Note: also hosts the
gravestone of moe.neon.moe, an old Mastodon instance, and it's
relatively important to keep hosting it (to return 410 instead of not
responding).

### Services
- caddy (proxy for every other pi + serving the following from git)
  - all the status pages in this doc
  - neon.moe
  - moe.neon.moe
  - blog.neon.moe
  - cv.pitkanen.dev
- netdata (monitor.eevee.neon.moe)

## Sylveon - Raspberry Pi 3B+
The "storage" pi, mostly just serving big files with caddy.
Has an external hard drive, keeps local backups. 

### Services
- caddy (serving big files and the status page, sylveon.neon.moe)
- netdata (monitor.sylveon.neon.moe)
- backups for:
  - backup system creation in progress

## Leafeon - Raspberry Pi 3B+
The "jack of all trades" pi, running all kinds of light loads.

### Services
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
The "social media" pi.

### Services
- pleroma (fedi.neon.moe)
- caddy (status page, flareon.neon.moe)
- netdata (monitor.flareon.neon.moe)
