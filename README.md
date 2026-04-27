# edge-web-01
Proxy &amp; SSL Config

# ops-config-webserver (edge-web-01)

## Description
Configuration repository for the Edge/Front-end layer. Manages the entry point for all user traffic, SSL termination, and load balancing.

## Stack
- **Service:** Nginx / Apache
- **Security:** Certbot (Let's Encrypt), UFW Firewall

## Key Configurations
- `nginx.conf`: Reverse proxy rules to route `/api` to `proc-gpu-01` and `/db` requests to `data-sql-01`.
- `ssl/`: Certificate management scripts.

## Connectivity
- **Public Port:** 80, 443
- **Internal Network:** 192.168.56.20
