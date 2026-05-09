# GLPI Local Smoke Evidence

Captured on May 9, 2026 from a local Docker Compose run.

## Runtime

The default `8080` host port was already used by an existing local Weaviate container, so GLPI was started with a temporary Compose override on `8081`.

```text
docker compose --env-file .env.example -f docker-compose.yml -f /tmp/glpi-port-8081.yml up -d --force-recreate glpi
```

## Result

```text
glpi_db   mariadb:10.11      Up (healthy)
glpi      glpi/glpi:latest   Up, 0.0.0.0:8081->80/tcp
```

The GLPI container completed installation and reached the dashboard:

```text
GLPI installation completed successfully.
Apache/2.4.66 configured -- resuming normal operations
```

HTTP check:

```text
200 http://localhost:8081/
```

## Screenshots

- [Login screen](glpi-login.png)
- [Dashboard](glpi-dashboard.png)

This proves the Docker Compose stack can run locally. It does not yet prove configured ticket categories, assets, SLA rules, or reporting views.
