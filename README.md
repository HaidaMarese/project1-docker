# Docker Project - WordPress & Hello App

This project runs 4 Docker containers using Docker Compose:

- **nginx**: Acts as a reverse proxy with SSL for two custom domains.
- **wordpress**: CMS site served at `https://wordpress.example.com`
- **mysql**: Database for WordPress (data persists on down)
- **hello-app**: Custom static HTML app served at `https://hello.example.com`

## Features
- Uses images from `ghcr.io`
- Self-signed SSL certs for both domains
- nginx and mysql are on separate networks
- MySQL data persists across shutdowns

## How to Run
1. Clone the repo:
   ```bash
   git clone https://github.com/HaidaMarese/project1-docker.git
   cd project1-docker

## Run the Project

```bash
docker compose up --build
