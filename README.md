# Setting up GitLab

GitLab deployment with integrated PostgreSQL and Redis.

## Requirements

* [Docker](https://www.docker.com) and [Docker Compose](https://docs.docker.com/compose).
* Port 22 is available (for convenience when specify Git remotes' url).
* [nginx-proxy](https://github.com/jwilder/nginx-proxy) to act as a reverse proxy.

## Installation

```sh
cp env/postgresql.env.example env/postgresql.env
cp env/gitlab.env.example env/gitlab.env

# Edit configuration files for your own need

# For nginx-proxy's virtual-host settings, kindly refer to:
# https://github.com/jwilder/nginx-proxy#usage

# For GitLab settings, kindly refer to:
# https://github.com/sameersbn/docker-gitlab#available-configuration-parameters

docker-compose up -d
```

## Upgrade

Please refer to instruction [here](https://github.com/sameersbn/docker-gitlab#upgrading).

## License

MIT licensed.
