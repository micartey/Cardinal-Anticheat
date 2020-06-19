# Cardinal-Anticheat

<div align="center">
    <a href="https://link.lukasl.dev/discord">
        <img
            height="30" src="https://img.shields.io/discord/432617716961116180.svg?logo=discord&style=for-the-badge"
        />
    </a>
</div>

## Disclaimer

## Installation

First navigate to the [**release**](https://github.com/Clientastisch/Cardinal-Anticheat/releases) tab and download the newest version available.

## Addons

1. First things first, download the `CACApi.jar` of the newest [**release**](https://github.com/Clientastisch/Cardinal-Anticheat/releases)
2. Add `CACApi.jar` as you dependency. It's **only** a placeholder, nothing you should do inside your `plugins` folder
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

5. Export you addon to `plugins//CAC//addons`
6. Reload your server or use `/cac addon load <addon>` and you're done!
