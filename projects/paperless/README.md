# [paperless](https://docs.paperless-ngx.com)

## paperless

### General

- Compose Path: `./projects/paperless/docker-compose.yml`

### Environment

- PAPERLESS_REDIS: #default: `redis://redis:6379`
- PAPERLESS_TIME_ZONE: #local time zone - example: `Europe/Berlin`
- PAPERLESS_ADMIN_USER: 
- PAPERLESS_ADMIN_PASSWORD: 
- PAPERLESS_OCR_LANGUAGE: #example: `deu+eng`
- PAPERLESS_URL: #same as [domains](#domains) host
- PAPERLESS_ALLOWED_HOSTS: 
- PAPERLESS_DBHOST: #db container-name
- PAPERLESS_DBNAME: #default: `paperless`
- PAPERLESS_DBUSER:
- PAPERLESS_DBPASS: #same as db POSTGRES_PASSWORD
- PAPERLESS_OCR_OUTPUT_TYPE:
- PAPERLESS_SECRET_KEY:

### Domains

- Service Name: `paperless`
- Container Port: `8000`
- HTTPS: `true`
- Certificate Provider: `Let's Encrypt`

### Volume Backups

#### db

- Task Name: `db`
- Schedule `0 0 * * *`
- Service Name: `db`
- Volume: `paperless-paperless-xxx`
- Keep Latest Backups: `7`
- Enabled: true