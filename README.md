![dezor icon 1](imgs/dezor_icon_1.png)
# DEZOR: The web browser including VPN & Adblocker 
[official website](https://www.dezor.net/)
![dezor icon 2](imgs/dezor_icon_2.png)

## COMMANDS
``` bash
podman build -t dezor .
xhost +
podman run -it --rm -e DISPLAY -v /run/user/1000/pipewire-0:/tmp/pipewire-0 -e XDG_RUNTIME_DIR=/tmp --net=host --ipc=host --pid=host --name dezor dezor:latest
```
