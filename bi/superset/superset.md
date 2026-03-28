# superset

Apache Superset — open-source BI and data visualization platform.
Plateforme d'analyse et de visualisation de données libre.

---

## Requirements / Prérequis

Create a `.env` file in this directory before starting.
Créez un fichier `.env` dans ce répertoire avant de démarrer.

```env
SUPERSET_SECRET_KEY=changeme_use_a_long_random_string
ADMIN_USERNAME=admin
ADMIN_PASSWORD=changeme
ADMIN_EMAIL=admin@localhost
```

Generate a secure key / Générer une clé sécurisée :

```bash
openssl rand -base64 42
```

---

## Usage / Utilisation

```bash
# First run — initializes DB and creates admin account
# Premier démarrage — initialise la base et crée le compte admin
docker compose up -d

# Superset will be available at / Disponible à :
# http://localhost:8088
```

> The `superset-init` container runs once on first start to migrate the DB and create the admin user, then exits. Safe to restart.
>
> Le conteneur `superset-init` s'exécute une fois au premier démarrage pour migrer la base et créer l'admin, puis se termine. Sans danger au redémarrage.

---

## Tear Down / Arrêt

```bash
# Stop only / Arrêter seulement
docker compose down

# Stop and delete data / Arrêter et supprimer les données
docker compose down -v
```

---

## Notes

- To connect a data source, go to **Settings → Database Connections** after first login
