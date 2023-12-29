Small script to set your wallpaper to the album art of the currently playing
[`mpd`](https://www.musicpd.org/) song.

![example](./screenshot.png)

# Dependencies

`imagemagick xrandr xwallpaper mpc`

# Installation

Run the script continuously somewhere. Personally I do this by putting the
following in my `.xinitrc`:

```sh
nohup $HOME/code/mpd_coverwall/mpd_coverwall >/dev/null 2>&1 &
```
