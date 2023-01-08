# system
A collection of system-wide configuration files, i.e. requiring sudo to edit

## deploy the system files
### manually (recommended)
for instance, deploy the `pacman` configuration with
```bash
cd /path/to/goatfiles/system
sudo cp etc/pacman.conf /etc/pacman.conf
```

### with a script (at your own risk)
the [`gssync`](https://github.com/goatfiles/scripts/blob/main/scripts/gssync)
script was made to do exactly this, i.e. taking a file in this repo and moving it
to the root of the host system, the `/` directory, e.g.
- `etc/...` would move to `/etc/...` and become available to the whole system
