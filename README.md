# alpinex
## Docker command
Use the following command to run the container:
```docker run --privileged -v /run/udev/data:/run/udev/data alpinex```
## Points to note
```/run/udev/data``` contains the data of the USB input davices connected to the computer and without attaching the volume, the input devices aren't detected.
