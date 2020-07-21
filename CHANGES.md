# Cardinal-Anticheat Changes

<img
 src="http://cac.dodo1213.de/img/banner.png"
/>

<div
 align="center">
    <a
     href="https://link.lukasl.dev/cacdiscord">
        <img
            height="30" src="https://img.shields.io/discord/647922123192533022.svg?logo=discord&style=for-the-badge"
        />
    </a>
</div>

## 0.9995

```text
Removed Check
    - DeathInteract Type A
    - BlockDestroy

Added Check
    - AimAssist Type E
    - Scaffold Type E
    - Speed Type N

Fixed false positives
    - FastLadder Type A
    - ChestAura
    - PreAura

    1.8 - 1.12:
        - Speed Type B
        - Blink Type C

Fixed other
    - Addon unloading
    - Fly Type E

Changed default config:
    - Phase
        - banType: kick -> none
```

## 0.9994

```text
Debug log will now be stored in the cloud in case a player gets banned.
This has the big advantage, that I'll understand more false positives.
```

## 0.9993

```text
Removed checks
    - SporadicAiming

Added checks
    - AimAssist Type C
    - AimAssist Type D
    - ChestAura
    - PingSpoof

Changed default config:
    - disabled AimAssist Type A
    - disabled Blink Type A
    - disabled Blink Type B

Important:
    In case you already used Cardinal before version 0.9991,
    please delete the config files for AimAssist Type C and D
```

## 0.9992

```text
Cardinal-Anticheat loader

Updates don't have to be downloaded manually anymore.
You will always be up-to-date
```

## 0.9991

```text
Removed checks
    - NetFrequence Type C
    - AimAssist Type C
    - AimAssist Type D

Added checks
    - NetFrequence Type C
    - Blink Type C

Fixed false positives
    - Speed Type M
    - Spider

Recoded Command-system
    - Improved tab-copletion
    - New command 'cac report'
```