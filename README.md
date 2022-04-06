# Setup Odoo13 via Docker with pgAdmin access


## Installation (Docker):
```bash
$ sudo apt install docker.io
$ sudo systemctl start docker
$ sudo systemctl enable docker
```

## Installation (Docker Compose):
```bash
$ sudo curl -L "https://github.com/docker/compose/releases/download/1.23.1/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
$ sudo chmod +x /usr/local/bin/docker-compose
$ sudo systemctl enable docker
```

## Start the container:
```bash
$ docker-compose up  -d
```

Then locate `localhost:18069` to access your Odoo 13.0.

## Access development logs:
```bash
$ docker-compose logs -f -t --tail 100
```
