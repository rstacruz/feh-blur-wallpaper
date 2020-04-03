<p align='center'>
<br>
<a href='https://raw.githubusercontent.com/ngynLk/feh-blur-wallpaper/master/untitled.gif'>
<img src='https://raw.githubusercontent.com/ngynLk/feh-blur-wallpaper/master/untitled.gif' width='400'>
</a>
<br>

</p>

<h1 align='center'>
feh-blur-wallpaper
</h1>

<p align='center'>
<em>ngynLk's fork : Blur your desktop wallpaper when windows are open (Linux)</em>
</p>

<p align='center'>
<img src='https://img.shields.io/badge/build-pending-lightgrey.svg'>
</p>

<br>

Blurs your desktop wallpaper when windows are open.
This is a fork, with added support for minimized/activated windows: if you minimize your windows in openbox for example, your wallpaper also blurs!
Runs as a service, blurring any wallpaper set by [feh].
Works great with [i3wm], but should work with any Linux window manager! 🎉

## Usage

Run `feh-blur`. (Tip: optionally, you can pass `-d` to it to run it in the background.)

```sh
# Step 1: run the feh-blur service
$ feh-blur

 >> Monitoring changes
    feh-blur will now blur any wallpapers set using 'feh'.

 >> Found wallpaper
    /home/rsc/wallpapers/unsplash.jpg
    Generating blurred images... done.
```

Set a wallpaper using [feh]. You can do this before starting feh-blur, or while feh-blur is running.

```
feh --bg-fill "/path/to/yourwallpaper.jpg"
```

See `feh-blur --help` for full usage options.

```
Usage: feh-blur [-v|--verbose]

Options:
  -b, --blur N            set blur strength to N (4...128, default 32)
      --darken N          darken image by N (4...100, default 32)
      --lighten N         lengthen image by N (4...100, default 0)
  -c, --uncontrast        reduce contrast
      --save-image PATH   save blurred image to PATH
      --no-animate        skip fading animation

Daemon options:
  -d, --daemon            run in background
  -s, --stop              stop previously-ran daemon

Other options:
  -v, --verbose           show more messages
  -q, --quiet             supress messages
```

## Installation

Install [feh-blur](./feh-blur) somewhere. You may also need some dependencies, install them using your Linux distro's appropriate package manager.

```sh
# Arch Linux
sudo pacman -S wmctrl graphicsmagick feh

# Ubuntu and alike
sudo apt install wmctrl graphicsmagick feh
```

## Prior art

Based on [ganifladi/blurme](https://github.com/ganifladi/blurme). feh-blur-wallpaper has been written from the ground up, using some parts of blurme as reference.

## Thanks

**feh-wallpaper-blur** © 2019, Rico Sta. Cruz. Released under the [MIT] License.<br>
Authored and maintained by Rico Sta. Cruz with help from contributors ([list][contributors]).

> [ricostacruz.com](http://ricostacruz.com) &nbsp;&middot;&nbsp;
> GitHub [@rstacruz](https://github.com/rstacruz) &nbsp;&middot;&nbsp;
> Twitter [@rstacruz](https://twitter.com/rstacruz)

[![](https://img.shields.io/github/followers/rstacruz.svg?style=social&label=@rstacruz)](https://github.com/rstacruz) &nbsp;
[![](https://img.shields.io/twitter/follow/rstacruz.svg?style=social&label=@rstacruz)](https://twitter.com/rstacruz)

[mit]: http://mit-license.org/
[contributors]: http://github.com/rstacruz/feh-wallpaper-blur/contributors
[feh]: https://wiki.archlinux.org/index.php/feh
[i3wm]: https://i3wm.org/
