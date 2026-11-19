<div align="center">

# 💎 Gen-Splitter

**Share generator drops between teammates in [MBedwars](https://www.spigotmc.org/resources/mbedwars.13940/).**

![Java 8+](https://img.shields.io/badge/Java-8%2B-orange?logo=openjdk&logoColor=white)
![MBedwars](https://img.shields.io/badge/requires-MBedwars%205.5.9%2B-dc2626)
![License](https://img.shields.io/badge/license-GPL--3.0-blue)

> BlockStorm's fork of [MetallicGoat/Gen-Splitting](https://github.com/MetallicGoat/Gen-Splitting).

</div>

---

## ✨ Features

| | Feature | |
|---|---|---|
| ✂️ | **Gen splitting** | When a player picks up items from a generator, teammates standing nearby get the same items |
| 🧲 | **Auto collect** | When a player is killed, the killer gets a message listing the resources they collected, and the amount can be cut to a percentage (the items themselves are handed over by MBedwars' own killer auto-pickup) |
| 🕳️ | **Anti void drops** | Stops players from dropping items while they are above the void |
| 🆙 | **LevelShop support** | Also splits experience levels when the MBedwars LevelShop addon is installed |

## ⚙️ Configuration

The add-on's `config.yml` is in its folder inside MBedwars' add-ons directory:

| Option | Default | |
|---|---|---|
| `Gen-Splitter` | `true` | Turn splitting on or off |
| `Split-Spawners` | iron, gold | Which spawner materials are split |
| `Split-Radius` | `2.5` | How close teammates must be, in blocks |
| `Split-LevelShop-Addon` | `true` | Split experience levels from the LevelShop addon |
| `Anti-Void-Drops` | `false` | Block dropping items into the void |
| `Auto-Collect.Enabled` | `true` | Turn auto collect on or off |
| `Auto-Collect.Percentage-Kept` | `100` | Percentage of the victim's resources the killer receives |
| `Auto-Collect.Message-Materials` | iron, gold, diamond, emerald | Which resources are listed in the killer's message |
| `Auto-Collect.Message` | `{item} &f+{amount}` | Message shown to the killer for each resource |

## 📦 Requirements

| Plugin | |
|---|---|
| MBedwars 5.5.9 or newer | **Required** |
| MBedwars LevelShop | Optional |

## 🛠️ Building

```bash
mvn clean package
```

The jar is written to `target/Gen-Splitter-4.4.2.jar`.

## 📖 Documentation

The full guide is in the [wiki](https://github.com/BlockStormHU/mc-gen-splitting-fork/wiki):

- [Installation](https://github.com/BlockStormHU/mc-gen-splitting-fork/wiki/Installation): requirements, building the jar
  and installing it
- [Features](https://github.com/BlockStormHU/mc-gen-splitting-fork/wiki/Features): how splitting, auto collect and anti void
  drops work
- [Configuration](https://github.com/BlockStormHU/mc-gen-splitting-fork/wiki/Configuration): every option in `config.yml`
- [Original README](https://github.com/BlockStormHU/mc-gen-splitting-fork/wiki/Original-README): about the upstream project

## 📄 License

Gen-Splitter is licensed under the [GNU GPL v3](LICENCE.md), inherited from the original project by MetallicGoat.
Changes in this fork are released under the same license.
