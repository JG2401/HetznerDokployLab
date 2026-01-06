# [jellyseer](https://docs.seerr.dev/)

## jellyseer

### General

- Compose Path: `./projects/jellyseer/docker-compose.yml`

### Environment

- TIMEZONE: #your time zone - for example `Europe/Berlin`

### Domains

- Service Name: `jellyseer`
- Container Port: `5055`
- HTTPS: `true`
- Certificate Provider: `Let's Encrypt`

### Volume Backups

- Task Name: `jellyseer`
- Schedule `0 0 * * *`
- Service Name: `jellyseer`
- Volume: `jellyseer-jellyseer-xxx`
- Keep Latest Backups: `1`
- Enabled: true