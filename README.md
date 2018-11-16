Deploy script for answerfamily
======

## Initial setup
1. Make sure the env files are in place: copy all `.sample` files in env-files and rename file to remove `.sample`.
    Update their content.
2. Initialize DB

## Deploy

### Start all service

```bash
$ docker-compose up

# Initialize database
$ docker-compose exec api npm run schema
```

### Update specific service

```bash
$ docker-compose pull <service>
$ docker-compose up -d <service>
```
