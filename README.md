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

Installation
------------

### Prerequisites

1.  Docker
2.  Docker Compose
3.  Git

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

Support
-------

Please open an issue for support.

* * * * *

This README is a good starting point, but you may want to add more specific instructions or descriptions based on your actual setup. Feel free to modify it to suit your needs.
