# Cardinal-Anticheat

<img src="http://167.86.120.207/img/banner.png">

<div align="center">
[![Discord](https://img.shields.io/discord/463752820026376202.svg?label=&logo=discord&logoColor=ffffff&color=7389D8&labelColor=6A7EC2)](https://discord.gg/zxSwN8Z)
</div>

## Disclaimer

Cardinal-Anticheat is a **free** [**Spigot**](https://github.com/SpigotMC) anticheat which blocks most of the known cheats out there. Keep in mind, that Cardinal-Anticheat is still in beta, false postives may occurre...

## Installation

First navigate to the [**release**](https://github.com/Clientastisch/Cardinal-Anticheat/releases) tab and download the newest version available. After the download move the `CAC.jar` into the `plugins` folder. The `CACApi.jar` **is only for development purpose** and should not be moved inside the `plugins` folder too.

## Addons

1. First things first, download the `CACApi.jar` of the newest [**release**](https://github.com/Clientastisch/Cardinal-Anticheat/releases)
2. Add `CACApi.jar` as you dependency. It's **only** a placeholder, nothing you should move inside your `plugins` folder
3. Instead of `extends JavaPlugin` you have to `implement Addon` which requires two methods:

```java
import me.clientastisch.extension.Extension;
import me.clientastisch.extension.impl.Addon;
import net.clientastisch.events.FlagEvent;

public class Core implements Addon {

    @Override
    public void onEnable() throws Exception {
    
    }

    @Override
    public void onDisable() throws Exception {

    }
}
```

4. Unlike spigot, a file called `addon.json` must be created like following:

```json
{
  "name": "MyAwesomeAddon",
  "author": "Me",
  "main": "my.path.to.core",
  "version": "v1.0"
}
```

5. Export your addon to `plugins//CAC//addons`
6. Reload your server or use `/cac addon load <addon>` and you're done!

##Bugs

###How to handle bugs
