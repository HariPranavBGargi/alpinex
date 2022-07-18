# alpinex
## Docker build
```docker build . -f alpine -t alpinex```
## Docker command
Steps to run the container:
Run ```./dockerrun``` or use the command ```docker run --privileged -v /run/udev/data:/run/udev/data alpinex```
## Points to note
```/run/udev/data``` contains the data of the USB input davices connected to the computer and without attaching the volume, the input devices aren't detected.
If dockerrun fails, check for ```/run/udev/data``` and if not found, run ```./udev``` before running ```./dockerrun```.
