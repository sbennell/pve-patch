# pve-patch

Removes subscription dialogs, replaces enterprise repository with non-subscription repository and replaces branding. Tested on PVE 66.1-8.

## Note

Use at your own risk! Read the script before you run it. 

## Install

1. Connect to node via SSH
2. Run

```bash
# if root
wget -qO - https://raw.githubusercontent.com/sbennell/pve-patch/master/patch.sh | bash

# if non-root
wget -qO - https://raw.githubusercontent.com/sbennell/pve-patch/master/patch.sh | sudo bash
```

## Restore

Enterprise repository

```
mv /etc/apt/sources.list.d/pve-enterprise.list~ /etc/apt/sources.list.d/pve-enterprise.list
```
