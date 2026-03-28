# Metabase

BI and analytics. H2 embedded DB.

## Paths
- DB file: `${CONFIG_PATH}/metabase/data/metabase.db`

## First run
```
mkdir -p /share/docker/home/metabase/data
docker compose up -d
```


## Notes
- H2 is fine for personal use; migrate to Postgres if load increases
- Initial setup wizard runs on first access
