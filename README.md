# Cardinal-Anticheat 1.8-1.12

<div align="center">
    <img src="images/banner.png" />
</div>

<br />

<div align="center">
    <img
        src="https://img.shields.io/badge/Written%20in-java-%23EF4041?style=for-the-badge"
        height="30"
    />
    <a href="https://go.lukasl.dev/cacdiscord">
        <img 
            src="https://img.shields.io/discord/647922123192533022?color=212121&label=Discord&logo=discord&logoColor=212121&style=for-the-badge"
            height="30"
        />
    </a>
    <a href="https://micartey.github.io/Cardinal-Anticheat/documentation" target="_blank">
        <img
            src="https://img.shields.io/badge/javadoc-reference-5272B4.svg?style=for-the-badge"
            height="30"
        />
    </a>
</div>

<br />

<p align="center">
  <a href="#-introduction">Introduction</a> |
  <a href="#-testserver">Testserver</a> |
  <a href="#-terms-of-use">Getting started</a> |
  <a href="https://github.com/Clientastisch/Cardinal-Anticheat/issues">Troubleshooting</a>
</p>


## 📚 Introduction

Cardinal-Anticheat is a free spigot anticheat which blocks most of the known cheats out there. Keep in mind, that Cardinal-Anticheat is still in beta, false postives may occurre...

![img](images/ezgif.com-gif-maker.gif)

Cardinal-Anticheat also contains a custom build-in replay system which is quite usable to check whether a player was cheating or not. The output-file is a .zip file ~ 5MB depending on the amount of worlds used and their size.

## 👾 Testserver

If you are interested but don't want to setup a test server to try out the anticheat, you are welcome to join the official public testserver. The server, however, runs minecraft 1.8

```
cardinal.micartey.dev
```

## 📄 Terms of Use

**IMPORTANT NOTICE:** By downloading and using Cardinal-Anticheat you accept the following terms of use:

- I allow the plugin to download source code from another computer
- I understand that decomiling any related source code is strictly prohibited
- I understand that reengineering any part of Cardinal is strictly prohibited

If you have any questions about the backgrounds, please contact my discord

## 📝 Getting Started

Cardinal Anticheat is a great system with a lot of functionality. First navigate to the [**release**](https://github.com/Clientastisch/Cardinal-Anticheat/releases) tab and download the newest version available. After the download move the jar file into the plugins folder. Reload your server and you're ready to go.

### Commands

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

### Permission

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

### Custom ban manager

By default Cardinal Anticheat doesn't handle a database connection. The reason is farily easy to understand. Cardinal Anticheat is a close source plugin whose source is never on the server physically. This has legitimate security and privacy concerns. 

That's why you can tell cardinal anticheat in the `Config.yml` which commands should be executed in case of a ban etc.

### Built-in ban system

As already stated does Cardinal Anticheat not handle any database connections by default, however using the build-in ban system requires you to use a so called dialect which you have to write yourself. The documentation for writing a dialect is available [here](DIALECT.md).

Due to inquiries I have already written a dialect for the mongo and mysql driver. You can download them [here](dialects/)

### Report system

Maybe you don't want a player to be banned right away or lower the chance of banning a legit player. For this reason it makes sense to use Cardinal's report system. Each flag is saved in the database using a [dialect](DIALECT.md) and based on the number and type of flags, a moderator can decide for himself when a player should be banned. For example you only ban the 10% of players with the most falgs each month etc. Maybe you want to introduce some form of trust factor and scale damage and recoil as a result. You might want to let players with similar trust factors play against each other. If you are a developer and want to get to implement such a system, the possibilities are limitless.

### Addons

Cardinal also allows loading, developing and sharing addons. There are already some addons on my [discord](https://go.lukasl.dev/cacdiscord) server. Furthermore, there is a rather good documentation for developsers on how to write your own addons [here](ADDON.md).