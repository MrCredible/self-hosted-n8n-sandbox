# n8n Demo setup

This repo helps setup a docker-compose based setup to quickly bootstrap an n8n demo environment.

### Requirements
- [Docker compose](https://docs.docker.com/compose/)

### Setup
- Clone this repo
- **Optionally** edit the credentials in the `.env` file
- Run `docker compose up -d`, and wait a couple of minutes for all the containers to become healthy.

### Included service endpoints
- [n8n](http://localhost:5678/)
- [Ollama](http://localhost:11434/)
- [Qdrant](http://localhost:6333/dashboard)
- [Infinity](http://localhost:7997/docs)

### Updating
- Run `docker compose pull` to fetch all the latest images
- Run `docker compose create && docker compose up -d` to update and restart all the containers