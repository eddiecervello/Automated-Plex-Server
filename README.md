Automated Plex Server
=====================

An all-in-one solution for a Plex media server with automatic downloading, management, and reverse proxy capabilities. This repository leverages Docker and Docker Compose to create a seamless and easy-to-use platform for managing your home media.

Features
--------

-   Plex Media Server: Your own personal Netflix, but better.
-   Nginx Proxy Manager: Easily route traffic to your various services with a web UI.
-   qBittorrent: Torrent client with a web UI.
-   Sonarr: TV series management.
-   Radarr: Movie management.
-   Prowlarr: Unified indexer management.
-   AutoBrr: Automated downloading based on your criteria.
-   Bazarr: Download subtitles for your movies and TV shows.
-   Overseerr: Request manager for new content.
-   Portainer: Docker UI for container management.
-   DuckDNS: Dynamic DNS service.
-   Tautulli: Plex Monitoring and tracking what has been streamed.
-   Watchtower: Automatic Docker container updates.

![image](https://github.com/eddiecervello/Automated-Plex-Server/assets/17179138/6ce759d5-2018-41dc-92b9-9c586a41d49b)

Quick Start Guide
-----------------

1.  Clone this repository: `git clone https://github.com/eddiecervello/automated-plex-server.git`
2.  Change into the directory: `cd automated-plex-server`
3.  Rename `docker-compose.yml.sample` to `docker-compose.yml`.
4.  Edit `docker-compose.yml` to add your own settings and secrets.
5.  Run the Docker Compose file: `docker-compose up -d`
6.  Open the Nginx Proxy Manager dashboard to start routing traffic to your services.

Installation
------------

### Prerequisites

-   Docker
-   Docker Compose
-   Git

### Steps

1.  Clone this repository:

    `git clone https://github.com/eddiecervello/automated-plex-server.git`

2.  Change into the directory:

    `cd automated-plex-server`

3.  Rename `docker-compose.yml.sample` to `docker-compose.yml`.

4.  Edit `docker-compose.yml` to add your own settings and secrets.

5.  Run the Docker Compose file:

    `docker-compose up -d`

Configuration
-------------

After the services are up, you'll need to configure each one. Detailed instructions can be found in the `docs/` folder for each service.

Updates
-------

To update, simply pull the latest version of this repository and run `docker-compose up -d` again.

Security
--------

Please note that the current Docker Compose configuration may expose various services and ports. Make sure to review your firewall settings and understand the implications.

FAQ
---

### How do I update a specific service?

You can update a specific service using the following command:

`docker-compose up -d <service-name> `

Troubleshooting
---------------

If you encounter issues, please check the following:

-   Make sure all environment variables in `docker-compose.yml` are set.
-   Check the logs for each Docker container: `docker logs <container_name>`

Acknowledgments
---------------

Special thanks to all the open-source projects that make this setup possible.

Support
-------

Please open an issue for support.
