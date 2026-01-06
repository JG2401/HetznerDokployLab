# [vaultwarden](https://github.com/dani-garcia/vaultwarden)

## vaultwarden

### General

- Compose Path: `./projects/vaultwarden/docker-compose.yml`

### Environment

- SIGNUPS_ALLOWED: #set it `true` for initial deployment BUT set it `false` afterwards and redeploy.
- DOMAIN: #your vaultwarden domain - for example `https://vaultwarden.example.com`
- ADMIN_TOKEN #your secret admin token to access the admin panel

### Domains

- Service Name: `vaultwarden`
- Container Port: `80`
- HTTPS: `true`
- Certificate Provider: `Let's Encrypt`

### Volume Backups

- Task Name: `vaultwarden`
- Schedule `0 0 * * *`
- Service Name: `vaultwarden`
- Volume: `vaultwarden-vaultwarden-xxx`
- Keep Latest Backups: `7`
- Enabled: `true`