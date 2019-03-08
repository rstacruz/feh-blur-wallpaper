<p align='center'>
<br>
<a href='https://user-images.githubusercontent.com/74385/54021387-03d57c80-41cb-11e9-8015-2352778271d9.gif'>
<img src='https://user-images.githubusercontent.com/74385/54021387-03d57c80-41cb-11e9-8015-2352778271d9.gif' width='400'>
</a>
<br>

</p>

<h1 align='center'>
feh-blur-wallpaper
</h1>

<p align='center'>
Blur your desktop wallpaper when windows are open. Runs as a service, blurring any wallpaper set by [feh]. Works great with [i3], but should work with any window manager (!).
</p>

<p align='center'>
<img src='https://img.shields.io/badge/build-pending-lightgrey.svg'>
</p>

<br>

## Usage

Run `feh-blur`. (Tip: optionally, you can pass `-d` to it to run it in the background.)

```sh
# Step 1: run the feh-blur service
feh-blur [-d]
```

Set a wallpaper using [feh]. You can do this before starting feh-blur, or while feh-blur is running.

```
feh --bg-fill "/path/to/yourwallpaper.jpg"
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

[feh]: https://wiki.archlinux.org/index.php/feh
[i3]: https://i3wm.org/

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
