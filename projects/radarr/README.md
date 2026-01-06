# [radarr](https://radarr.video)

## radarr

### General

- Compose Path: `./projects/radarr/docker-compose.yml`

### Environment

- TIMEZONE: #your time zone - for example `Europe/Berlin`

### Domains

- Service Name: `radarr`
- Container Port: `7878`
- HTTPS: `true`
- Certificate Provider: `Let's Encrypt`

### Volume Backups

- Task Name: `radarr`
- Schedule `0 0 * * *`
- Service Name: `radarr`
- Volume: `radarr-radarr-xxx`
- Keep Latest Backups: `7`
- Enabled: `true`