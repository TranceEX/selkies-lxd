# selkies-lxd-amd64

Selkies setup script for Ubuntu Noble amd64 running inside LXD container.

Based on [Selkies Base Images from LinuxServer](https://github.com/linuxserver/docker-baseimage-selkies/tree/ubuntunoble).

## Setting up
```
git clone --single-branch --branch ubuntunoble-amd64 https://github.com/TranceEX/selkies-lxd.git
cd selkies-lxd
bash setup.kde.sh
```

## Notes

If you intend to use a joystick, you must run `00-lxd-host-joystick.sh` on the LXD host before running the setup script.

## Access
```
http://localhost:3000
https://localhost:3001
```

## Why

I stumbled upon [Chromium - LinuxServer.io](https://docs.linuxserver.io/images/docker-chromium/), which worked flawlessly for my use case.

Curious about how the image was built and how it functioned, I decided to dig deeper and eventually adapted it to run inside an LXD container.

## Todo
- [ ] Fix `Download` function.
- [ ] Remove `proot-app` integration.
- [ ] Cobine the setup scripts into a single interactive script.
