# home_server_setup

This is repository that contains setup for my home server, goal it to easily reproduce current setup and store in
one place knowledge about it's state.

## ToDo list

- [ ] unattended-upgrades turn on in startup script
- [ ] clean docker compose files that are used right now on server
- [ ] test if new caddy config is working
- [ ] make samba work from inside docker - maybe not, just describe in a good way how to setup samba directly on server
- [ ] do a tailwind configuration from inside docker - maybe not, just describe it good and do a startup on restart
- [ ] research power usage optimization script
- [ ] download of my dot files config from my repo/ git config prompt etc and implement them at the startup
- [ ] research what is username, servername, name etc. in linux setup
- [ ] try to modify fan behavior - enable in bios

## List of currently running services

- samba server
- tailwind
- pi-hole
- caddy
- dozzle
- librespeed
- the arr stack
  - qbit
  - jackett
  - sonarr
  - radarr
  - jellyfin

## Services and functionalities I'm planning on implementing

- mature observability stack - grafana, prometheus
- backup of mobile to samba?
- samba in completed torrent downlands folder
- vaultwarden / bitwarden
- nextcloud
- bazarr
- flaresolverr
- jellyseerr
