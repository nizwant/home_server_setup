# How to setup home server (old guide - first iteration)

1. Download ubuntu desktop on machine
2. figure out how to add ssh server (tricky) - next i will have to download ubuntu server (or even nix)
3. connect from mac
4. add ssh key with `ssh-copy-id`
5. Download docker
6. configure jellyfin as in this guide [jellyfin config](https://pimylifeup.com/jellyfin-docker/)
7. Turn of systemd dns with by editing the `/etc/systemd/resolved.conf`: `DNSStubListener=no` then restart with `service systemd-resolved restart`
8. configure PiHole as in this guide [pihole git](https://github.com/pi-hole/docker-pi-hole?tab=readme-ov-file)
9. Update router to point at pihole as dns
10. add new blacklisted websites from [firebog](https://v.firebog.net/hosts/lists.php)
11. add them to adlist in pihole and run in pihole container `pihole -g`
12. configure caddy to point at jellyfin, pihole ui etc.
13. create local domain name for it in pihole
