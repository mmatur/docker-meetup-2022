# Docker Lyon meetup

## Docker

```bash
docker-compose up 
```

## Kubernetes

```bash
k3d cluster create --k3s-arg "--disable=traefik@server:*" \
--agents="2" \
--port 80:80@loadbalancer \
--port 443:443@loadbalancer

kubectl apply -f whoami.yaml
```
