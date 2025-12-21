# [n8n](https://n8n.io)

## n8n

### General

- Compose Path: `./projects/n8n/n8n.yml`

### Environment

- N8N_HOST: same as host in #[domains](#domains)
- N8N_PORT: #default `5678`
- N8N_PROTOCOL: #default: `http`
- NODE_ENV: #default: `production`
- WEBHOOK_URL: #default: `https://${N8N_HOST}/`
- GENERIC_TIMEZONE: #local time zone - example: `Europe/Berlin`
- N8N_SECURE_COOKIE: #default `false`

### Domains

- Service Name: `n8n`
- Container Port: `5678`
- HTTPS: `true`
- Certificate Provider: `Let's Encrypt`