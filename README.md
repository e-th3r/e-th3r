## 🔨 Currently building — **quake.su** tournament platform

![PHP](https://img.shields.io/badge/PHP-8.3-777BB4?style=flat-square&logo=php&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-16-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Apache](https://img.shields.io/badge/Apache-2.4-D22128?style=flat-square&logo=apache&logoColor=white)
![GitLab CI](https://img.shields.io/badge/GitLab_CI-auto--deploy-FC6D26?style=flat-square&logo=gitlab&logoColor=white)
![Status](https://img.shields.io/badge/status-in_production-success?style=flat-square)
![Source](https://img.shields.io/badge/source-private-lightgrey?style=flat-square)

Tournament management system serving the Russian **QuakeWorld** community — live, in production, running real seasons right now.
A heavily reworked fork of the abandoned `phpTourney` engine (2004-era PHP), migrated to PHP 8.3 and extended with a full Round Robin
subsystem, multi-division seasons and an admin toolchain.

**Live instances:** [quake.su](https://quake.su) · [RQWL](https://rqwl.quake.su) · [ThunderDome](https://td.quake.su) · [Dinosaurus&Noobs](https://din.quake.su)

**What I built into it**
- ⚔️ **Round Robin engine** — Game of N / Best of N match types, configurable (and negative) point rules, frag-diff tiebreakers, live standings, AJAX possible-score calculator
- 🏆 **Seasons & divisions** — nested divisions, per-season head-admin roles, cascade clearing, season-scoped permissions
- 🗺️ **Map pool management** — per-tournament pools, clone-from-another-tournament, live preview endpoint
- 📸 **Screenshot pipeline** — upload, crop (ImageMagick with a GD fallback), cache-busted thumbnails, N-map matches
- 🛠️ **Admin tooling** — account merge, walkover handling, bracket generation, moderated news & comments, RSS feed
- 🚀 **Ops** — legacy 5.4 → 8.3 migration, `mysql_*` → `mysqli` prepared statements, GitLab CI auto-deploy to a bare-metal VPS

> 🔒 The repository is private — it holds production config and community user data.
> Happy to walk through the architecture or share code excerpts on request.
