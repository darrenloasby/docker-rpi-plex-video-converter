Raspberry PI - Plex Video converter - Docker Image
==================================================
[![latest release](https://img.shields.io/github/release/jaymoulin/docker-rpi-plex-video-converter.svg "latest release")](http://github.com/jaymoulin/docker-rpi-plex-video-converter/releases)

This image purpose is to convert unsupported video files by Plex for Raspberry to mp4 which is supported.

Just run the container to convert all avi files recursively with your Raspberry Pi though the `media` volume :

```
docker run --rm -t -v /path/to/your/media/folder:/media jaymoulin/rpi-plex-video-converter
```

This image also exists for PC so your videos can be converted quicker using a more powerful machine

```
docker run --rm -t -v /path/to/your/media/folder:/media jaymoulin/rpi-plex-video-converter:pc
```

Appendixes
---

### Install RaspberryPi Docker

If you don't have Docker installed yet, you can do it easily in one line using this command
 
```
curl -sSL "https://gist.githubusercontent.com/jaymoulin/e749a189511cd965f45919f2f99e45f3/raw/0e650b38fde684c4ac534b254099d6d5543375f1/ARM%2520(Raspberry%2520PI)%2520Docker%2520Install" | sudo sh && sudo usermod -aG docker $USER
```
