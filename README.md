- id: tiger

  # The display name of the pet
  name: "&6Tiger"

  # The description of the pet
  description: "&8&oLevel up by dealing melee damage"

  # The xp requirements for each pet level - add new levels by adding more to this list
  level-xp-requirements:
    - 50
    - 125
    - 200
    - 300
    - 500
    - 750
    - 1000
    - 1500
    - 2000
    - 3500
    - 5000
    - 7500
    - 10000
    - 15000
    - 20000
    - 30000
    - 50000
    - 75000
    - 100000
    - 200000
    - 300000
    - 400000
    - 500000
    - 600000
    - 700000
    - 800000
    - 900000
    - 1000000
    - 1100000
    - 1200000
    - 1300000
    - 1400000
    - 1500000
    - 1600000
    - 1700000
    - 1800000
    - 1900000
    - 2000000
    - 2100000
    - 2200000
    - 2300000
    - 2400000
    - 2500000
    - 2600000
    - 2750000
    - 2900000
    - 3100000
    - 3400000
    - 3700000

  # An XP Gain method takes a trigger as the ID and a multiplier
  # The multiplier takes the value produced by the trigger and multiplies it
  # by some value to calculate the experience that should be given
  xp-gain-methods:
    - id: melee_attack
      multiplier: 0.5

  # Custom placeholders to be used in descriptions,
  # Don't add % to the IDs, this is done automatically
  # The value takes a %level% placeholder and is a mathetmatical expression
  level-placeholders:
    - id: "damage_multiplier"
      value: "%level%"

  # The text shown with the %effects% placeholder
  # The number dictates the minimum level for this text to show for
  # Adding new levels will override this text on those levels or above
  effects-description:
    1:
      - "&8» &8Gives a &a+%damage_multiplier%%&8 bonus to"
      - "   &8melee damage"

  # Same as above, but for %rewards%
  rewards-description:
    1:
      - "&8» &8Gives a &a+%damage_multiplier%%&8 bonus to"
      - "   &8melee damage"

  # Same as above, but for %level_up_messages%
  level-up-messages:
    1:
      - "&8» &8Gives a &a+%damage_multiplier%%&8 bonus to"
      - "   &8melee damage"

  # Commands to be sent on levelup, can be formatted two ways:
  # level:command (e.g. 10:eco give %player% 1000), which would execute that command for level 10
  # command (e.g. eco give %player% 5000), which would execute that command for all levels
  level-commands: [ ]

  # The effects for the pet, has %level% as a placeholder
  effects:
    - id: damage_multiplier
      args:
        multiplier: "%level% * 0.01 + 1"
      triggers:
        - melee_attack

  # The conditions for the pet, also has %level% as a placeholder
  conditions: [ ]

  # The texture of the pet entity in game
  # If you're using modelengine, use modelengine:id as the texture
  entity-texture: "eyJ0ZXh0dXJlcyI6eyJTS0lOIjp7InVybCI6Imh0dHA6Ly90ZXh0dXJlcy5taW5lY3JhZnQubmV0L3RleHR1cmUvOTA5NWZjYzFlM2Q3Y2JkMzUwZjE5YjM4OTQ5OGFiOGJiOTZjNjVhZDE4NWQzNDU5MjA2N2E3ZDAzM2FjNDhkZSJ9fX0="

  # The icon in GUIs
  icon: player_head texture:eyJ0ZXh0dXJlcyI6eyJTS0lOIjp7InVybCI6Imh0dHA6Ly90ZXh0dXJlcy5taW5lY3JhZnQubmV0L3RleHR1cmUvOTA5NWZjYzFlM2Q3Y2JkMzUwZjE5YjM4OTQ5OGFiOGJiOTZjNjVhZDE4NWQzNDU5MjA2N2E3ZDAzM2FjNDhkZSJ9fX0=

  # The spawn egg
  spawn-egg:
    enabled: true # If the pet should have a spawn egg
    item: blaze_spawn_egg unbreaking:1 hide_enchants
    name: "&6Tiger&f Spawn Egg"
    lore:
      - ""
      - "&8&oPlace on the ground to"
      - "&8&ounlock the &r&6Tiger&8&o pet!"
    craftable: false
    recipe: [ ]
   # recipe-permission: ecopets.craft.tiger
