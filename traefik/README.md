# Dockerized Traefik

https://traefik.io

Copy this docker-compose.yml and traefik.toml wherever you'd like and edit as needed. You'll also need an acme.json on your docker host:

```touch /opt/docker/traefik/acme.json && chmod 600 /opt/docker/traefik/acme.json```

Before this will work you will need an external docker network on your docker host that will be shared by other docker services. To create this:

```docker network create web```

To start Traefik, make sure that docker-compose.yml is in your current working directory and:

```docker-compose up -d```