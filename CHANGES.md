# Cardinal-Anticheat Changes

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

## 1.0002

```text
Added checks
    - AntiBot Type A
    - KillAura Type C
    - Velocity Type B

Other:
    • Fixed 'cannot interact with itself' issue
```

## 1.0001

```text
Added checks
    - KillAura Type B
    - AimAssist Type G

Other:
    • Removed database, therefore added a dialect layer
      so no fixed database is required and thus exchangeable
```

## 0.9999

```text
Improved checks
    - KillAura Type A
    - AimAssist Type F

Removed checks
    - AntiTeams

Fixed exceptions
    - KeepAlive Timeout for 1.12

Fixed disabling issue
```

## 0.9998

```text
Added checks
    - Range Type F

Improved checks
    - KillAura Type A

Added description for some checks
```

## 0.9997

```text
Fixed false positives for high ping
    - KillAura Type A
    - Range Type D
    - Range Type E

Changed default config
    - Range Type B
        - toggle: true -> false
    - Range Type C
        - toggle: true -> false
```

## 0.9996

```text
Removed check
    - AimAssist Type E
    - Velocity Type B
    - Velocity Type C

Added checks
    - Scaffold Type F
    - Scaffold Type G

Recoded checks
    - Range Type A
        slightly more accurate than Type B and C

Fixed false positives
    - PacketAnalysis Type F
    - Blink Type C
    - PingSpoof

Fixes:
    - Force disabled checks won't be saved as disabled anymore
    - Flag bug

Other:
    Added command: 'cac graph'
    Displays performance per tick in a graph
```

## 0.9995

```text
Removed checks
    - DeathInteract Type A
    - BlockDestroy

Added checks
    - PacketAnalysis Type F
    - AimAssist Type E
    - Scaffold Type E
    - Speed Type N

Fixed false positives
    - FastLadder Type A
    - AimAssist Type C
    - ChestAura
    - PreAura

    1.9 - 1.12:
        - Speed Type B
        - Blink Type C

Fixed other
    - Addon unloading
    - Fly Type E

Changed default config:
    - Phase
        - banType: kick -> none

Replay System:
    - Added BlockListener to detect block changes
    - Fixed world loading issue

Important:
    Config changes will interfere with the documentation
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