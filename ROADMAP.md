# Roadmap — docker-pro / Feuille de route

---

## Phase 1 — Foundation / Fondation

Core services up and running. Shared infrastructure confirmed.
Services de base opérationnels. Infrastructure partagée confirmée.

- [x] Repo initialized / Dépôt initialisé
- [x] Caddy reverse proxy configured / Proxy inverse Caddy configuré
- [x] Tailscale private network active / Réseau privé Tailscale actif
- [x] Cloudflare DNS routing / Routage DNS Cloudflare
- [ ] `security/authentik` — SSO & 2FA live / SSO et 2FA opérationnel
- [ ] `security/vaultwarden` — password manager live / Gestionnaire de mots de passe opérationnel
- [ ] `bi/superset` — BI stack live / Stack analytique opérationnel
- [ ] `bi/metabase` — BI stack live / Stack analytique opérationnel
- [ ] `devops/prometheus` — metrics collection live / Collecte de métriques opérationnelle
- [ ] `devops/grafana` — metrics dashboard live / Tableau de bord opérationnel
- [ ] `pm/vikunja` — project management live / Gestion de projet opérationnelle

## Phase 2 — ERP & CRM
 
Resource-heavy — plan NAS headroom before starting.
Gourmands en ressources — planifier la capacité du NAS avant de démarrer.
 
- [ ] `erp-crm/twenty` — open-source CRM (lean, start here) / CRM libre (léger, commencer ici)
- [ ] `erp-crm/erpnext` — open-source ERP (resource-heavy) / ERP libre (gourmand en ressources)
