# Consul Local Setup

## Prerequisites

1. Create Docker network:
   ```bash
   docker network create project_network
   ```

2. Add DNS entry to hosts file:
   ```bash
   echo "127.0.0.1 consul.local" >> /etc/hosts
   ```

## Docker Commands Reference

### Network Management

```
docker network list
docker network create project_network
docker network inspect project_network

docker save -o config-service-app-1.0.0.tar config-service-app:1.0.0
docker load -i config-service-app-1.0.0.tar
```