# docker-pro
A curated set of Docker Compose stacks for professional demos, running on a QNAP TS-264 NAS.
Containers reverse proxied using Caddy on a private Tailscale network.

## Structure
 
```
docker-pro/
├── bi/
│   ├── superset/          # BI & analytics
│   └── metabase/          # BI & analytics
├── devops/
│   ├── gitea/             # → see docker-home
│   ├── prometheus/        # Metrics collection
│   └── grafana/           # Metrics dashboard
├── security/
│   ├── vaultwarden/       # → see docker-home
│   └── authentik/         # SSO, 2FA, OAuth2
├── pm/
│   └── vikunja/           # Project management
├── design/
│   └── penpot/            # Design & prototyping
├── files/
│   └── nextcloud/         # → see docker-home
└── erp-crm/
    ├── erpnext/           # Open-source ERP
    └── twenty/            # Open-source CRM  
```
 

Usage

```
cd <category>/<service>
docker compose up -d
```

# Stop and remove
```
docker compose down
```

Cross-home services (Gitea, Vaultwarden, Nextcloud) use the same compose files as docker-home. That repo is the source of truth.
