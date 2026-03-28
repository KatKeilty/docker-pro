# Vikunja

Task manager. Postgres backend.

## Paths
- Config/files: `${CONFIG_PATH}/vikunja/`
- DB data: `${CONFIG_PATH}/vikunja/db/`

## First run
```
mkdir -p /share/docker/home/vikunja/{files,db}
docker compose up -d
```

## Notes
- JWT secret must be set before first start
- DB container must be healthy before app starts (depends_on handles ordering)
