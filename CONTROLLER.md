# Cardinal-Anticheat Database

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

## PlayerController

```java
    /**
     * PvPLounge is a modification to have advantages in pvp due
     * being verified for playing legit. However I do not consider
     * this as legit, but it is your server so I don't mind
     *
     * @return whether a players uses PvPLounge or not
     */
    public abstract boolean isUsingPvpLounge();

    /**
     * If a player is whitelisted, he wouldn't be detected anymore.
     *
     * @return true if a player is whitelisted
     */
    public abstract boolean isWhitelisted();

    /**
     * If a player is whitelisted, he wouldn't be detected anymore.
     *
     * @param whitelisted The state of the player whitelist
     * @see PlayerController#isWhitelisted()
     */
    public abstract void setWhitelisted(boolean whitelisted);

    /**
     * If a player is whitelisted, he wouldn't be detected anymore.
     *
     * @param whitelisted The state of the player whitelist
     * @param time Time amount of seconds a player keeps the new state
     * @see PlayerController#isWhitelisted()
     */
    public abstract void setWhitelisted(boolean whitelisted, long time);


    /**
     * If a player is verified he wouldn't be detected by the most
     * detections.
     *
     * @return The verified state
     */
    public abstract boolean isVerified();

    /**
     * Set a players verify state. He wouldn't be detected by the most
     * detections.
     *
     * @param verified whether the player should be verified or not
     * @see PlayerController#isVerified()
     */
    public abstract void setVerified(boolean verified, Verify state);

    /**
     * Returns whether a player is showing alerts or not.
     * He can see every violation caused by a player.
     *
     * @return Showing flags
     */
    public abstract void isShowingFlags();

    /**
     * Show/Hide alerts caused by players.
     *
     * @param state whether the player can see flags or not
     * @see PlayerController#isShowingFlags()
     */
    public abstract void setShowingFlags(boolean state);

    /**
     * Returns the modification identifier,
     * for instance Vanilla
     *
     * @return Modification identifier
     */
    public abstract String getVersion();

    /**
     * Returns the current trustfactor of a player.
     * Values less than 1 are below the average and should be
     * threaten very carefully. Normally the trustfactor is 1.
     *
     * @return TrustFactor
     */
    public abstract Double getTrustFactor();

    /**
     * Returns the average ping of the last {@param size}
     * packets
     *
     * @param size of the ping packets
     * @return Average ping of the last {@param size} packets
     */
    public abstract long getAveragePing(int size);
```
