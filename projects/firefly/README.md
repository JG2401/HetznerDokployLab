# [firefly](https://www.firefly-iii.org)

## firefly

### General

- Compose Path: `./projects/firefly/docker-compose.yml`

### Environment

- SITE_OWNER: #site owner email-address
- DB_CONNECTION: #db connection type like `mysql` or `postgres`
- DB_HOST: #db hostname
- DB_PORT: #database port - default: `3306`
- DB_DATABASE: #database name
- DB_USERNAME: #database user-name
- DB_PASSWORD: #database password
- STATIC_CRON_TOKEN: #32 digits token - use [it-tools token-generator](https://it-tools.tech/token-generator?length=32) to get one
- APP_ENV: #default: `production`
- APP_KEY: #a base64 php app key - use [Generate Laravel APP_KEY](https://generate-random.org/laravel-key) to get one
- APP_URL: #default: `http://app:8080`
- TRUSTED_PROXIES: default: `"*"`

### Domains

- Service Name: `firefly`
- Container Port: `8080`
- HTTPS: `true`
- Certificate Provider: `Let's Encrypt`

### Volume Backups

- Task Name: `db`
- Schedule `0 0 * * *`
- Service Name: `db`
- Volume: `firefly-firefly-xxx`
- Keep Latest Backups: `7`
- Enabled: true