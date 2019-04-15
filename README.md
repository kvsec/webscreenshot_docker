# webscreenshot_docker
Docker version of tool https://github.com/maaaaz/webscreenshot
```sh
$ docker build -t webscreenshot . 
Creates webscreenshot directory on hostOS where you can find all the screenshots.
$ docker run -it -v ~/webscreenshot:/webscreenshot/screenshots webscreenshot
```
