# Backup & Restore
It is highly recommended to make regular backups of your OnMyShelf instance.

## Backup with docker project
To backup OnMyShelf database, run the following command:
```bash
docker compose exec server oms-backup
```

Or using docker command:
```bash
docker exec <CONTAINER_NAME> oms-backup
```

The database dump file is stored in `volumes/backups` folder.

It's also highly recommended to backup your `volumes/media` folder.

## Backup with custom installs
You need to dump the database and backup the media folder.

## Restore
You just need to restore the database.