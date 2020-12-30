# Cardinal-Anticheat 1.8-1.12

<img
 src="http://cac.dodo1213.de/img/banner.png"
/>

<div
 align="center">
    <a
     href="https://go.lukasl.dev/cacdiscord">
        <img
            height="30" src="https://img.shields.io/discord/647922123192533022.svg?logo=discord&style=for-the-badge"
        />
    </a>
</div>

## Disclaimer

Cardinal-Anticheat is a **free** [**Spigot**](https://github.com/SpigotMC) anticheat which blocks most of the known cheats out there. Keep in mind, that Cardinal-Anticheat is still in beta, false postives may occurre...

Cardinal-Anticheat also contains a custom build-in replay system which is quite usable to check whether a player was cheating or not. The output-file is a .zip file ~ 5MB depending on the amount of worlds used and their size.

[**Download**](#terms-of-use)

## Commands

```text
cac flag    - Shows the flags/alerts
cac ban     - Bans a player permanently
cac unban   - Unbans a player
cac info    - Tells you whether a player is banned or not
cac iptable - Adds the ip-address of a player to the firewall rule and prevents any further communication
cac replay  - Watch a replay which has been recorded before
cac report  - A custom report system only for stuffs in which each flag will be a 'report' which will be stored
cac reset   - Resets the violations of a player
cac reboot  - Restarts the plugin
cac reload  - Reloads configurations
cac export  - Export the current settings into a single file
cac import  - Import a setting from a file
```

## Permission

```text
CAC.command       - Allows you to use most of the commands
CAC.tabcomplete   - Allows you to use tab-completion
CAC.flag          - Allows you to toggle /cac flag
CAC.manage.ban    - Allows you to ban players
CAC.manage.unban  - Allows you to unban players
CAC.manage.report - Allows you to edit reports
CAC.addon         - Allows you to manage addons
CAC.proxy         - Allows you to join even though your ip might be a proxy
CAC.config.import - Allows you to import settings
CAC.config.export - Allows you to export settings
CAC.replay.watch  - Allows you to watch replays
CAC.replay.gui    - Allows you to see a list of all replays ingame
```

## Important

If you're using multiversion to allow players of any version to join false positives will occurre...
In case your server is on 1.8 and players with versions higher than that are able to you disable at least following detections:

+ yMotion
+ Speed Type A

# Installation

First navigate to the [**release**](https://github.com/Clientastisch/Cardinal-Anticheat/releases) tab and download the newest version available. After the download move the `Cardinal.jar` into the `plugins` folder. Reload your server and you're ready to go :)

In case you wan't to use the build in ban and report system, you need to download a database [dialect](https://github.com/Clientastisch/Cardinal-Anticheat/blob/master/DIALECT.md) either from [github](https://github.com/Clientastisch/Cardinal-Anticheat/tree/master/dialects) or [discord](https://go.lukasl.dev/cacdiscord). Move the addon into your `plugins//CAC//addons` folder, it'll be recognized, loaded and used by Cardinal and all database connections are handled by the addon, which provides better security.

<hr >

### Bugs & False positives

If any bugs or false positives occurre **report** them [**here**](https://github.com/Clientastisch/Cardinal-Anticheat/issues/new/choose). <br>
Otherwise I'll probably never notice them