- id: Craft

  # The display name of the pet
  name: "&6Crafting Table"

  # The description of the pet
  description: "&8&oLevel up by Crafting"

  # The xp requirements for each pet level - add new levels by adding more to this list
  level-xp-requirements:
    - 50
    - 125
    - 200
    - 300
    - 500
    - 750
    - 1000
    - 1500
    - 2000
    - 3500
    - 5000
    - 7500
    - 10000
    - 15000
    - 20000
    - 30000
    - 50000
    - 75000
    - 100000
    - 200000
    - 300000
    - 400000
    - 500000
    - 600000
    - 700000
    - 800000
    - 900000
    - 1000000
    - 1100000
    - 1200000
    - 1300000
    - 1400000
    - 1500000
    - 1600000
    - 1700000
    - 1800000
    - 1900000
    - 2000000
    - 2100000
    - 2200000
    - 2300000
    - 2400000
    - 2500000
    - 2600000
    - 2750000
    - 2900000
    - 3100000
    - 3400000
    - 3700000

  # An XP Gain method takes a trigger as the ID and a multiplier
  # The multiplier takes the value produced by the trigger and multiplies it
  # by some value to calculate the experience that should be given
  xp-gain-methods:
    - id: craft
      multiplier: 1

  # Custom placeholders to be used in descriptions,
  # Don't add % to the IDs, this is done automatically
  # The value takes a %level% placeholder and is a mathetmatical expression
  level-placeholders:
    - id: "damage_multiplier"
      value: "%level%"

  # The text shown with the %effects% placeholder
  # The number dictates the minimum level for this text to show for
  # Adding new levels will override this text on those levels or above
  effects-description:
    1:
      - "&8» &8This Pet Has No Effects"

  # Same as above, but for %rewards%
  rewards-description:
    1:
      - "&8» &8This Pet Has No Effects"

  # Same as above, but for %level_up_messages%
  level-up-messages: [ ]
  
  # Commands to be sent on levelup, can be formatted two ways:
  # level:command (e.g. 10:eco give %player% 1000), which would execute that command for level 10
  # command (e.g. eco give %player% 5000), which would execute that command for all levels
  level-commands: [ ]

  # The effects for the pet, has %level% as a placeholder
  effects: [ ]

  # The conditions for the pet, also has %level% as a placeholder
  conditions: [ ]

  # The texture of the pet entity in game
  # If you're using modelengine, use modelengine:id as the texture
  entity-texture: "eyJ0ZXh0dXJlcyI6eyJTS0lOIjp7InVybCI6Imh0dHA6Ly90ZXh0dXJlcy5taW5lY3JhZnQubmV0L3RleHR1cmUvMmNkYzBmZWI3MDAxZTJjMTBmZDUwNjZlNTAxYjg3ZTNkNjQ3OTMwOTJiODVhNTBjODU2ZDk2MmY4YmU5MmM3OCJ9fX0="

  # The icon in GUIs
  icon: player_head texture:eyJ0ZXh0dXJlcyI6eyJTS0lOIjp7InVybCI6Imh0dHA6Ly90ZXh0dXJlcy5taW5lY3JhZnQubmV0L3RleHR1cmUvMmNkYzBmZWI3MDAxZTJjMTBmZDUwNjZlNTAxYjg3ZTNkNjQ3OTMwOTJiODVhNTBjODU2ZDk2MmY4YmU5MmM3OCJ9fX0=

  # The spawn egg
  spawn-egg:
    enabled: true # If the pet should have a spawn egg
    item: villager_spawn_egg unbreaking:1 hide_enchants
    name: "&Crafting Table&f Spawn Egg"
    lore:
      - ""
      - "&8&oPlace on the ground to"
      - "&8&ounlock the &r&6Crafting Table&8&o pet!"
    craftable: true
    recipe: 
      - ""
      - ""
      - ""
      - ""
      - "crafting_table"
      - ""
      - ""
      - ""
      - ""
     # recipe-permission: ecopets.craft.table
