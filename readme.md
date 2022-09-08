# Infra

This repository contains my infrastructure as an [Ansible](https://github.com/ansible/ansible) configuration. 

## What is included?

Docker configurations for:

- [Traefik](https://github.com/traefik/traefik)
- [Visual Studio Code Server](https://github.com/coder/code-server)
- [Factorio headless server](https://github.com/factoriotools/factorio-docker)
- [File Browser](https://github.com/filebrowser/filebrowser)
- [Gitea](https://github.com/go-gitea/gitea)
- [Nextcloud](https://github.com/nextcloud/docker)
- [SSH Server for file upload](https://hub.docker.com/r/linuxserver/openssh-server)
- [overseerr](https://github.com/sct/overseerr)
- [Plex](https://hub.docker.com/r/plexinc/pms-docker)
- [Paperless-ngx](https://github.com/paperless-ngx/paperless-ngx)
- [Portainer](https://github.com/portainer/portainer)
- [PsiTransfer](https://github.com/psi-4ward/psitransfer)
- [qBittorrent](https://github.com/qbittorrent/qBittorrent)
- [Docker Registry](https://hub.docker.com/_/registry) with [Docker Registry UI](https://github.com/Joxit/docker-registry-ui)
- [RStudio Server](https://hub.docker.com/r/rocker/rstudio)
- [SheetAble](https://github.com/SheetAble/SheetAble)
- [Tautulli](https://github.com/Tautulli/Tautulli)
- [Uptime Kuma](https://github.com/louislam/uptime-kuma)
- [Portfolio page from my brother](https://github.com/vallezw/AboutMePage)
- [Vaultwarden](https://github.com/dani-garcia/vaultwarden)
- [Watchtower](https://github.com/containrrr/watchtower)

## Installation

This setup is designed to be run on an unRAID server. 
Since unRAID is based on Slackware and doesn't ship package managers by hand, we need to install Python manually.

For this, we need to install the [NerdPack](https://forums.unraid.net/topic/35866-unraid-6-nerdpack-cli-tools-iftop-iotop-screen-kbd-etc/).
Then, we need to install Python by clicking on Settings -> Nerd Pack and selecting Python there.

After that, we need to install the `docker` and `docker-compose` Python packages by running the following commands:

```console
pip3 install --upgrade pip
pip3 install docker docker-compose
```

TODO setup ssh key, run ansible, ...