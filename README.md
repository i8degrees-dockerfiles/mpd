
# mpd-1

A docker image for `MPD` with support for ALSA and PulseAudio. This container also includes support for `mpdscribble`.

Additionally, this image supports the use of an [ALSA equalization interface](https://github.com/GioF71/mpd-alsa-docker/blob/main/doc/alsa-eq.md). 

## usage

```shell
docker compose up
docker compose down
docker exec -it mpd-1 alsamixer -D equal
```

## TODO

- [ ] verify that Ampache can still access its `mysql` 
database; we have not tested this since relocating its
bind mount into its own volume mount.
  * re-create the database files if non-accessible

## Reference Documents

1. <https://github.com/GioF71/mpd-alsa-docker>
2. <https://hub.docker.com/r/giof71/mpd-alsa>
2. <https://www.musicpd.org/>
3. <https://www.musicpd.org/clients/mpdscribble/>
4. <https://github.com/GioF71/mpd-alsa-docker/blob/main/doc/alsa-eq.md>

