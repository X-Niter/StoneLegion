## Changelog for keeping up to date with changes of the server, preferably large changes.

## [1.0.0] - 2021-09-02 - First Update Notation

### Large Optimization tuning
Will tune this up and down as time moves forward for sure!

- **Replaced FAWE with Worldedit.

- **chunk-gc.period-in-ticks**:***Decreased-to***: *400*

- **ticks-per.monster-spawns**:***Increased-to***: *4*

- **spawn-limits.monsters**:***Decreased-to***: *25*

- **spawn-limits.water-ambient**:***Decreased-to***: *5*

- **spawn-limits.ambient**:***Decreased-to***: *1*

- **spawn-limits.animals**:***Decreased-to***: *5*

- **entity-activation-range.animals**:***Decreased-to***: *16*

- **entity-activation-range.monsters**:***Decreased-to***: *16*

- **entity-activation-range.misc**:***Decreased-to***: *12*

- **entity-activation-range.water**:***Decreased-to***: *12*

- **entity-activation-range.villagers**:***Decreased-to***: *16*

- **entity-activation-range.tick-inactive-villagers**:***Changed-to***: *Disabled*

- ****entity-activation-range.wake-up-inactive.villagers-for****:***Decreased-to***: *20*

- ****entity-activation-range.wake-up-inactive.flying-monsters-for****:***Decreased-to***: *60*

- **entity-activation-range.wake-up-inactive.villagers-max-per-tick**:***Decreased-to***: *1*

- **entity-activation-range.wake-up-inactive.animals-for**:***Decreased-to***: *40*

- **entity-activation-range.wake-up-inactive.monsters-max-per-tick**:***Decreased-to***: *4*

- **entity-activation-range.wake-up-inactive.flying-monsters-max-per-tick**:***Decreased-to***: *1*

- **entity-activation-range.wake-up-inactive.animals-max-per-tick**:***Decreased-to***: *2*

- **entity-activation-range.wake-up-inactive.monsters-for**:***Decreased-to***: *60*

- **Aikar's Flags**:***Changed-to***: *Using Flags listed below*
```
java -Xms{RamMinimum}M -Xmx{RamMaximum}M -XX:+UseG1GC -XX:+ParallelRefProcEnabled -XX:MaxGCPauseMillis=200 -XX:+UnlockExperimentalVMOptions -XX:+DisableExplicitGC -XX:+AlwaysPreTouch -XX:G1NewSizePercent=30 -XX:G1MaxNewSizePercent=40 -XX:G1HeapRegionSize=8M -XX:G1ReservePercent=20 -XX:G1HeapWastePercent=5 -XX:G1MixedGCCountTarget=4 -XX:InitiatingHeapOccupancyPercent=15 -XX:G1MixedGCLiveThresholdPercent=90 -XX:G1RSetUpdatingPauseTimePercent=5 -XX:SurvivorRatio=32 -XX:+PerfDisableSharedMem -XX:MaxTenuringThreshold=1 -Dusing.aikars.flags=https://mcflags.emc.gs -Daikars.new.flags=true -jar server.jar nogui
```

- **arrow-despawn-rate**:***Decreased-to***: *300*

- **merge-radius.item**:***Increased-to***: *4.0*

- **merge-radius.exp**:***Increased-to***: *6.0*

- **max-entity-collisions**:***Decreased-to***: *2*

- **max-auto-save-chunks-per-tick**:***Decreased-to***: *6*

- **optimize-explosions**:***Changed-to***: *Enabled*

- **mob-spawner-tick-rate**:***Increased-to***: *2*

- **game-mechanics.disable-chest-cat-detection**:***Changed-to***: *Enabled*

- **despawn-ranges.soft**:***Decreased-to***: *28*

- **despawn-ranges.hard**:***Decreased-to***: *98*

- **hopper.disable-move-event**:***Changed-to***: *Enabled*

- **non-player-arrow-despawn-rate**:***SetValue-to***: *0 -> 60*

- **creative-arrow-despawn-rate**:***SetValue-to***: *0 -> 60*

- **prevent-moving-into-unloaded-chunks**:***Changed-to***: *Enabled*

- **use-faster-eigencraft-redstone**:***Changed-to***: *Enabled*

- **armor-stands-do-collision-entity-lookups**:***Changed-to***: *Disabled*

- **per-player-mob-spawns**:***Changed-to***: *Enabled*

- **alt-item-despawn-rate.enabled**:***Changed-to***: *Enabled*

- **no-tick-view-distance**:***SetValue-to***: *0/-1 -> 60*

- **view-distance**:***Decreased-to***: *5*

- **maxEntityCramming**:***Decreased-to***: *8*

- **max-auto-save-chunks-per-tick**:***Decreased-to***: *6*

- **mob-spawn-range**:***Decreased-to***: *3*

### Notes

I do expect that the Entities changes will for sure go up based on game play, for now this is a solid API based change that I made, meaning the online tool took my timing reports and gave me feedback, I went it did all of the suggested feedback and went back with a new timing report every time until it said that my changes were at it's best optimum configuration, but again, I'll for sure be changing the mob/entity configurations as time goes on. Already with making all these changes I've noticed a pretty solid preformance difference which is always a plus!
