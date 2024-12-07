React documentation for [Docker](https://hub.docker.com/r/wcjiang/react.dev)
===

This repository provides the official React documentation, now available for deployment via Docker. This makes it convenient for local viewing and learning.

<!--rehype:ignore:start-->
[![CI](https://github.com/uiwjs/react.dev-for-docker/actions/workflows/ci.yml/badge.svg)](https://github.com/uiwjs/react.dev-for-docker/actions/workflows/ci.yml)
[![Docker Image Version (latest by date)](https://img.shields.io/docker/v/wcjiang/react.dev)](https://hub.docker.com/r/wcjiang/react.dev)
[![Docker Image Size (latest by date)](https://img.shields.io/docker/image-size/wcjiang/react.dev)](https://hub.docker.com/r/wcjiang/react.dev)
[![Docker Pulls](https://img.shields.io/docker/pulls/wcjiang/react.dev)](https://hub.docker.com/r/wcjiang/react.dev)
[![GitHub last commit](https://img.shields.io/github/last-commit/reactjs/react.dev?style=flat&label=react.dev)](https://github.com/reactjs/react.dev/commits)
<!--rehype:ignore:end-->

## Introduction

The new [React documentation](https://github.com/reactjs/react.dev) supports Docker deployment, making it easy to run and explore the documentation locally. This Docker image includes all the necessary dependencies and configurations to get you started quickly.

## Getting Started

To pull the latest Docker image for the React documentation, run the following command:

```bash
docker pull wcjiang/react.dev:latest
```

To run the Docker container, use the following command:

```bash
docker run --name react.dev \
  -p 60009:3000 \
  --restart=always \
  -d wcjiang/react.dev:latest
```

This will start the React documentation server on port 3000, accessible via `http://localhost:60009`.

## License

MIT © [Kenny Wong](https://github.com/jaywcjlove)
