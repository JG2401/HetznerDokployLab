# [nextcloud](https://nextcloud.com)

## nextcloud

I recommend using the `nextcloud-aio` template as a basis.

### General

- Compose Path: `./projects/nextcloud/docker-compose.yml`

### Environment

- NEXTCLOUD_DOMAIN: 
- MYSQL_SECRET_PASSWORD: 
- MYSQL_SECRET_PASSWORD_ROOT: 

### Domains

- Service Name: `nextcloud`
- Container Port: `80`
- HTTPS: `true`
- Certificate Provider: `Let's Encrypt`

### Volume Backups

- Task Name: `db`
- Schedule `0 0 * * *`
- Service Name: `nextcloud_db`
- Volume: `nextcloud-nextcloudaio-xxx`
- Keep Latest Backups: `7`
- Enabled: true

### Apps (nextcloud-intern)

####  External storage support

Enable `External storage support` and create a new external storage in the admin-settings.

- Foldername: `StorageBox`
- External storage: `local`
- Authentication: `None`
- Configuration: `/mnt/storagebox`
- Available for `All people`
