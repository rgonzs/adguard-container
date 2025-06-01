# ADGUARD

Create the syslink to the systemd rootless user directory, if not exits create it with:
```shell
mkdir -p $HOME/.config/containers/systemd/

ln -s $(pwd)/adguard.container $HOME/.config/containers/systemd/
```
Reload the systemd units with
```shell
systemctl --user daemon-reload
```


