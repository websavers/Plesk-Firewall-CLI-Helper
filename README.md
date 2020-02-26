# Plesk-Firewall-CLI-Helper
 Plesk FIrewall's CLI tools are not great. This helps by emulating how CSF works via CLI

# Installation Instructions
- On Plesk server, ensure you have the Plesk firewall extension enabled
- Via SSH, as root, run: 

```
curl -o /usr/local/bin/pfw https://raw.githubusercontent.com/websavers/Plesk-Firewall-CLI-Helper/master/pfw`
chmod +x /usr/local/bin/pfw
ln -s /usr/local/bin/pfw /usr/bin/pfw
```
Note: The symlink ensures pfw is available as a command by being in the $PATH var.

# Usage

pfw -d [ip] -- blocks an IP address

# Future
We're open to pull requests to add functionality like potentially:
- pfw -r [ip] to remove the IP from the block list
- pfw -a [ip] -p [port] to allow an IP and Port combination