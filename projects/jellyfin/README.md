# [jellyfin](https://jellyfin.org)

## jellyfin

### General

- Compose Path: `./projects/jellyfin/docker-compose.yml`

### Environment

- TIMEZONE: #your time zone - for example `Europe/Berlin`

### Domains

- Service Name: `jellyfin`
- Container Port: `8096`
- HTTPS: `true`
- Certificate Provider: `Let's Encrypt`

### Volume Backups

- Task Name: `jellyfin`
- Schedule `0 0 * * *`
- Service Name: `jellyfin`
- Volume: `jellyfin-jellyfin-xxx`
- Keep Latest Backups: `1`
- Enabled: true