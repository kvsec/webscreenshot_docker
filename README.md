# webscreenshot_docker
Docker version of tool https://github.com/maaaaz/webscreenshot

Build
```sh
$ docker build -t webscreenshot . 
```
Creates webscreenshot directory on hostOS where you can find all the screenshots.
```sh
$ docker run -it -v ~/webscreenshot:/webscreenshot/screenshots webscreenshot
```
After you run the container, be sure to enter the following commands:
```sh
$ export DISPLAY=':99.0'
$ Xvfb :99 -screen 0 1024x768x24 > /dev/null 2>&1 &
```
To change user-agent or resolution if you need so, check the .js file.
