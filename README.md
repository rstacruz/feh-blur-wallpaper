# feh-blur

Blur your feh wallpaper. Runs as a service, blurring any wallpaper set by feh.

Based on [ganifladi/blurme](https://github.com/ganifladi/blurme).

## Usage

```sh
# Step 1: set a wallpaper using feh
feh --bg-fill "/path/to/yourwallpaper"

# Step 2: run the feh-blur service
feh-blur & disown
```
