# Task

Map game-specific keybinding names to standardized FPS schema given in the "Dummy Schema Reference". Using the JSON provided below for the "Game specific keybindings".

Map to closest matching "name" from the "Dummy Schema Reference" (check groupedActions if needed).
Be sure you don't map multiple keys to the same "name". Expand the "name" instead. For example:
If a game has two grenade types the player can throw, create an extra binding "name" with a logical and descriptive extension of the closest matching "name" for the second option, like so:

```json
    {
      "name": "Throw Grenade",
      "category": "combat",
      "groupedActions": ["Grenade", "Lethal Equipment", "Ordinance"],
      "defaultKey": "",
      "modifier": "",
      "notes": "Standard bind for throwing lethal explosives."
    },
    {
      "name": "Throw Grenade Special",
      "category": "combat",
      "groupedActions": [],
      "defaultKey": "",
      "modifier": "",
      "notes": "Standard bind for throwing special grenade."
    },
```


# Dummy Schema Reference

```json
{
  "bindings": [
    {
      "name": "Move Forward",
      "category": "movement",
      "groupedActions": ["Forward", "Throttle Up"],
      "defaultKey": "",
      "modifier": "",
      "notes": "Standard forward movement in virtually all FPS/TPS games."
    },
    {
      "name": "Move Backward",
      "category": "movement",
      "groupedActions": ["Backward", "Throttle Down"],
      "defaultKey": "",
      "modifier": "",
      "notes": "Standard backward movement in virtually all FPS/TPS games."
    },
    {
      "name": "Move Left",
      "category": "movement",
      "groupedActions": ["Strafe Left"],
      "defaultKey": "",
      "modifier": "",
      "notes": "Left strafe mapped next to W and S for easy access."
    },
    {
      "name": "Move Right",
      "category": "movement",
      "groupedActions": ["Strafe Right"],
      "defaultKey": "",
      "modifier": "",
      "notes": "Right strafe mapped next to W and S for easy access."
    },
    {
      "name": "Jump",
      "category": "movement",
      "groupedActions": ["Vault", "Climb", "Mantle", "Ascend", "Rappel"],
      "defaultKey": "",
      "modifier": "",
      "notes": "Often context-sensitive for vaulting or climbing in tactical shooters and pure jump in arcade shooters."
    },
    {
      "name": "Sprint",
      "category": "movement",
      "groupedActions": ["Run", "Boost", "Hold Breath"],
      "defaultKey": "",
      "modifier": "",
      "notes": "Used for sprinting or holding breath while aiming in many shooters."
    },
    {
      "name": "Crouch",
      "category": "movement",
      "groupedActions": ["Duck", "Slide", "Descend"],
      "defaultKey": "",
      "modifier": "",
      "notes": "Can initiate a slide when used while sprinting in many modern shooters."
    },
    {
      "name": "Prone",
      "category": "movement",
      "groupedActions": ["Lie Down", "Drop Shot"],
      "defaultKey": "",
      "modifier": "",
      "notes": "Common in tactical and military shooters for low profile movement."
    },
    {
      "name": "Walk",
      "category": "movement",
      "groupedActions": ["Slow Walk", "Stealth Mode"],
      "defaultKey": "",
      "modifier": "",
      "notes": "Reduces movement speed for stealth and sound discipline."
    },
    {
      "name": "Lean Left",
      "category": "movement",
      "groupedActions": ["Peek Left"],
      "defaultKey": "",
      "modifier": "",
      "notes": "Leaning bound to a mouse side button to keep WASD fingers free."
    },
    {
      "name": "Lean Right",
      "category": "movement",
      "groupedActions": ["Peek Right"],
      "defaultKey": "",
      "modifier": "",
      "notes": "Leaning bound to a mouse side button to keep WASD fingers free."
    },
    {
      "name": "Fire",
      "category": "combat",
      "groupedActions": ["Attack", "Shoot", "Swing"],
      "defaultKey": "",
      "modifier": "",
      "notes": "Primary attack for firearms and melee weapons in nearly all shooters."
    },
    {
      "name": "Aim",
      "category": "combat",
      "groupedActions": ["ADS", "Zoom", "Block", "Alt-Fire"],
      "defaultKey": "",
      "modifier": "",
      "notes": "Aiming down sights or blocking/alt-fire depending on game."
    },
    {
      "name": "Reload",
      "category": "combat",
      "groupedActions": ["Vent Heat", "Check Ammo"],
      "defaultKey": "",
      "modifier": "",
      "notes": "Reload or vent heat; often hold to check magazine in tactical games."
    },
    {
      "name": "Melee",
      "category": "combat",
      "groupedActions": ["Bash", "Knife", "Kick", "Parry"],
      "defaultKey": "",
      "modifier": "",
      "notes": "Quick close-range attack; may conflict with Push to Talk if sharing key."
    },
    {
      "name": "Throw Grenade",
      "category": "combat",
      "groupedActions": ["Grenade", "Lethal Equipment", "Ordinance"],
      "defaultKey": "",
      "modifier": "",
      "notes": "Standard bind for throwing lethal explosives."
    },
    {
      "name": "Switch Weapon",
      "category": "combat",
      "groupedActions": ["Next Weapon", "Previous Weapon", "Weapon Cycle"],
      "defaultKey": "",
      "modifier": "",
      "notes": "Mouse wheel cycling between available weapons."
    },
    {
      "name": "Holster Weapon",
      "category": "combat",
      "groupedActions": ["Put Away Weapon", "Lower Weapon"],
      "defaultKey": "",
      "modifier": "",
      "notes": "Used in tactical shooters to indicate non-hostility or move faster."
    },
    {
      "name": "Primary Weapon",
      "category": "combat",
      "groupedActions": ["Slot 1", "Rifle"],
      "defaultKey": "",
      "modifier": "",
      "notes": "Direct selection of main firearm."
    },
    {
      "name": "Secondary Weapon",
      "category": "combat",
      "groupedActions": ["Slot 2", "Pistol", "Sidearm"],
      "defaultKey": "",
      "modifier": "",
      "notes": "Direct selection of backup weapon."
    },
    {
      "name": "Fire Mode",
      "category": "combat",
      "groupedActions": ["Toggle Semi/Auto", "Burst Mode"],
      "defaultKey": "",
      "modifier": "",
      "notes": "Toggles between available firing modes on supported weapons."
    },
    {
      "name": "Interact",
      "category": "abilities",
      "groupedActions": ["Use", "Revive", "Pick Up", "Hack", "Plant"],
      "defaultKey": "",
      "modifier": "",
      "notes": "Context-sensitive interaction with world objects and teammates."
    },
    {
      "name": "Flashlight",
      "category": "abilities",
      "groupedActions": ["Torch", "Night Vision", "Laser Toggle"],
      "defaultKey": "",
      "modifier": "",
      "notes": "Toggles light or vision aids in dark environments."
    },
    {
      "name": "Ping",
      "category": "abilities",
      "groupedActions": ["Mark", "Spot", "Tag Enemy", "Place Marker"],
      "defaultKey": "",
      "modifier": "",
      "notes": "Marks locations or enemies for team communication."
    },
    {
      "name": "Use Consumable",
      "category": "abilities",
      "groupedActions": ["Heal", "Stim", "Medkit", "Armor Plate", "Potion"],
      "defaultKey": "",
      "modifier": "",
      "notes": "Activates bound consumable such as healing or armor."
    },
    {
      "name": "Map",
      "category": "tactical",
      "groupedActions": ["Tactical Map", "Objectives", "Mission Info"],
      "defaultKey": "",
      "modifier": "",
      "notes": "Displays world or tactical map and often objectives."
    },
    {
      "name": "Scoreboard",
      "category": "tactical",
      "groupedActions": ["Status Screen", "Team Loadout", "Mission Status"],
      "defaultKey": "",
      "modifier": "",
      "notes": "Shows current mission or match status; sometimes doubles as inventory."
    },
    {
      "name": "Voice Team",
      "category": "communication",
      "groupedActions": ["Push to Talk team", "Voice Chat Team"],
      "defaultKey": "",
      "modifier": "",
      "notes": "Hold to transmit voice to team."
    },
    {
      "name": "Voice All",
      "category": "communication",
      "groupedActions": ["Push to Talk all", "Voice Chat All"],
      "defaultKey": "",
      "modifier": "",
      "notes": "Hold to transmit voice to all."
    },
    {
      "name": "Text Chat Team",
      "category": "communication",
      "groupedActions": ["Team Chat"],
      "defaultKey": "",
      "modifier": "",
      "notes": "Opens text chat box and sends message to team."
    },
    {
      "name": "Text Chat All",
      "category": "communication",
      "groupedActions": ["All Chat"],
      "defaultKey": "",
      "modifier": "",
      "notes": "Opens text chat box and sends message to all."
    }
  ]
}
```

# Rules

1. Replace name with closest dummy schema match, keep original notes
2. If no good match exists, keep original game name
3. Preserve all actions, categories, keys, modifiers, notes exactly
4. Never drop actions
5. Never map multiple actions and keys to the same dummy name, create new unmapped actions instead

# Output Format (3 sections required)

## 1. Mapped JSON
[complete mapped JSON in code block]

## 2. Changed Names

List of the actions where the name and/or category changed.

## 3. Unmapped Actions

List of the actions where no similar default action was available.

# Provided Game Specific Keybindings

Get the "Game Specific Keybindings" from the attachment or the user prompt.
IMPORTANT: If no "Game Specific Keybindings" are available in the attachment or the user prompt, ask the user to provide them.