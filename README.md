# mpd_coverwall

Small script to set your wallpaper to the album art of the currently playing
[`mpd`](https://www.musicpd.org/) song. Currently it looks for embedded art
first, and then falls back to a file with a name containing `folder` or `cover`
in the same folder as the music file.

The size depends on the size of the image, and is scaled down to 80% of the
monitor height if too large.

![example](./screenshot.png)

## Dependencies

`imagemagick xrandr xwallpaper mpc`

## Installation

Run the script continuously somewhere. Personally I do this by putting the
following in my `.xinitrc`:

```sh
nohup $HOME/code/mpd_coverwall/mpd_coverwall >/dev/null 2>&1 &
```
