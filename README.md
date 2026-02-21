# Jellyfin sysVinit

This script is to use [Jellyfin](https://github.com/jellyfin/jellyfin) with the service / daemon manager SysVinit.

## How to install

1. follow the instruction [from the official documentation](https://jellyfin.org/docs/general/installation/linux)
2. At the end of the execution you get an error with the service not launched, caused by the systemd not used on this system
3. download the file <https://github.com/Labna/jellyfin-sysvinit/raw/refs/heads/main/jellyfin>
4. move it to `/etc/init.d/jellyfin`  
   exemple `sudo mv jellyfin /etc/init.d/`
5. change the settings of your Jellyfin instance in `/etc/defaults/jellyfin`
6. Update the service list `sudo update-rc.d jellyfin defaults`
7. Finally start your server `sudo service jellyfin start`
8. You may can access via the url <http://127.0.0.1:8096>
