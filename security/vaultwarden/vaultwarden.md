# Vaultwarden

Bitwarden-compatible password manager. SQLite backend.

## Paths
- Data: `${CONFIG_PATH}/vaultwarden/data/`

## First run
```
mkdir -p /share/docker/home/vaultwarden/data
openssl rand -base64 48  # use output as VAULTWARDEN_ADMIN_TOKEN
docker compose up -d
```

## Notes
- `SIGNUPS_ALLOWED=false` -- invite users via admin panel at `/admin`
- Admin panel protected by `ADMIN_TOKEN`; use a strong generated value
- HTTPS required for Bitwarden clients to connect
