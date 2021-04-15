# Terraria Server Config

- `terraria.service` -- systemd config for terraria
- `bin` -- helper scripts. store in `/opt/terraria/bin/`, and symlink `TerrariaServer.bin.x86_64` as `/opt/terraria/bin/TerrariaServer`
- `/var/lib/terraria/config` -- server config file, as documented in https://terraria.fandom.com/wiki/Server#Server_config_file
- `/var/lib/terraria/worlds/` -- terraria worlds should be stored here
- `/var/lib/terraria/backup/` -- world backups repo for duplicacy


This repo uses a FIFO in `/tmp/terraria-comms` to communicate with the server. This works a lot better with systemd than using screen.
