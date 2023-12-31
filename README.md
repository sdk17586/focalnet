# focalnet-classification

## Build
```bat
docker build -t dnn_test .
```
## Container
```bat
docker run -it \
    --name dnn_test \
    --privileged \
    --gpus all \
    --network host \
    -e DISPLAY=$DISPLAY \
    -e QT_X11_NO_MITSHM=1 \
    -v /tmp/.X11-unix:/tmp/.X11-unix:rw \
    -v /etc/localtime:/etc/localtime:ro \
    -e TZ=Asia/Seoul \
    -v /dev:/dev \
    -w /root \
    dnn_test:latest
```
## Container_setting
```bat
docker cp
```
