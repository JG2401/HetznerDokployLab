# [tandoor](https://tandoor.dev)

## tandoor

### General

- Compose Path: `./projects/tandoor/docker-compose.yml`

### Environment

POSTGRES_HOST: #db name (not container-name)
POSTGRES_PORT: #default: `5432`
POSTGRES_USER: #database user
POSTGRES_PASSWORD: #database password
POSTGRES_DB: #database name
SECRET_KEY: #32 digits token - use [it-tools token-generator](https://it-tools.tech/token-generator?length=32) to get one

### Domains

- Service Name: `tandoor`
- Container Port: `80`
- HTTPS: `true`
- Certificate Provider: `Let's Encrypt`

### Volume Backups

- Task Name: `staticfiles`
- Schedule `0 0 * * *`
- Service Name: `tandoor`
- Volume: `tandoor-tandoor-xxx`
- Keep Latest Backups: `7`
- Enabled: true