# Sandyk server image

The public Docker image of the [Sandyk](https://sandyk.app) server:

```sh
docker run -d --name sandyk --restart unless-stopped \
  -p 8080:8080 -v sandyk-data:/data \
  ghcr.io/keremet-dev/sandyk
```

Instructions — installing with Docker, docker compose or Home Assistant, the first account,
access from outside, backups and updates: https://sandyk.app/server/ (по-русски:
https://sandyk.app/ru/server/).

Platforms: `linux/amd64`, `linux/arm64`, `linux/arm/v7`. Tags: the version (`0.3.0`) and
`latest` for the newest one.

This repository holds no source code: a workflow republishes each release of the server image
here, unchanged. Questions and problems: support@sandyk.app.
