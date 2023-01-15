Space hooks into [PlaceholderAPI](https://www.spigotmc.org/resources/placeholderapi.6245/) automagically and registers these placeholders for use by other plugins. 

| Placeholder | Description |
| --- | --- |
| `%space_oxygen%` | Returns the current amount of oxygen in the player's in-use Oxygen Tank. Will return "Infinite" if the player is in an oxygenated world. |
| `%space_oxygen_max%` | Returns the oxygen capacity of the player's in-use Oxygen Tank. Will return "Infinite" if the player is in an oxygenated world. |
| `%space_planet%` | Returns the display name of the Space planet the player is in. Will return `null` if the player is in a non-Space world. |
| `%gravity_level%` | Returns the gravity level of the Space planet the player is in. Will return `null` if the player is in a non-Space world. |
| `%gravity_status%` | Returns the gravity status of the Space planet the player is in. Will return `null` if the player is in a non-Space world. |