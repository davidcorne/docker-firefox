# Firefox in Docker

This shows running GUI apps in Docker. Very much based on the description [here](https://dev.to/darksmile92/run-gui-app-in-linux-docker-container-on-windows-host-4kde).

## Running 

You will need some sort of XServer running. Then run these commands:

```
docker build -t firefox .
set-variable -name DISPLAY -value YOUR-IP:0.0
docker run -ti --rm -e DISPLAY=$DISPLAY firefox
```
