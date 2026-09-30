# Docker Compose Guide

## The Compose File

The `docker-compose.yml` file defines a two-tier Nextcloud stack: a MariaDB database and a Nextcloud application.

## What does the `services:` block do?

The `services:` block lists every container that makes up the application. Each entry under it (`database` and `app`) becomes one container, with its own image, ports, and environment variables. Compose also puts all services on a shared network automatically, so they can talk to each other.

## How did the Nextcloud container find the database?

The `MYSQL_HOST=database` environment variable tells Nextcloud which host to connect to. `database` is the name of the service in the Compose file. Compose's built-in DNS resolves that service name to the database container's IP address on the shared network, so no IP address had to be written by hand.

## docker run vs. docker-compose up -d

| `docker run` | `docker-compose up -d` |
|---|---|
| Starts a single container per command | Starts every service defined in the YAML file at once |
| Options are typed manually each time | Configuration is saved in a reusable file (Infrastructure as Code) |
| Networking must be set up manually | A shared network is created automatically |
| Easy to make typos or forget options | Repeatable, versionable, and easy to share |

The `-d` flag runs the containers in the background (detached mode).
