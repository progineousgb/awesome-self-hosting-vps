<p align="center"><img src="assets/logo.png" alt="Pro Gineous" width="360"></p>

# Awesome self-hosting on a VPS

Open-source apps that are practical to run yourself on one small virtual server (1 to 4 GB of RAM, a couple of vCPUs). Heavy platforms that really want a cluster or a big box are left out on purpose, as are projects that are archived or no longer maintained.

Links go to each project's own site or source repository. Every link was checked when the list was last updated; if one breaks, open an issue.

## Contents

- [Reverse proxies](#reverse-proxies)
- [Deployment and containers](#deployment-and-containers)
- [Files and sync](#files-and-sync)
- [Passwords and identity](#passwords-and-identity)
- [Analytics](#analytics)
- [Monitoring and alerts](#monitoring-and-alerts)
- [Automation](#automation)
- [Git and CI](#git-and-ci)
- [Websites and publishing](#websites-and-publishing)
- [Notes, wikis and docs](#notes-wikis-and-docs)
- [Reading and bookmarks](#reading-and-bookmarks)
- [Email and newsletters](#email-and-newsletters)
- [Chat](#chat)
- [Networking and VPN](#networking-and-vpn)
- [Backups](#backups)
- [Productivity](#productivity)
- [Small utilities](#small-utilities)
- [Related articles](#related-articles)

## Reverse proxies

- [Caddy](https://caddyserver.com/) - Web server and reverse proxy that gets and renews TLS certificates on its own.
- [Nginx](https://nginx.org/) - The usual web server and reverse proxy. More config to write, very well documented.
- [Traefik](https://doc.traefik.io/traefik/) - Reverse proxy that configures itself from Docker labels.
- [Nginx Proxy Manager](https://nginxproxymanager.com/) - Web UI on top of Nginx for proxy hosts and Let's Encrypt certificates.

## Deployment and containers

- [Coolify](https://coolify.io/) - Self-hosted alternative to Heroku/Netlify. Deploys apps, databases and services to your own servers.
- [Dokku](https://dokku.com/) - Small PaaS built on Docker; `git push` to deploy.
- [CapRover](https://caprover.com/) - App platform with a web UI and one-click apps, running on Docker Swarm.
- [Dockge](https://dockge.kuma.pet/) - Web UI for managing `compose.yaml` stacks.
- [Portainer](https://www.portainer.io/) - Container management UI. The Community Edition is open source.

## Files and sync

- [Nextcloud](https://nextcloud.com/) - File sync and share, plus calendar, contacts and office apps. One of the heavier apps here.
- [Seafile](https://www.seafile.com/en/home/) - File sync focused on speed, with block-level deduplication.
- [Syncthing](https://syncthing.net/) - Peer-to-peer folder sync. No central server needed, but a VPS makes a good always-on peer.
- [File Browser](https://github.com/filebrowser/filebrowser) - Web file manager for a directory on the server.

## Passwords and identity

- [Vaultwarden](https://github.com/dani-garcia/vaultwarden) - Lightweight Bitwarden-compatible server written in Rust.
- [Authelia](https://www.authelia.com/) - Single sign-on and two-factor portal that sits in front of your reverse proxy.
- [authentik](https://goauthentik.io/) - Identity provider with OAuth2/OIDC, SAML and LDAP.
- [Pocket ID](https://pocket-id.org/) - Simple OIDC provider that uses passkeys only.
- [Keycloak](https://www.keycloak.org/) - Full identity and access management server. Heavier than the others here.

## Analytics

- [Umami](https://umami.is/) - Privacy-focused web analytics on PostgreSQL.
- [Plausible Community Edition](https://plausible.io/self-hosted-web-analytics) - Cookie-free analytics. Needs ClickHouse, so plan for more RAM.
- [Matomo](https://matomo.org/) - Full-featured analytics on PHP and MySQL/MariaDB.
- [GoatCounter](https://www.goatcounter.com/) - Small analytics app, a single Go binary with SQLite or PostgreSQL.

## Monitoring and alerts

- [Uptime Kuma](https://uptime.kuma.pet/) - Uptime monitoring with status pages and many notification channels.
- [Gatus](https://gatus.io/) - Health checks and a status page defined in a YAML file.
- [Beszel](https://beszel.dev/) - Lightweight server monitoring with a hub and small agents, including Docker stats.
- [Netdata](https://www.netdata.cloud/) - Per-second system metrics with no setup.
- [Prometheus](https://prometheus.io/) - Metrics collection and alerting.
- [Grafana](https://grafana.com/oss/grafana/) - Dashboards for Prometheus and many other data sources.
- [Healthchecks](https://github.com/healthchecks/healthchecks) - Alerts you when a cron job or backup does not check in.
- [changedetection.io](https://github.com/dgtlmoon/changedetection.io) - Watches web pages for changes and notifies you.
- [ntfy](https://ntfy.sh/) - Push notifications to phone or desktop with a plain HTTP POST.
- [Gotify](https://gotify.net/) - Self-hosted push notification server with an Android app.

## Automation

- [n8n](https://n8n.io/) - Workflow automation with a visual editor and hundreds of integrations. Fair-code licence, source available.
- [Node-RED](https://nodered.org/) - Flow-based programming for wiring APIs and devices together.
- [Activepieces](https://www.activepieces.com/) - Zapier-style automation, MIT-licensed community edition.

## Git and CI

- [Forgejo](https://forgejo.org/) - Community-run Git forge, a hard fork of Gitea.
- [Gitea](https://about.gitea.com/) - Lightweight Git hosting with issues, pull requests, packages and Actions.
- [Woodpecker CI](https://woodpecker-ci.org/) - Container-based CI that works with Forgejo, Gitea, GitLab and GitHub.

## Websites and publishing

- [WordPress](https://wordpress.org/) - The CMS behind a large share of the web.
- [Ghost](https://ghost.org/) - Publishing platform for blogs and paid newsletters, on Node.js and MySQL.
- [Flarum](https://flarum.org/) - Forum software on PHP, light enough for a small server.
- [Discourse](https://www.discourse.org/) - Discussion platform. Heavier than Flarum; read the memory notes in its install guide first.

## Notes, wikis and docs

- [BookStack](https://www.bookstackapp.com/) - Wiki organised as shelves, books, chapters and pages.
- [Wiki.js](https://wiki.js.org/) - Wiki on Node.js with Markdown and a visual editor.
- [Outline](https://www.getoutline.com/) - Team knowledge base with real-time collaborative editing.
- [HedgeDoc](https://hedgedoc.org/) - Collaborative Markdown editor in the browser.
- [Memos](https://usememos.com/) - Lightweight note-taking with a timeline layout.
- [Paperless-ngx](https://github.com/paperless-ngx/paperless-ngx) - Scans, OCRs and indexes paper documents.

## Reading and bookmarks

- [FreshRSS](https://freshrss.org/) - RSS aggregator on PHP with mobile app support.
- [Miniflux](https://miniflux.app/) - Minimalist RSS reader, one Go binary plus PostgreSQL.
- [wallabag](https://wallabag.org/) - Save web pages to read later.
- [linkding](https://linkding.link/) - Bookmark manager, small and fast.
- [Linkwarden](https://linkwarden.app/) - Bookmarks with archived copies of each page.

## Email and newsletters

Running your own mail server is the hardest thing on this list. You need a clean IP, reverse DNS, SPF, DKIM and DMARC, and some providers block outbound port 25 by default.

- [mailcow](https://mailcow.email/) - Full mail suite in Docker: Postfix, Dovecot, Rspamd, SOGo webmail.
- [docker-mailserver](https://docker-mailserver.github.io/docker-mailserver/latest/) - Mail server in one container, configured with files and env vars.
- [Stalwart](https://stalw.art/) - Mail server written in Rust with JMAP, IMAP and SMTP.
- [listmonk](https://listmonk.app/) - Newsletter and mailing list manager. Send through your own SMTP or a relay.

## Chat

- [Matrix](https://matrix.org/) - Open protocol for decentralised chat. Synapse is the reference homeserver; [Element](https://element.io/) is the main client.
- [Mattermost](https://mattermost.com/) - Slack-style team chat.
- [Zulip](https://zulip.com/) - Team chat organised by topic threads.
- [Rocket.Chat](https://www.rocket.chat/) - Team chat with omnichannel support.

## Networking and VPN

- [WireGuard](https://www.wireguard.com/) - Fast, simple VPN built into the Linux kernel.
- [wg-easy](https://github.com/wg-easy/wg-easy) - WireGuard with a web UI for adding clients.
- [Headscale](https://headscale.net/) - Open-source implementation of the Tailscale control server.
- [NetBird](https://netbird.io/) - WireGuard-based mesh VPN with a self-hostable management server.
- [Pi-hole](https://pi-hole.net/) - DNS sinkhole that blocks ads and trackers.
- [AdGuard Home](https://github.com/AdguardTeam/AdGuardHome) - DNS-level ad blocking with DoH and DoT support.
- [Technitium DNS Server](https://technitium.com/dns/) - Authoritative and recursive DNS server with a web UI.

## Backups

- [restic](https://restic.net/) - Encrypted, deduplicated backups to S3, SFTP, B2 and more.
- [BorgBackup](https://www.borgbackup.org/) - Deduplicating, compressed, encrypted backups over SSH.
- [Kopia](https://kopia.io/) - Snapshot backups with a CLI and optional web UI.
- [Duplicati](https://duplicati.com/) - Encrypted backups to cloud storage, configured through a web UI.

## Productivity

- [Cal.com](https://cal.com/) - Scheduling and booking pages.
- [Vikunja](https://vikunja.io/) - To-do lists and project boards.
- [Planka](https://planka.app/) - Kanban boards similar to Trello.
- [Kanboard](https://kanboard.org/) - Minimal Kanban project management on PHP.
- [Kimai](https://www.kimai.org/en/) - Time tracking for freelancers and teams.
- [Invoice Ninja](https://invoiceninja.com/) - Invoicing, quotes and payments.
- [Actual Budget](https://actualbudget.org/) - Local-first personal budgeting with an optional sync server.
- [Firefly III](https://firefly-iii.org/) - Personal finance manager.
- [Mealie](https://mealie.io/) - Recipe manager and meal planner.
- [LimeSurvey](https://www.limesurvey.org/) - Survey tool. The Community Edition is GPL.
- [Formbricks](https://formbricks.com/) - Forms and in-app surveys.

## Small utilities

- [PrivateBin](https://privatebin.info/) - Pastebin where the server cannot read the pastes (client-side encryption).
- [YOURLS](https://yourls.org/) - URL shortener on PHP and MySQL.
- [Shlink](https://shlink.io/) - URL shortener with a REST API and visit stats.
- [SearXNG](https://docs.searxng.org/) - Metasearch engine that does not track you.
- [Homepage](https://gethomepage.dev/) - Dashboard page for all your self-hosted services.

## Related articles

From the [Pro Gineous blog](https://blog.progineous.com/):

- [Setting Up a New VPS: The First-Boot Checklist](https://blog.progineous.com/how-to-set-up-a-vps/)
- [How Much RAM Does a VPS Need?](https://blog.progineous.com/how-much-ram-a-vps-needs/)
- [Choosing a VPS Plan: Start with Memory](https://blog.progineous.com/how-to-choose-a-vps-plan/)
- [Shared Hosting vs VPS: Which One Fits Your Site?](https://blog.progineous.com/shared-hosting-vs-a-vps/)
- [Managed vs Unmanaged VPS: Who Does the Work?](https://blog.progineous.com/managed-vps-vs-unmanaged/)
- [Secure a Linux VPS in 15 Minutes: SSH, ufw, fail2ban](https://blog.progineous.com/secure-linux-vps-15-minutes/)
- [How to Secure a VPS: Keys, Ports and Updates](https://blog.progineous.com/how-to-secure-a-vps/)
- [How to Back Up a VPS and Prove the Restore Works](https://blog.progineous.com/how-to-back-up-a-vps/)
- [Moving WordPress to a Cloud Server](https://blog.progineous.com/wordpress-on-a-cloud-server/)
- [Why Is My Email Going to Spam?](https://blog.progineous.com/how-to-keep-email-out-of-spam/)

## Contributing

Add an app by merge request. It should be open source, actively maintained, and run on a single small server without heroics. One line, link to the official site or repository, no marketing copy. Keep each section in the order it is in; new entries go at the end of their section.

## License

MIT, see [LICENSE](LICENSE).

---

Need a server to try these on? [Pro Gineous](https://progineous.com/) sells VPS plans. Scripts for setting one up: [server-toolkit](https://gitlab.com/pro-gineous-group/server-toolkit).
