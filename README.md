# Forestracks Pterodactyl Installer
Pterodactyl Panel installer for Forestracks customers. This installer works on both Ubuntu and CentOS. Please carefully read all options for the best experience.

## Installation:
1) Reinstall your machine if you changed anything before you run the installer.
2) Download and run installer:
```
wget https://raw.githubusercontent.com/ForestRacks/pterodactyl-installer/main/install.sh
chmod +x install.sh
./install.sh
```
## Post Installation:
* Note - YourFQDN.TLD refers to the FQDN you set during the installation process.
1) Go to http://YourFQDN.TLD/admin/locations and make a location
2) Go to http://YourFQDN.TLD/admin/nodes and create your first machine
3) Go to http://YourFQDN.TLD/admin/nodes/view/1/allocation and add ports for your games
4) Go to http://YourFQDN.TLD/admin/nodes/view/1/configuration and grab the block of text
5) Then paste the configuration you copied in `/etc/pterodactyl/config.yml` on your machine
6) Lastly, do `systemctl restart wings` and you should be all set

## Troubleshooting:
1) If you get a mysql connection error when you run the installer, you mostly ran the installer multiple times. The easiest way of fixing this is reinstalling your OS and running the install script again.
2) If you get Let's Encrypt SSL generation errors, you might be using an IP address as your FQDN and Let's Encrypt only generates SSLs for domains.

## Coming Soon:
1) Cloudflare Proxy option
2) Improve Firewall
3) Enable Swap

## Contributors ✨

Created and maintained by:
1) [Zinidia](https://github.com/Zinidia)
2) [Neon](https://github.com/DeveloperNeon)
3) [Vilhelm Prytz](https://github.com/vilhelmprytz)
4) [sam1370](https://github.com/sam1370)
5) [Linux123123](https://github.com/Linux123123)
