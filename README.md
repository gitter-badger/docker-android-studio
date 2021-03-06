 [![](https://badge.imagelayers.io/yongjhih/android-studio:latest.svg)](https://imagelayers.io/?images=yongjhih/android-studio:latest)

## Usage

```sh
docker run -it \
  --privileged
  -v $HOME/AndroidStudioProjects:/home/ubuntu/AndroidStudioProjects \
  -v $HOME/.android:/home/ubuntu/.android \
  -v $HOME/.AndroidStudioPreview2.0:/home/ubuntu/.AndroidStudioPreview2.0 \
  -v /dev/bus/usb:/dev/bus/usb \
  -v /dev/kvm:/dev/kvm \
  -v $ANDROID_HOME:/opt/android-sdk \
  -e DISPLAY=$DISPLAY \
  -v /tmp/.X11-unix:/tmp/.X11-unix \
  -v $XAUTHORITY:/home/ubuntu/.Xauthority \
  --net host \
  yongjhih/android-studio
```

## Usage with docker-compose

```
docker-compose up
```

## Ref.

* Download: [2.0 beta 2] (https://dl.google.com/dl/android/studio/ide-zips/2.0.0.11/android-studio-ide-143.2586769-linux.zip)
* http://tools.android.com/download/studio
* http://tools.android.com/download/studio/stable
* http://tools.android.com/download/studio/beta
* http://tools.android.com/download/studio/canary
