# check_luks

## is_luks

Check if a list of devices are encrypted with LUKS. Raise an error if not.
Return OK is no device is provided. The device argument can be repeated.

```
command[check_luks_devices]=/usr/bin/sudo -u root /opt/ovh-nagios-plugins/bin/check_luks --device /dev/mapper/vg-data is_luks
```
