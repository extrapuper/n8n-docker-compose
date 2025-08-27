# N8N with Nginx Reverse Proxy

This is a Docker Compose setup that runs N8N behind an Nginx reverse proxy.

## Overview

- N8N runs internally on port 5678
- Nginx acts as reverse proxy on port 80
- All services run in Docker containers

## Quick Start

1. Clone the repository:
   ```bash
   git clone https://github.com/extrapuper/n8n-docker-compose.git
   cd n8n-docker-compose
   ```

2. Start the services:
   ```bash
   docker-compose up -d
   ```

3. Access N8N at: http://localhost

## Configuration

- `docker-compose.yml` - Service definitions and environment variables
- `nginx/default.conf` - Nginx reverse proxy configuration

## Management

Stop services:
```bash
docker-compose down
```

Stop and remove data:
```bash
docker-compose down -v
```

View logs:
```bash
docker-compose logs n8n
docker-compose logs nginx
```
