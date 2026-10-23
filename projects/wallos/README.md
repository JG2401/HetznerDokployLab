# [Wallos](https://github.com/ellite/Wallos)

## Wallos

### General

- Compose Path: `./projects/wallos/docker-compose.yml`

### Domains

- Service Name: `wallos`
- Container Port: `80`
- HTTPS: `true`
- Certificate Provider: `Let's Encrypt`

### Volume Backups

- Service Name: `wallos`
- Volumes: `wallos-wallos_db-xxx`, `wallos-wallos_logos-xxx`
- Keep Latest Backups: `7`
- Enabled: `true`
