# Random Wallpaper Display
A minimalist, high-definition web wallpaper built for **Wallpaper Engine**, powered by the **Wallhaven API**. 

Even though this wallpaper is designed for Wallpaper Engine, it works perfectly in any modern browser as a standalone dynamic webpage.

## Features
- **Automated Sync**: Refreshes automatically at the top of every hour, synced to your system clock.
- **Smooth Transitions**: Features a 1-second ease-in-out crossfade when switching images.

## Using with Wallpaper Engine

### Creating the Wallpaper
1. Open the **Wallpaper Engine Editor**.
2. Click on **Create Wallpaper** and select the `index.html` file.

For more details, refer to the [official guide](https://docs.wallpaperengine.io/en/web/first/gettingstarted.html).


## Force Refresh Image
If you want to skip the current image and fetch a new one immediately you have two options, double click or using the console.

For details about the debugger, refer to the [official guide](https://docs.wallpaperengine.io/en/web/debug/debug.html).

To access the developer tools while the wallpaper is running inside Wallpaper Engine:
1. Enable the **Web Wallpaper Debugging** feature in Wallpaper Engine.
2. Open your browser and navigate to your debug port (default is `http://localhost:8080`).

### Direct Interaction
Simply **double-click** anywhere on the wallpaper.

### Using the Console
1. Open the **Console** tab in DevTools.
2. Type the following command and press Enter:
   ```js
   forceRefresh()
   ```

## Changing the wallpaper API parameters
By default, it's set to always use wallpapers from the Nature Landscape category (tag ID `41`) and with image resolution of at least `1920x1080`.

If you wish you change it, you can modify the API URL parameters.

This is the default URL used in the code:
```
https://wallhaven.cc/api/v1/search?q=id:41&categories=100&purity=100&sorting=random&atleast=1920x1080
```

For more details of each parameters, refer to the [official API help](https://wallhaven.cc/help/api).
