# worlds.yml
worlds.yml is a file that contains information on how you'd like the plugin to load, and affect specific worlds. All attributes are case sensitive.

## **Contents**
* [Attributes](https://github.com/Z4OLLIEZ4/Space/wiki/World-Configuration#Attributes)
* [Example Configuration File](https://github.com/Z4OLLIEZ4/Space/wiki/World-Configuration#Example-Configuration-File)

## **Attributes**
There are a few attributes that space requires in order to load a world successfully.

### **<u>oxygen</u>**
* This attribute determines whether a world will be freely breathable or require protective gear
* This can only accept the arguments `true` or `false`

_Example:_
```yaml
oxygen: false
```

### **<u>microgravity</u>**
* This attribute determines whether a planet will have slow-falling or not
* This can only accept the arguments `true` or `false`

_Example:_
```yaml
microgravity: true
```

### **<u>microgravity-level</u>**
* This attribute determines how quickly players will fall in microgravity enabled worlds
* This is not used if `microgravity: false`
* This can accept integers between 1-15. Higher numbers will mean slower falling.

_Example:_
```yaml
microgravity-level: 1
```

### **<u>mob-microgravity</u>**
* This attribute determines whether mobs in the world will be affected by microgravity or not
* This is independent to the `microgravity` option
* This can only accept the arguments `true` or `false`

_Example:_
```yaml
mob-microgravity: true
```

### **<u>item-microgravity</u>**
* This attribute determines whether items in the world will be affected by microgravity or not
* This is independent to the `microgravity` option
* This can only accept the arguments `true` or `false`

_Example:_
```yaml
item-microgravity: true
```

### **<u>display-name</u>**
* This attribute determines the display name of the world in the rocket
* This can accept any string argument

_Example:_
```yaml
display-name: "Space"
```

### **<u>enhanced-creepers</u>**
* This attribute determines whether the world will use [enhanced creepers](enhanced-creeper)
* This can only accept the arguments `true` or `false`

_Example:_
```yaml
enhanced-creepers: true
```

### **<u>radioactive</u>**
* This attribute determines whether the world will be radioactive
* This can only accept the arguments `true` or `false`

_Example:_
```yaml
radioactive: true
```

### **<u>dead-astronauts</u>**
* This attribute determines whether the world will use [dead astronauts](Dead-Astronaut)
* This can only accept the arguments `true` or `false`

_Example:_
```yaml
dead-astronauts: true
```

### **<u>custom-ores</u>**
* This attribute determines whether the world will use custom ores
* This can only accept the arguments `true` or `false`

_Example:_
```yaml
custom-ores: true
```

### **<u>prevent-crops</u>**
* This attribute determines whether the world will prevent crop growth
* This only matters if `oxygen: false`
* This can be quite resource intensive
* This can only accept the arguments `true` or `false`

_Example:_
```yaml
prevent-crops: true
```

### **<u>deny-flight</u>**
* This attribute determines whether player flight should be disabled in the world
* This will also render the jetpack module unusable
* This can only accept the arguments `true` or `false`

_Example:_
```yaml
deny-flight: true
```

### **<u>skull</u>**
* This attribute determines the skull texture that should be shown for the world within the rocket GUI
* This can only accept string arguments

_Example:_
```yaml
skull: "eyJ0ZXh0dXJlcyI6eyJTS0lOIjp7InVybCI6Imh0dHA6Ly90ZXh0dXJlcy5taW5lY3JhZnQubmV0L3RleHR1cmUvMjdhZDk2Y2IyYTRiMTRkMDE2MWYyODc5OTRkM2RiMTg3YWZkODcxNjRmMzk4N2I4N2U3ZjExOGQxZjU4NzkifX19"
```

### **<u>skull-lore</u>**
* This attribute determines the lore of the skull displayed in the rocket GUI
* This can only accept string arguments

_Example:_
```yaml
skull-lore: "&7An extraterrestrial planet devoid of life"
```

### **<u>prevent-passive</u>**
* This attribute determines whether the world will prevent passive mobs spawning
* This can only accept the arguments `true` or `false`

_Example:_
```yaml
prevent-passive: true
```

### **<u>use-jumpboost</u>**
* This attribute determines whether the world will allow the player to jump higher
* This can only accept the arguments `true` or `false`

_Example:_
```yaml
use-jumpboost: true
```

### **<u>jumpboost-level</u>**
* This attribute determines how high the player can jump
* This attribute is only relevant if `use-jumpboost: true`
* This can only accept integer values

_Example:_
```yaml
jumpboost-level: 1
```

### **<u>zero-gravity</u>**
* This attribute determines whether the world will have no gravity at all (Absolute floating, as in Orbit)
* This can only accept the arguments `true` or `false`

_Example:_
```yaml
zero-gravity: true
```

### **<u>display-in-rocket</u>**
* This attribute determines whether the world will be shown in the rocket GUI for players to teleport to
* This can only accept the arguments `true` or `false`

_Example:_
```yaml
display-in-rocket: true
```

### **<u>cost</u>**
* This attribute determines how much it costs in economy to teleport to the planet using a rocket
* If set to 0, this option will not matter
* This can only accept integer arguments

_Example:_
```yaml
cost: 0
```

### **<u>safe-void</u>**
* This attribute, if `true`, will make it impossible for the player to die due to void damage
* This can only accept the arguments `true` or `false`

_Example:_
```yaml
safe-void: true
```

### **<u>acid-rain</u>**
* This attribute determines whether the world will have acid rain or not
* This can only accept the arguments `true` or `false`

_Example:_
```yaml
acid-rain: false
```

### **<u>temperature</u>**
* This attribute determines the temperature of the world
* A cold world requires the argument `-1`
* A normal world requires the argument `0`. This will disable temperature for that world.
* A hot world requires the argument `1`
* This can only accept the arguments `-1`, `0`, `1`

_Example:_
```yaml
temperature: 0
```

### **<u>respawn-world</u>**
* This attribute determines the world the player will respawn in, provided they die in this world
* The world provided must exist
* If the same world is input as the world you are currently adding, this will have no effect 
* This can only accept string arguments

_Example:_
```yaml
respawn-world: Space
```

### **<u>permission</u>**
* The permission required to teleport to this world
* This can only accept string arguments

_Example:_
```yaml
permission: space.test
```

### **<u>rocket-mode</u>**
* The mode which rockets should operate under. Rocket mode 0 indicates world-to-world transfers should be used, where as rocket mode 1 indicated world-to-server transfers should be used. This is only necessary if you are using bungee and would like to send the player to another server, otherwise you should be using `rocket-mode: 0`
* This can only accept integer arguments 0 and 1

_Example:_
```yaml
rocket-mode: 0
```

### **<u>Example Configuration File</u>**
```yaml
Worlds:
  Space:
    oxygen: false
    microgravity: true
    microgravity-level: 1
    mob-microgravity: true
    item-microgravity: true
    display-name: "Space"
    enhanced-creepers: true
    radioactive: false
    dead-astronauts: true 
    custom-ores: true
    prevent-crops: false
    deny-flight: true
    skull: "eyJ0ZXh0dXJlcyI6eyJTS0lOIjp7InVybCI6Imh0dHA6Ly90ZXh0dXJlcy5taW5lY3JhZnQubmV0L3RleHR1cmUvMjdhZDk2Y2IyYTRiMTRkMDE2MWYyODc5OTRkM2RiMTg3YWZkODcxNjRmMzk4N2I4N2U3ZjExOGQxZjU4NzkifX19"
    skull-lore: "&7An extraterrestrial planet devoid of life"
    prevent-passive: true
    use-jumpboost: true
    jumpboost-level: 1
    zero-gravity: false
    display-in-rocket: true
    cost: 0
    safe-void: true
    acid-rain: false
    temperature: 0 # -1 = cold, 0 = normal, 1 = hot
    respawn-world: Space # The world the player will spawn in if they die in this world
    rocket-mode: 0 # 0 for world to world transportation, 1 for server to server transportation (bungee only)
  Orbit:
    oxygen: false
    # This does not matter on the orbit world
    microgravity: true
    microgravity-level: 1
    mob-microgravity: true
    item-microgravity: true
    display-name: "Orbit"
    enhanced-creepers: false
    radioactive: false
    custom-ores: false
    prevent-crops: false
    dead-astronauts: false
    zero-gravity: true
    deny-flight: true
    skull: "eyJ0ZXh0dXJlcyI6eyJTS0lOIjp7InVybCI6Imh0dHA6Ly90ZXh0dXJlcy5taW5lY3JhZnQubmV0L3RleHR1cmUvM2U4YWFkNjczMTU3YzkyMzE3YTg4YjFmODZmNTI3MWYxY2Q3Mzk3ZDdmYzhlYzMyODFmNzMzZjc1MTYzNCJ9fX0="
    skull-lore: "&7Create or teleport to your space station"
    prevent-passive: true
    display-in-rocket: true
    use-jumpboost: false
    jumpboost-level: 0
    safe-void: true
    acid-rain: false
    temperature: 0 # -1 = cold, 0 = normal, 1 = hot
    respawn-world: world # The world the player will spawn in if they die in this world
    rocket-mode: 0 # 0 for world to world transportation, 1 for server to server transportation (bungee only)
  world:
    oxygen: true
    microgravity: false
    microgravity-level: 0
    mob-microgravity: false
    item-microgravity: false
    display-name: "Earth"
    enhanced-creepers: false
    radioactive: false
    display-in-rocket: true
    zero-gravity: false
    custom-ores: true
    prevent-crops: false
    deny-flight: false
    skull: "eyJ0ZXh0dXJlcyI6eyJTS0lOIjp7InVybCI6Imh0dHA6Ly90ZXh0dXJlcy5taW5lY3JhZnQubmV0L3RleHR1cmUvMmUyY2M0MjAxNWU2Njc4ZjhmZDQ5Y2NjMDFmYmY3ODdmMWJhMmMzMmJjZjU1OWEwMTUzMzJmYzVkYjUwIn19fQ"
    skull-lore: "&7Return to your home planet"
    prevent-passive: false
    use-jumpboost: false
    jumpboost-level: 0
    dead-astronauts: false
    cost: 1000
    safe-void: true
    acid-rain: false
    temperature: 0 # -1 = cold, 0 = normal, 1 = hot
    respawn-world: world # The world the player will spawn in if they die in this world
    rocket-mode: 0 # 0 for world to world transportation, 1 for server to server transportation (bungee only)
```