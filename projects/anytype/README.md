# [Anytype](https://anytype.io)

## anytype

### General

- Compose Path: `./projects/anytype/docker-compose.yml`

### Environment

- SERVER_IP: `123.123.123.123`

### Domains

- Service Name: `anytype`
- Container Port: `8443`
- HTTPS: `true`
- Certificate Provider: `Let's Encrypt`

### Notes

- The container stores its data in the `anytype_data` volume.
- Expose your service through Dokploy with the configured host and port.
- Adjust the environment values to match your deployment and public URL.
