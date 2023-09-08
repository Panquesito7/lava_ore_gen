# Lava Ore Generation

> **Note**
> This mod was originally owned by Coder12 which is no longer available on GitHub.\
> The mod might be outdated and not work in the latest MT versions. I'll be updating the mod soon.

This mod makes the lava turn stone into ore over time.    
When lava comes in contact with stone it turns red hot. After a specific time it turns into ore.

## Installation

- Unzip the archive, rename the folder to `lava_ore_gen` and
place it in .. minetest/mods/

- GNU/Linux: If you use a system-wide installation place
    it in ~/.minetest/mods/.

- If you only want this to be used in a single world, place
    the folder in .. worldmods/ in your world directory.

For further information or help, see:   
https://wiki.minetest.net/Installing_Mods


# API

`lava_ore_gen.blacklist` is a table where you can blacklist node names by listing them in the table.   
Example code:

```lua
lava_ore_gen.blacklist["default:stone_with_iron"] = true
```

# Settings

The stone node name to override.

```lua
lava_ore_gen.stone_name = "default:stone"
```

Fixed interval of when to change stone to ore.

```lua
lava_ore_gen.interval = 3600
```

Random chance of when to change stone to ore.

```lua
lava_ore_gen.chance = 86400
```

Make ores random instead of being based on how rare they are.

```lua
lava_ore_gen.random = false
```
