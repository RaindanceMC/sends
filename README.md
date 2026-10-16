# RaindanceMC/sends

- **`sends-module`** — Rain's Flexible Modules — Sends: Send items to another player: put them in a window, press send, and they accept with a click or /send accept. Sends wait ten minutes (configurable) and survive restarts; whoever has no room can take them later from /sends, and anything not accepted goes back.
- **`sends-standalone`** — Rain's Sends: Rain's Sends, as a plugin of its own. Nothing here but a build file and a descriptor: the sends module and the standard wrapper are shaded together, and that is the whole plugin.

Part of [RaindanceMC](https://github.com/RaindanceMC); built on [RainsCore](https://github.com/RaindanceMC/RainsCore) and the shared parent in [framework](https://github.com/RaindanceMC/framework). Split out of `rains-flexible-modules` on 16.10.2026, history kept.

## Build

```
mvn install
```

Needs Java 25 and read access to `packages.tstieh.de` (server ids `packages-releases` / `packages-snapshots` in `~/.m2/settings.xml`).

## Plugins

- `sends-standalone/target/RainsSends-0.3.0.jar` — also published as `de.raindancer.modules:sends-standalone:0.3.0`

## Versions

A module's version is a property in this repository's root `pom.xml`, a plugin's is `plugin.version` in its own pom. CI publishes every version that is not in the registry yet on the next push to master.
