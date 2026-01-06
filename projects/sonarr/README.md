# [sonarr](https://sonarr.tv)

## sonarr

### General

- Compose Path: `./projects/sonarr/docker-compose.yml`

### Environment

- TIMEZONE: #your time zone - for example `Europe/Berlin`

### Domains

- Service Name: `sonarr`
- Container Port: `8989`
- HTTPS: `true`
- Certificate Provider: `Let's Encrypt`

### Volume Backups

- Task Name: `sonarr`
- Schedule `0 0 * * *`
- Service Name: `sonarr`
- Volume: `sonarr-sonarr-xxx`
- Keep Latest Backups: `1`
- Enabled: true