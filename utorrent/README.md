[appurl]: http://www.utorrent.com/
[![uTorrent](http://www.utorrent.com/img/logos/utorrent.png)][appurl]

## Usage

### Volumes:

* `<path to data>:/data`
where utorrent should store config files and logs
* `<path to watch folder>:/utorrent`
watch folder for torrent files

### Variables:

* `PUID=<uid>`
See below for explanation
* `PGID=<gid>`
See below for explanation
* `TZ=<timezone>`
e.g. Europe/London

### Ports:
* 8080:8080
* 6881:6881

### User / Group Identifiers

Sometimes when using data volumes, permissions issues can arise between the host OS and the container. We avoid this issue by allowing you to specify the user `PUID` and group `PGID`. Ensure the data volume directory on the host is owned by the same user you specify and it will "just work" ™.

## Setting up the application

Webui is on port 8080
