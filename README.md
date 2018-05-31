# Traefik acme test

this should be deployed on a vps with a valid `A` record pointing to it.

on the server...

### Start test

```sh
docker-compose up
```

### Verify

```sh
curl localhost
```

### Inspecting

```sh
docker-compose exec traefik sh
```

check `/config/acme.json` in the container

### Debugging

make changes to `traefik.toml`

kill `docker-compose`

`docker-compose down`

`docker-compose up`
