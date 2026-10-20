# [seer](https://docs.seerr.dev/)

## seer

### General

- Compose Path: `./projects/seer/docker-compose.yml`

### Domains

- Service Name: `seer`
- Container Port: `5055`
- HTTPS: `true`
- Certificate Provider: `Let's Encrypt`

### Volume Backups

- Task Name: `seer`
- Schedule `0 0 * * *`
- Service Name: `seer`
- Volume: `seer-seer-xxx`
- Keep Latest Backups: `1`
- Enabled: true