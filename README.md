# lazy-smartctl
lazy-smartctl only output problems not all info


Use lazy-smartctl with the same options as you would use smartctl

Example:
lazy-smartctl -a /dev/sda

Example for all devices:
for i in $(lsblk -ndp -e 7 -o NAME) ; do lazy-smartctl -a $i ; done
