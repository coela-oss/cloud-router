# Cloud Router

Finding the best practice of edge routing with docker swarm &amp; traefik.

## Status

The structure is changed for each directory.

### file-swarm 

Use File provider and Swarm provider.

Run a standalone docker container with file provider to proxy swarm overlay network.

### swarm-only (wip)

Use Swarm provider only.

Swarm cluster include traefik container routing all service.

Work in progress but this structure may not work in traefik V3 yet...
