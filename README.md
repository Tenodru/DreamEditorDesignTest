# DreamEditorDesignTest
A design test I was assigned as part of a studio application. This test was done using the studio's provided engine, using Lua script.


## Project Description and Design
The initial part of this design test tasked me with following a series of brief tutorials that explained how specific parts of the editor worked - adding units, creating abilities and weapons, and so on.
Following this, the test became rather freeform, allowing me to create a mini-game of my own design, with a few requirements testing my knowledge of Lua. I chose to design a game that was heavily influenced by past projects like [A Numbers Game](https://github.com/Tenodru/ANumbersGame): a straightforward action-roguelike that features endless waves of enemies and an experience & upgrade system that provides scaling power and unlockable abilities for the player.

## Script Breakdown
- **[Trigger.lua.txt](EntryMap/Trigger.lua.txt)** : The bulk of written code is contained here. This script is where the triggers for EntryMap reside - systems including the experience and upgrade system, and the enemy spawning system, are located here.
- **[Ability.json](EntryMap/Ability.json)** : Contains a structured list of all abilities, which utilize *effects* to determine behavior when cast.
- **[Actor.json](EntryMap/Actor.json)** : Contains a structured list of all actors, or entities; actors are used by units and abilities alike to assign animations, models, and visual and sound FX.
- **[Behavior.json](EntryMap/Behavior.json)** : Contains a structured list of all behaviors, which act like buffs and debuffs for a unit. In this project, I utilized behaviors for the basic player stat upgrades, like health and movement speed.
- **[Effect.json](EntryMap/Effect.json)** : Contains a structured list of all effects. Effects take on multiple forms in this engine, from destroying units, to running area searches for subsequent effects, to initiating persistent actions.
- **[Unit.json](EntryMap/Unit.json)** : Contains a structured list of all units. Units have multiple components that determine their behavior, from health to collision detection.
- **[Weapon.json](EntryMap/Weapon.json)** : Contains a structured list of all weapons, which give units the ability to attack and determine how these attacks behave.
- **[Terrain.json](EntryMap/Terrain.json)** : Contains data that determines the shape and size of the map terrain. Map terrain edits were purely done through the engine.
