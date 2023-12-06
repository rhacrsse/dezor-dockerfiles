# [DEZOR](https://www.dezor.net/)
It is a web browser including VPN & Adblocker.
This repo is used for dockerfiles to embed the browser inside a container.

## APPIMAGE
Download the app image from [dezor download website section](https://www.dezor.net/#download) or from [repo](https://drive.google.com/file/d/1IqNPAut9uuo9uL9i-SFMjopgGwtwi2ST/view?usp=drive_link).
<!--
``` bash
 ./Dezor-v1.2.9-x86_64.AppImage  --appimage-extract
```
-->

## COMMANDS

``` bash
podman build -t dezor .
xhost +
podman run -it --rm -e DISPLAY -v /run/user/1000/pipewire-0:/tmp/pipewire-0 -e XDG_RUNTIME_DIR=/tmp --net=host --ipc=host --pid=host --name dezor dezor:latest
```
