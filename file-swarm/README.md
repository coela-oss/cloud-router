# Traefik File provider connect swarm network


## Run

* http://localhost

```
docker compose -p router -f compose.http.yaml up -d
```


* https://localhost

```
docker compose -p router -f compose.https.yaml up -d
```

* https://localhost (basic auth)

```
docker compose -p router \
  -f compose.https.yaml up \
  -f basic-auth/compose.dashboard.yaml -d
```

## Init

* Docker (Swarm mode)
  * `docker swarm init`
* Traefik V3
  * create shared net

    ```
    docker network create -d overlay proxy-net --attachable
    docker network create traefik-public --attachable
    ```

## Config

`config/traefik.toml` is default config in container `/etc/traefik`

Other settings could see `sample/` this repo. 
