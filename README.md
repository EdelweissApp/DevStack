## Edelweiss app - DevStack

### Usage
```
# Base image only
cp ./.env.example ./.env
docker-compose up -d
```
### Base configuration
- Edelweiss app (edelweissapp/dev:latest)
- MariaDB (bitnami/mariadb:latest)
- Redis (bitnami/redis:latest)
- RabbitMQ (bitnami/rabbitmq)

```
# Base image and addons
cp ./.env.example ./.env
docker-compose -f docker-compose.yml -f docker-compose-addon.yml up -d
```

### Addon useful services
- Redmon (vieux/redmon)
