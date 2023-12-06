![dezor icon 1](imgs/dezor_icon_1.png)
# DEZOR: The web browser including VPN & Adblocker 
[official website](https://www.dezor.net/)
![dezor icon 2](imgs/dezor_icon_2.png)

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
