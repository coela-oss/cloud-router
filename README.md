# Cloud Router

Finding the best practice of edge routing with docker swarm &amp; traefik.

## Run

```
docker compose -p router -f compose.yaml up -d
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

* TODO

## Memo:

pattern

* Traefik
  * Dashboard
* Place(Domain)
  * Local,Server
