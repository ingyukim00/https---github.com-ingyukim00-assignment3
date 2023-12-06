# Assignment3 Part2

## Included material

- backend binary, hello-server
  
  `/var/www/backend/hello-server`

- frontend, index.html
  
  `/var/www/my-site/index.html`

- nginx configuration file, hello.conf

  `/etc/nginx/sites-available/hello.conf`

- service file for backend, hello-server.service

  `/etc/systemd/system/hello-server.service`

- config for setting up servers, cloud-config.yml
- example curl commands for testing your server, curl.md
  Run these commands from your host machine, not your server.

## Testing your frontend web1 

```bash
curl http://164.92.95.174
```

## Testing your backend web1 hey

```bash
curl http://164.92.95.174/hey
```

## Testing your backend web1 echo

```bash
curl -X POST -H "Content-Type: application/json" \
  -d '{"message": "Hello from your server"}' \
  http://164.92.95.174/echo
```

## Testing your frontend web2 

```bash
curl http://164.92.108.27
```

## Testing your backend web2 hey

```bash
curl http://164.92.108.27/hey
```

## Testing your backend web2 echo

```bash
curl -X POST -H "Content-Type: application/json" \
  -d '{"message": "Hello from your server"}' \
  http://164.92.108.27/echo
```

## Testing your frontend load balancer IP

```bash
curl http://146.190.1.254
```

## Testing your backend load balancer IP hey

```bash
curl http://146.190.1.254/hey
```

## Testing your backend load balancer IP echo

```bash
curl -X POST -H "Content-Type: application/json" \
  -d '{"message": "Hello from your server"}' \
  http://146.190.1.254/echo
```
