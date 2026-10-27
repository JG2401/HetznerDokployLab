# [ntfy](https://ntfy.sh)

## ntfy

### General

- Compose Path: `./projects/ntfy/docker-compose.yml`

### Environment

- NTFY_HOST: `https://ntfy.example.com`
- HTTP_PORT: `80`
- TZ: `Europe/Berlin`

### Domains

- Service Name: `ntfy`
- Container Port: `80`
- HTTPS: `true`
- Certificate Provider: `Let's Encrypt`

### Notes

- ntfy stores persistent state in the `ntfy_data` volume.
- Set `NTFY_BASE_URL` to the public URL used by your reverse proxy.
- If you want authentication, configure the ntfy auth db or add a custom wrapper config.
