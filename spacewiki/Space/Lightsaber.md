![Image unavailable](https://i.imgur.com/cSW7QfV.png)

A Lightsaber is a retractable weapon that can be modified in a [Quantum Workbench](Quantum-Workbench).

# Obtaining

## Crafting

Lightsabers can be crafted using the following items:

* 1x Diamond Sword
* 1x [Energized Wire](Energized-Wire)
* 1x [Reinforced Aluminium Alloy Ingot](Reinforced-Aluminium-Alloy-Ingot)
* 2x Diamond
* 4x [Aluminium Alloy Ingot](Aluminium-Alloy-Ingot)

![Image unavailable](https://i.imgur.com/cdhTCQo.png)

# Usage

## Attributes

A default Lightsaber has 20.0 attack damage.

## Toggling

Holding use (right-click) whilst holding a Lightsaber will toggle whether it is active or inactive after two seconds.

## Modifying

Putting a Lightsaber in a [Quantum Workbench](Quantum-Workbench) will allow modifying the Lightsaber's model, attack damage, attack speed, durability, and enchantments. The modifications are done by selecting another Lightsaber from the displayed options.

# Adding Lightsabers

To add Lightsabers, copy the default format that is stored within `config.yml`:

```yaml
Lightsabers:
  Default:
    cost: 10000 # The cost to buy the Lightsaber in the Quantum Workbench
    charged: false # Should the lightsaber need to be charged to be used
    max-charge: 800 # What should the max charge be? (Only relevant if charged: true)
    active: # The active variant of the Lightsaber we are making
      name: '&cLightsaber'
      type: STONE_SWORD
      modeldata: 1234568
      activate-sound: lightsaber_on
      enchanted: true
      damage: 20
      attackspeed: 2
      lore:
        1: '&7A powerful plasma blade'
        2: '&7Right click to toggle states'
        3: '&aActive'
      enchantments:
      - 'FIRE_ASPECT:2'
    inactive: # The inactive variant of the Lightsaber we are making
      name: '&cLightsaber'
      type: STONE_SWORD
      modeldata: 1234567
      deactivate-sound: lightsaber_off
      enchanted: false
      damage: 0
      attackspeed: 0
      lore:
        1: '&7A powerful plasma blade'
        2: '&7Right click to toggle states'
        3: '&cInactive'
```

A few notes:

* One must define an active and inactive variant for any Lightsaber you create. This is so the blade can properly retract.
* The valid enchantments are listed [here](https://hub.spigotmc.org/javadocs/bukkit/org/bukkit/enchantments/Enchantment.html) and must be in the format shown above.
* One can currently define up to 15 Lightsabers.
* One can define up to 4 lines of lore.