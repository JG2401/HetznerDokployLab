# [gitea](https://about.gitea.com/)

## gitea

### General

- Compose Path: `./projects/gitea/docker-compose.yml`

### Environment

- USER_UID: #for example `1000`
- USER_GID: #for example `1000`
- DISABLE_REGISTRATION: #should be set to `true` after initial registration

### Domains

- Service Name: `gitea`
- Container Port: `3000`
- HTTPS: `true`
- Certificate Provider: `Let's Encrypt`

### Volume Backups

- Task Name: `gitea-sqlite`
- Schedule `0 0 * * *`
- Service Name: `gitea`
- Volume: `gitea-giteasqlite-xxx`
- Keep Latest Backups: `5`
- Enabled: true