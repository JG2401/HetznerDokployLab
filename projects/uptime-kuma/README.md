# [Uptime Kuma](https://github.com/louislam/uptime-kuma)

## uptime-kuma

### General

- Compose Path: `./projects/uptime-kuma/docker-compose.yml`

### Domains

- Service Name: `uptime-kuma`
- Container Port: `3001`
- HTTPS: `true`
- Certificate Provider: `Let's Encrypt`

### Notes

- The container persists its data in the `uptime_kuma_data` volume.
- Expose the service through Dokploy using the generated hostname.
- The default web UI is available on port `3001` inside the container.
