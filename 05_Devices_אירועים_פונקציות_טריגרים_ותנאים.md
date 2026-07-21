# Devices, אירועים, פונקציות, טריגרים ותנאים

> **מטרת הקובץ:** להסביר את שפת העבודה עם Devices ואת בניית הלוגיקה באמצעות Events, Functions, Direct Event Binding, קלט ותנאים.  
> **מתי להשתמש בו:** כאשר מפרקים מכניקה למערכת Devices או פותרים בעיית חיבור בין התקנים.  
> **לא כלול:** Devices שעיקרם תנועה במרחב, שחקנים, HUD, AI או ניקוד כאשר הם מתועדים בקבצים ייעודיים.  
> **מקורות עיקריים:** `06_יסודות_Devices_ואירועים(1).md`, `07A_קלט_טריגרים_תנאים_והחלטות(1).md`

## תוכן עניינים

- [Using Devices in Fortnite](#using-devices-in-fortnite)
- [Creating Gameplay with Devices in Fortnite](#creating-gameplay-with-devices-in-fortnite)
- [Getting Started with Devices in Fortnite](#getting-started-with-devices-in-fortnite)
- [Getting Started with Direct Event Binding in Fortnite Creative](#getting-started-with-direct-event-binding-in-fortnite-creative)
- [Using Attribute Evaluator Devices in Fortnite Creative](#using-attribute-evaluator-devices-in-fortnite-creative)
- [Using Button Devices in Fortnite Creative](#using-button-devices-in-fortnite-creative)
- [Using Channel Devices in Fortnite Creative](#using-channel-devices-in-fortnite-creative)
- [Using Conditional Button Devices in Fortnite Creative](#using-conditional-button-devices-in-fortnite-creative)
- [Using Input Trigger Devices in Fortnite Creative](#using-input-trigger-devices-in-fortnite-creative)
- [Using Perception Trigger Devices in Fortnite Creative](#using-perception-trigger-devices-in-fortnite-creative)
- [Using Player Counter Devices in Fortnite Creative](#using-player-counter-devices-in-fortnite-creative)
- [Using Pulse Trigger Devices in Fortnite Creative](#using-pulse-trigger-devices-in-fortnite-creative)
- [Using Random Number Generator Devices in Fortnite Creative](#using-random-number-generator-devices-in-fortnite-creative)
- [Using Signal Remote Manager Devices in Fortnite Creative](#using-signal-remote-manager-devices-in-fortnite-creative)
- [Using Skilled Interaction Devices in Fortnite Creative](#using-skilled-interaction-devices-in-fortnite-creative)
- [Using Switch Devices in Fortnite Creative](#using-switch-devices-in-fortnite-creative)
- [Using Timer Devices in Fortnite Creative](#using-timer-devices-in-fortnite-creative)
- [Using Trigger Devices in Fortnite Creative](#using-trigger-devices-in-fortnite-creative)
- [Using Volume Devices in Fortnite Creative](#using-volume-devices-in-fortnite-creative)
- [Using Voting Group and Voting Options Devices in Fortnite](#using-voting-group-and-voting-options-devices-in-fortnite)

---
## Using Devices in Fortnite

**כותרת מקורית:** Using Devices in Fortnite  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/using-devices-in-fortnite  
**מקור קלט:** `06_יסודות_Devices_ואירועים(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `using-devices-in-fortnite`

**
Devices **are an important part of your toolset for setting up interactive experiences on your islands.

By customizing devices and combining them with other devices, you can build specific [game mechanics](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#game-mechanics).

You can also make a device more versatile by using Verse in UEFN!

Any Creative design examples described in the device docs themselves or in the [Device Design Examples](https://dev.epicgames.com/documentation/fortnite/device-design-examples-in-fortnite-creative) can also be made using [Unreal Editor for Fortnite (UEFN)](https://dev.epicgames.com/documentation/en-us/uefn/devices-in-unreal-editor-for-fortnite).

#### The Device Advantage — Read This First!

Ever wondered why devices are important to gameplay?

- [

Creating Gameplay with Devices

Find out what devices actually are, how they work, and why they can save you hours of unnecessary programming!

](https://dev.epicgames.com/documentation/fortnite/creating-gameplay-with-devices-in-fortnite)

#### Explore the Devices

For information on **Fortnite Patchwork devices**, see [Patchwork Devices](https://dev.epicgames.com/documentation/fortnite/using-patchwork-devices-in-fortnite-creative).

- [
*

Creating Gameplay with Devices

Find out what devices actually are, how they work, and why they can save you hours of unnecessary programming!

](https://dev.epicgames.com/documentation/fortnite/creating-gameplay-with-devices-in-fortnite)
- [

Getting Started with Devices

Learn how to add and modify devices in Fortnite, and how to use Verse to expand device functionality!

](https://dev.epicgames.com/documentation/fortnite/getting-started-with-devices-in-fortnite)
- [

UEFN-Only Devices

Learn about using devices in UEFN and Verse!

](https://dev.epicgames.com/documentation/fortnite/uefnonly-devices-in-fortnite)
- [

Accolades Devices

Help players earn Battle Pass XP using the Accolades device!

](https://dev.epicgames.com/documentation/fortnite/using-accolades-devices-in-fortnite-creative)
- [

Advanced Storm Controller Beacon Devices

Customize individual storm phases when you use the Advanced Storm Controller.

](https://dev.epicgames.com/documentation/fortnite/using-advanced-storm-controller-beacon-devices-in-fortnite-creative)
- [

Advanced Storm Controller Devices

Create a Battle Royale-style, multiple-phase storm, and control its size, movement and damage for each phase.

](https://dev.epicgames.com/documentation/fortnite/using-advanced-storm-controller-devices-in-fortnite-creative)
- [

AI Navigation Modification Devices

Use this device to block off areas so AI enemies can't spawn or enter there.

](https://dev.epicgames.com/documentation/fortnite/using-ai-navigation-modification-devices-in-fortnite-creative)
- [

AI Patrol Path Node Devices

Add patrol paths for guards to increase the challenge of your game.

](https://dev.epicgames.com/documentation/fortnite/using-ai-patrol-path-node-devices-in-fortnite-creative)
- [

Air Vent Devices

This device boosts players up into the air.

](https://dev.epicgames.com/documentation/fortnite/using-air-vent-devices-in-fortnite-creative)
- [

Analytics Devices

Level up your understanding of player behavior by setting custom-measuring actions on your island!

](https://dev.epicgames.com/documentation/fortnite/using-analytics-devices-in-fortnite-creative)
- [

Armored Battle Bus Spawner Device

Trick out your map with an Armored Battle Bus players can drive and use to destroy buildings and eliminate other players.

](https://dev.epicgames.com/documentation/fortnite/using-armored-battle-bus-spawner-devices-in-fortnite-creative)
- [

Armored Transport Spawner Devices

Use this armored transport to provide more opportunities for players to plan and perform heists on your island!

](https://dev.epicgames.com/documentation/fortnite/using-armored-transport-spawner-devices-in-fortnite-creative)
- [

Ascender Devices

Create new ways for players to move around your island with the Ascender device!

](https://dev.epicgames.com/documentation/fortnite/using-ascender-devices-in-fortnite-creative)
- [

ATK Spawner Devices

Race over all kinds of terrain with an ATK vehicle!

](https://dev.epicgames.com/documentation/fortnite/using-atk-spawner-devices-in-fortnite-creative)
- [

Attribute Evaluator Devices

This device transmits an event based on the attributes of any triggering player.

](https://dev.epicgames.com/documentation/fortnite/using-attribute-evaluator-devices-in-fortnite-creative)
- [

Audio Player Devices

Use this device to play sound effects to create immersive atmospheres for your players.

](https://dev.epicgames.com/documentation/fortnite/using-audio-player-devices-in-fortnite-creative)
- [

Audio Mixer Devices

The Audio Mixer device gives you professional control over the game's volume mix and more.

](https://dev.epicgames.com/documentation/fortnite/using-audio-mixer-devices-in-fortnite-creative)
- [

Automated Turret Devices

Use this customizable turret that scans for nearby targets on its own. You can set target types and other behaviors, and change these using events.

](https://dev.epicgames.com/documentation/fortnite/using-automated-turret-devices-in-fortnite-creative)
- [

Ball Spawner Devices

Spawn a ball that your players can knock around!

](https://dev.epicgames.com/documentation/fortnite/using-ball-spawner-devices-in-fortnite-creative)
- [

Baller Spawner Devices

Place a Baller vehicle in your game for your players to drive.

](https://dev.epicgames.com/documentation/fortnite/using-baller-spawner-devices-in-fortnite-creative)
- [

Bank Vault Devices

Place this bank vault in buildings on your island to create a heist mechanic in your game.

](https://dev.epicgames.com/documentation/fortnite/using-bank-vault-devices-in-fortnite-creative)
- [

Barrier Devices

This device creates an impenetrable zone to block both players and weapon fire.

](https://dev.epicgames.com/documentation/fortnite/using-barrier-devices-in-fortnite-creative)
- [

Basic Storm Controller Devices

Create a single-phase storm and control its size, movement and damage.

](https://dev.epicgames.com/documentation/fortnite/using-basic-storm-controller-devices-in-fortnite-creative)
- [

Beacon Devices

Use the Beacon device to display a visual effect or a HUD Marker (or both!) at a specific location.

](https://dev.epicgames.com/documentation/fortnite/using-beacon-devices-in-fortnite-creative)
- [

Big Rig Spawner Devices

Place a semi truck vehicle in your game for your players to drive.

](https://dev.epicgames.com/documentation/fortnite/using-big-rig-spawner-devices-in-fortnite-creative)
- [

Billboard Devices

Provide custom text messages to players on billboards.

](https://dev.epicgames.com/documentation/fortnite/using-billboard-devices-in-fortnite-creative)
- [

Biplane Spawner Devices

Place a biplane vehicle in your game for your players to fly.

](https://dev.epicgames.com/documentation/fortnite/using-biplane-spawner-devices-in-fortnite-creative)
- [

Boat Spawner Devices

Race across the water with a motorboat using this device!

](https://dev.epicgames.com/documentation/fortnite/using-boat-spawner-devices-in-fortnite-creative)
- [

Bomb Flower Devices

Place a plant pod in the environment that players can hit with a pickaxe to toss a bomb toward enemies.

](https://dev.epicgames.com/documentation/fortnite/using-bomb-flower-devices-in-fortnite-creative)
- [

Bouncer Gallery Devices

You can choose from many types of bouncers that launch players into the air.

](https://dev.epicgames.com/documentation/fortnite/using-bouncer-gallery-devices-in-fortnite-creative)
- [

Button Devices

Use buttons to trigger other devices on your island.

](https://dev.epicgames.com/documentation/fortnite/using-button-devices-in-fortnite-creative)
- [

Campfire Devices

Place campfires players can use to heal themselves.

](https://dev.epicgames.com/documentation/fortnite/using-campfire-devices-in-fortnite-creative)
- [

Cannon Spawner Devices

Add a movable cannon players can use to attack enemies or structures.

](https://dev.epicgames.com/documentation/fortnite/using-cannon-spawner-devices-in-fortnite-creative)
- [

Capture Area Devices

Use the Capture Area device to create a zone for item drop-off or point-capture objectives.

](https://dev.epicgames.com/documentation/fortnite/using-capture-area-devices-in-fortnite)
- [

Capture Item Spawner Devices

Spawn and track a single capturable item as your game objective.

](https://dev.epicgames.com/documentation/fortnite/using-capture-item-spawner-devices-in-fortnite-creative)
- [

Carryable Spawner Devices

Use the Carryable device to give players objects they can throw at other players.

](https://dev.epicgames.com/documentation/fortnite/using-carryable-spawner-devices-in-fortnite)
- [

Chair Devices

Create movie theaters, roller coasters, and other seated interactions with this device.

](https://dev.epicgames.com/documentation/fortnite/using-chair-devices-in-fortnite-creative)
- [

Changing Booth Devices

Place a Changing Booth so players can access their lockers and swap outfits during the game.

](https://dev.epicgames.com/documentation/fortnite/using-changing-booth-devices-in-fortnite-creative)
- [

Channel Devices

Use this device to simplify the connections between your devices.

](https://dev.epicgames.com/documentation/fortnite/using-channel-devices-in-fortnite-creative)
- [

Character Device Controller Devices

Control characters by groups — make one group dance while another group cries!

](https://dev.epicgames.com/documentation/fortnite/using-character-device-controller-devices-in-fortnite-creative)
- [

Character Devices

Create a character that can be customized and posed.

](https://dev.epicgames.com/documentation/fortnite/using-character-devices-in-fortnite-creative)
- [

Chest and Ammo Gallery Devices

This gallery offers items that will aid players in combat gameplay.

](https://dev.epicgames.com/documentation/fortnite/using-chest-and-ammo-gallery-devices-in-fortnite-creative)
- [

Class Designer Devices

Define custom classes and assign specific attributes and inventory loadouts for each class.

](https://dev.epicgames.com/documentation/fortnite/using-class-designer-devices-in-fortnite-creative)
- [

Class Selector Devices

Put those custom classes you made with Class Designer to work on your island for new kinds of gameplay.

](https://dev.epicgames.com/documentation/fortnite/using-class-selector-devices-in-fortnite-creative)
- [

Class Selector UI Devices

Create a UI element that lists the classes that players can choose from.

](https://dev.epicgames.com/documentation/fortnite/using-class-selector-ui-devices-in-fortnite-creative)
- [

Collectibles Object Devices

Place themed, customizable resources for players to collect throughout gameplay.

](https://dev.epicgames.com/documentation/fortnite/using-collectibles-object-devices-in-fortnite-creative)
- [

Color Changing Tile Devices

This device creates a tile that changes color when players interact with it.

](https://dev.epicgames.com/documentation/fortnite/using-color-changing-tile-devices-in-fortnite-creative)
- [

Conditional Button Devices

Create a button that can only be activated when players are carrying specific items.

](https://dev.epicgames.com/documentation/fortnite/using-conditional-button-devices-in-fortnite-creative)
- [

Crash Pad Devices

Place a crash pad that can bounce players and save them from fall damage.

](https://dev.epicgames.com/documentation/fortnite/using-crash-pad-devices-in-fortnite-creative)
- [

Developer Profile Devices

Use this device to display a QR code that links to your profile in Creator Portal.

](https://dev.epicgames.com/documentation/fortnite/using-creator-profile-link-devices-in-fortnite-creative)
- [

Creature Manager Devices

Use this device to customize a single creature type.

](https://dev.epicgames.com/documentation/fortnite/using-creature-manager-devices-in-fortnite-creative)
- [

Creature Placer Devices

Place creatures at the exact location where you want them.

](https://dev.epicgames.com/documentation/fortnite/using-creature-placer-devices-in-fortnite-creative)
- [

Creature Spawner Devices

Use Creature Spawner Devices to spawn enemies that can attack players.

](https://dev.epicgames.com/documentation/fortnite/using-creature-spawner-devices-in-fortnite-creative)
- [

Creepin' Cardboard Devices

Place Creepin' Cardboard devices for players to hide in and sneak around.

](https://dev.epicgames.com/documentation/fortnite/using-creepin-cardboard-devices-in-fortnite-creative)
- [

Crowd Volume Devices

Build an NPC audience to cheer your game!

](https://dev.epicgames.com/documentation/fortnite/using-crowd-volume-devices-in-fortnite-creative)
- [

Customizable Light Devices

This device is a light that can have a customized color.

](https://dev.epicgames.com/documentation/fortnite/using-customizable-light-devices-in-fortnite-creative)
- [

D-Launcher Devices

Launch players in various directions as a traversal aid or a hazard.

](https://dev.epicgames.com/documentation/fortnite/using-dlauncher-devices-in-fortnite-creative)
- [

Damage Amplifier Powerup Devices

Players can boost their damage potential with this potent powerup!

](https://dev.epicgames.com/documentation/fortnite/using-damage-amplifier-powerup-devices-in-fortnite-creative)
- [

Damage Volume Devices

Create a zone that can damage or eliminate players, vehicles, and creatures.

](https://dev.epicgames.com/documentation/fortnite/using-damage-volume-devices-in-fortnite-creative)
- [

Dance Mannequin Devices

The Dance Mannequin projects a hologram image of a character performing various dance emotes.

](https://dev.epicgames.com/documentation/fortnite/using-dance-mannequin-devices-in-fortnite-creative)
- [

Day Sequence Device in Creative

Create custom outdoor lighting on your island with the Day Sequence device.

](https://dev.epicgames.com/documentation/fortnite/day-sequence-device-in-fortnite-creative)
- [

Dirt Bike Spawner Devices

Place a fast, agile vehicle that players can ride.

](https://dev.epicgames.com/documentation/fortnite/using-dirt-bike-spawner-devices-in-fortnite-creative)
- [

Disguise Devices

Use the Disguise device to provide players the option to hide their true identity.

](https://dev.epicgames.com/documentation/fortnite/using-disguise-devices-in-fortnite)
- [

Down But Not Out Devices

Customize the DBNO state in your game.

](https://dev.epicgames.com/documentation/fortnite/using-down-but-not-out-devices-in-fortnite-creative)
- [

Driftboard Spawner Devices

Race through the air on a Driftboard!

](https://dev.epicgames.com/documentation/fortnite/using-driftboard-spawner-devices-in-fortnite-creative)
- [

Earth Sprite Devices

Place Earth Sprites around your island to give players a place to exchange something and receive loot!

](https://dev.epicgames.com/documentation/fortnite/using-earth-sprite-devices-in-fortnite-creative)
- [

Elimination Manager Devices

Place items in this device and the items will drop when a player or other target is eliminated.

](https://dev.epicgames.com/documentation/fortnite/using-elimination-manager-devices-in-fortnite-creative)
- [

End Game Devices

Determine when to end a round or game.

](https://dev.epicgames.com/documentation/fortnite/using-end-game-devices-in-fortnite-creative)
- [

Explosive Devices

Make things go boom!

](https://dev.epicgames.com/documentation/fortnite/using-explosive-devices-in-fortnite-creative)
- [

Fang Spawner Devices

Spawn cool cars on your island to give players a fast and stylish vehicle they can use to get around!

](https://dev.epicgames.com/documentation/fortnite/using-fang-spawner-devices-in-fortnite-creative)
- [

Fire Volume Devices

Specify where the player can set things on fire, and ignite or extinguish flames using channels.

](https://dev.epicgames.com/documentation/fortnite/using-fire-volume-devices-in-fortnite-creative)
- [

Firefly Spawner Devices

Place this device to spawn collectible fireflies that can cause fire destruction during combat.

](https://dev.epicgames.com/documentation/fortnite/using-firefly-spawner-devices-in-fortnite-creative)
- [

First Person Camera Devices

Use this device to create games that use a first-person perpective, such as first-person shooters.

](https://dev.epicgames.com/documentation/fortnite/using-first-person-camera-devices-in-fortnite-creative)
- [

Fishing Rod Barrel Devices

Place Fishing Rod Barrel devices next to your Fishing Zones so players can fish!

](https://dev.epicgames.com/documentation/fortnite/using-fishing-rod-barrel-devices-in-fortnite-creative)
- [

Fishing Zone Devices

Use this device to create fishing zones for a game.

](https://dev.epicgames.com/documentation/fortnite/using-fishing-zone-devices-in-fortnite-creative)
- [

Fixed Angle Camera Devices

Use this camera to frame the player from a certain angle and follow their movement.

](https://dev.epicgames.com/documentation/fortnite/using-fixed-angle-camera-devices-in-fortnite-creative)
- [

Fixed Point Camera Devices

Use this fixed point camera to focus the player's view on particular locations or scenes.

](https://dev.epicgames.com/documentation/fortnite/using-fixed-point-camera-devices-in-fortnite-creative)
- [

Fuel Pump Devices

Place Fuel Pumps for players to refuel vehicles, or target with weapons to inflict damage on opponents.

](https://dev.epicgames.com/documentation/fortnite/using-fuel-pump-devices-in-fortnite-creative)
- [

Grind Powerup Devices

Give your players a speed boost with this device!

](https://dev.epicgames.com/documentation/fortnite/grind-powerup-devices)
- [

Grind Rail Devices

Place a customizable rail that you can move and shape for the perfect grind!

](https://dev.epicgames.com/documentation/fortnite/using-grind-rail-devices-in-fortnite-creative)
- [

Guard Spawner Devices

Raise the stakes for your players by spawning guards to attack them!

](https://dev.epicgames.com/documentation/fortnite/using-guard-spawner-devices-in-fortnite-creative)
- [

Hammerhead Choppa Spawner Devices

Let players move across your island in a flying tactical vehicle.

](https://dev.epicgames.com/documentation/fortnite/using-hammerhead-choppa-spawner-devices-in-fortnite)
- [

Healing Cactus Devices

Place this cactus in your island environment to provide an additional source of healing for players.

](https://dev.epicgames.com/documentation/fortnite/using-healing-cactus-devices-in-fortnite-creative)
- [

Health Powerup Devices

This device regenerates a player's health and shields.

](https://dev.epicgames.com/documentation/fortnite/using-health-powerup-devices-in-fortnite-creative)
- [

Heavy Turret Devices

Give players a weapon that can eliminate vehicles on the ground or in the sky!

](https://dev.epicgames.com/documentation/fortnite/using-heavy-turret-devices-in-fortnite-creative)
- [

Helicopter Spawner Devices

Move across your island in style with a helicopter!

](https://dev.epicgames.com/documentation/fortnite/using-helicopter-spawner-devices-in-fortnite-creative)
- [

Hero Device

Add powered characters that players can transform into with the Hero device.

](https://dev.epicgames.com/documentation/fortnite/using-hero-devices-in-fortnite)
- [

Hiding Prop Gallery Devices

Add these props to your island to give players a place to hide, and use them to create new Hide-and-Seek games.

](https://dev.epicgames.com/documentation/fortnite/using-hiding-prop-gallery-devices-in-fortnite-creative)
- [

Holoscreen Devices

Create a holographic screen that displays a clock or other images.

](https://dev.epicgames.com/documentation/fortnite/using-holoscreen-devices-in-fortnite-creative)
- [

Hover Platform Devices

Use Hover Platform devices in your game to create platforms in mid-air.

](https://dev.epicgames.com/documentation/fortnite/using-hover-platform-devices-in-fortnite-creative)
- [

HUD Controller Devices

You can use this device to show or hide parts of the player's HUD.

](https://dev.epicgames.com/documentation/fortnite/using-hud-controller-devices-in-fortnite-creative)
- [

HUD Message Devices

Create custom HUD messages for players based on time or activities.

](https://dev.epicgames.com/documentation/fortnite/using-hud-message-devices-in-fortnite-creative)
- [

Input Trigger Devices

Learn how to trigger events with player input or by activating with other devices.

](https://dev.epicgames.com/documentation/fortnite/using-input-trigger-devices-in-fortnite-creative)
- [

Items Gallery Devices

Use the Items Gallery to offer players a quick status buff.

](https://dev.epicgames.com/documentation/fortnite/using-items-gallery-devices-in-fortnite-creative)
- [

Item Granter Devices

Use this device to grant items to a player during the game.

](https://dev.epicgames.com/documentation/fortnite/using-item-granter-devices-in-fortnite-creative)
- [

Item Placer Devices

Place weapons or items in a more realistic way, such as sitting on a table or hanging on a wall.

](https://dev.epicgames.com/documentation/fortnite/using-item-placer-devices-in-fortnite-creative)
- [

Item Remover Devices

Make players drop or lose items when they are downed.

](https://dev.epicgames.com/documentation/fortnite/using-item-remover-devices-in-fortnite-creative)
- [

Item Spawner Devices

Use Item Spawner Devices to spawn items that players can pick up and use.

](https://dev.epicgames.com/documentation/fortnite/using-item-spawner-devices-in-fortnite-creative)
- [

Level Instance Devices

Use this device to save a collection of structures, terrain or props, and copy-paste the collection all over your island.

](https://dev.epicgames.com/documentation/fortnite/using-level-instance-devices-in-fortnite-creative)
- [

Level Loader Devices

Load levels created and saved with the Level Instance device, then move, rotate or stack the levels on top of each other.

](https://dev.epicgames.com/documentation/fortnite/using-level-loader-devices-in-fortnite-creative)
- [

Lock Devices

Attach this device to a wall section with a door to allow the door to be opened, closed, locked and unlocked using receivers.

](https://dev.epicgames.com/documentation/fortnite/using-lock-devices-in-fortnite-creative)
- [

Map Indicator Devices

Place custom points of interest and markers to orient players and direct their attention.

](https://dev.epicgames.com/documentation/fortnite/using-map-indicator-devices-in-fortnite-creative)
- [

Matchmaking Portal Devices

Place a portal on your island to take players to a different island.

](https://dev.epicgames.com/documentation/fortnite/using-matchmaking-portal-devices-in-fortnite-creative)
- [

Melee Designer Devices

Customize melee weapons with secondary actions, charge attacks, and more!

](https://dev.epicgames.com/documentation/fortnite/using-melee-designer-devices-in-fortnite-creative)
- [

Message Feed Devices

Using this device, you can create customized messages that display in a player's message feed.

](https://dev.epicgames.com/documentation/fortnite/using-message-feed-devices-in-fortnite-creative)
- [

Mounted Turret Devices

Place this turret for players to use as a mounted artillery weapon.

](https://dev.epicgames.com/documentation/fortnite/using-mounted-turret-devices-in-fortnite-creative)
- [

Movement Modulator Devices

Temporarily change the speed of players and vehicles using Movement Modulators.

](https://dev.epicgames.com/documentation/fortnite/using-movement-modulator-devices-in-fortnite-creative)
- [

Mutator Zone Devices

The Mutator Zone applies effects to players or creatures within the zone.

](https://dev.epicgames.com/documentation/fortnite/using-mutator-zone-devices-in-fortnite-creative)
- [

Nitro Barrel Devices

Players can destroy this barrel to apply Nitro to players or vehicles near the location of the barrel.

](https://dev.epicgames.com/documentation/fortnite/using-nitro-barrel-devices-in-fortnite-creative)
- [

Nitro Drifter Spawner Devices

Time to drift! Use these Cyber-City themed cars in your racing games or anywhere you want a fast, stylish vehicle for players to use.

](https://dev.epicgames.com/documentation/fortnite/using-nitro-drifter-spawner-devices-in-fortnite-creative)
- [

Nitro Hoop Devices

Use this flaming hoop to accelerate players and vehicles passing through it by infusing them with Nitro!

](https://dev.epicgames.com/documentation/fortnite/using-nitro-hoop-devices-in-fortnite-creative)
- [

Objective Devices

Choose from multiple objects that can be set as the objectives for a game

](https://dev.epicgames.com/documentation/fortnite/using-objective-devices-in-fortnite-creative)
- [

Octane Spawner Devices

Boost your gameplay by using Rocket League's Octane vehicles.

](https://dev.epicgames.com/documentation/fortnite/using-octane-spawner-devices-in-fortnite-creative)
- [

Orbit Camera Devices

Set up a camera that follows a character but that the player can rotate freely.

](https://dev.epicgames.com/documentation/fortnite/using-orbit-camera-devices-in-fortnite-creative)
- [

Overlord Spire Devices

Use the Overlord Spire to create large boss-like encounters that really challenge your players!

](https://dev.epicgames.com/documentation/fortnite/using-overlord-spire-devices-in-fortnite)
- [

Perception Trigger Devices

Make things happen based on line of sight to players.

](https://dev.epicgames.com/documentation/fortnite/using-perception-trigger-devices-in-fortnite-creative)
- [

Physics Boulder Devices

Use this rolling boulder to create new hazards and obstacles for your players to overcome.

](https://dev.epicgames.com/documentation/fortnite/using-physics-boulder-devices-in-fortnite-creative)
- [

Physics Tree Devices

Place a tree that can be chopped down, and the falling tree can damage structures, vehicles, players or creatures. This can create new hazards and obstacles for your players to overcome.

](https://dev.epicgames.com/documentation/fortnite/using-physics-tree-devices-in-fortnite-creative)
- [

Pickup Truck Spawner Devices

Use this classic pickup truck to put the pedal to the metal!

](https://dev.epicgames.com/documentation/fortnite/using-pickup-truck-spawner-devices-in-fortnite-creative)
- [

Pinball Bumper Devices

Use Pinball Bumper devices in your game to move, damage, and give score to your players.

](https://dev.epicgames.com/documentation/fortnite/using-pinball-bumper-devices-in-fortnite-creative)
- [

Pinball Flipper Devices

The Pinball Flipper can knock players back, damage them, and give them score.

](https://dev.epicgames.com/documentation/fortnite/using-pinball-flipper-devices-in-fortnite-creative)
- [

Placeable Ledge Devices

Place a ledge anywhere — even midair — that players can use to launch!

](https://dev.epicgames.com/documentation/fortnite/using-placeable-ledge-devices-in-fortnite-creative)
- [

Player Checkpoint Devices

This device sets a player's spawn point when activated, and can also be used to clear player inventories.

](https://dev.epicgames.com/documentation/fortnite/using-player-checkpoint-devices-in-fortnite-creative)
- [

Player Counter Devices

Use to find out how many players are in a certain area of your island.

](https://dev.epicgames.com/documentation/fortnite/using-player-counter-devices-in-fortnite-creative)
- [

Player Marker Devices

Mark player positions and display different kinds of information for marked players.

](https://dev.epicgames.com/documentation/fortnite/using-player-marker-devices-in-fortnite-creative)
- [

Player Movement Devices

Use the Player Movement device to customize the way players move on your island based on the island’s gameplay mechanics, gameplay cameras, teams, and more.

](https://dev.epicgames.com/documentation/fortnite/using-player-movement-devices)
- [

Player Reference Devices

Stores player data that can be sent to other devices and displayed to players.

](https://dev.epicgames.com/documentation/fortnite/using-player-reference-devices-in-fortnite-creative)
- [

Player Spawner Devices

Use Player Spawn Pad Devices to spawn players onto your island.

](https://dev.epicgames.com/documentation/fortnite/using-player-spawn-pad-devices-in-fortnite-creative)
- [

Pop-Up Dialog Devices

Create text boxes that give players information or that prompt them to make a choice.

](https://dev.epicgames.com/documentation/fortnite/using-popup-dialog-devices-in-fortnite-creative)
- [

Post Process Devices

Add effects to set a mood or enhance your game mechanics.

](https://dev.epicgames.com/documentation/fortnite/using-post-processing-devices-in-fortnite-creative)
- [

Progress Based Mesh Devices

Learn to use the Progress Based Mesh device to create a visual representation of progress.

](https://dev.epicgames.com/documentation/fortnite/using-progress-based-mesh-devices-in-fortnite)
- [

Prop Manipulator Devices

Customize your props the way you would customize a device.

](https://dev.epicgames.com/documentation/fortnite/using-prop-manipulator-devices-in-fortnite-creative)
- [

Prop Mover Devices

Attach this device to a building piece or terrain prop to create moving platforms, capture areas that move around, complex traversal, or more diverse shooting galleries.

](https://dev.epicgames.com/documentation/fortnite/using-prop-mover-devices-in-fortnite-creative)
- [

Prop-O-Matic Manager Devices

With this device you can customize Prop-o-Matic game rules and HUD elements.

](https://dev.epicgames.com/documentation/fortnite/using-propomatic-manager-devices-in-fortnite-creative)
- [

Pulse Trigger Devices

Send a pulse through a customizable volume to damage players or activate other devices.

](https://dev.epicgames.com/documentation/fortnite/using-pulse-trigger-devices-in-fortnite-creative)
- [

Quadcrasher Spawner Devices

Place a Quadcrasher vehicle in your game for your players to drive.

](https://dev.epicgames.com/documentation/fortnite/using-quadcrasher-spawner-devices-in-fortnite-creative)
- [

Race Checkpoint Devices

The Race Checkpoint device enables designers to make racing games.

](https://dev.epicgames.com/documentation/fortnite/using-race-checkpoint-devices-in-fortnite-creative)
- [

Race Manager Devices

The Race Manager device enables designers to create advanced racing modes.

](https://dev.epicgames.com/documentation/fortnite/using-race-manager-devices-in-fortnite-creative)
- [

Random Number Generator Devices

Generate a random number and use it to trigger other devices.

](https://dev.epicgames.com/documentation/fortnite/using-random-number-generator-devices-in-fortnite-creative)
- [

Real Time Clock Devices

Use this to tie in-game events to real time.

](https://dev.epicgames.com/documentation/fortnite/using-real-time-clock-devices-in-fornite-creative)
- [

Reboot Van Spawner Devices

Place a device that spawns Reboot Vans in your islands to give players a way to revive eliminated team members!

](https://dev.epicgames.com/documentation/fortnite/using-reboot-van-spawner-devices-in-fortnite-creative)
- [

Rift Point Volume Devices

Use the Rift Point Volume device to use a bomb similar to the one used in Ballistic.

](https://dev.epicgames.com/documentation/fortnite/using-rift-point-volume-devices-in-fortnite-creative)
- [

Rocket Boost Powerup Devices

Use this to fuel up the Boost in your Octane vehicles.

](https://dev.epicgames.com/documentation/fortnite/usingrocketboostpowerupdevicesinfortnitecreative)
- [

Rocket Racing Boost Pad Devices

Give all players a uniform speed boost during the race!

](https://dev.epicgames.com/documentation/fortnite/using-rocket-racing-boost-pad-devices-in-unreal-editor-for-fortnite)
- [

Rocket Racing EMP Volume Hazard Devices

Slow players down in your races with this device.

](https://dev.epicgames.com/documentation/fortnite/using-rocket-racing-emp-volume-devices-in-unreal-editor-for-fortnite)
- [

Rocket Racing Track Devices

Add and manipulate tracks for your RR racing game.

](https://dev.epicgames.com/documentation/fortnite/using-rocket-racing-track-devices-in-unreal-editor-for-fortnite)
- [

Rocket Racing Vehicle Spawner Device

Customize this vehicle to use the same game mechanics as Rocket Racing, but on your own island.

](https://dev.epicgames.com/documentation/fortnite/using-rocket-racing-vehicle-spawner-devices-in-fortnite-creative)
- [

Roly Poly Devices

Add Roly Poly devices to your island for a bug filled adventure.

](https://dev.epicgames.com/documentation/fortnite/using-roly-poly-devices-in-fortnite)
- [

Round Settings Devices

With this device, developers can further customize individual game rounds, or all rounds in the game.

](https://dev.epicgames.com/documentation/fortnite/using-round-settings-devices-in-fortnite-creative)
- [

Save Point Devices

The Save Point device gives players the ability to save progress, location, resources and stats so they can leave the game and come back without starting over.

](https://dev.epicgames.com/documentation/fortnite/using-save-point-devices-in-fortnite-creative)
- [

Score Manager Devices

This device sets or changes player scores when activated.

](https://dev.epicgames.com/documentation/fortnite/using-score-manager-devices-in-fortnite-creative)
- [

Scout Spire Devices

The Scout Spire adds a challenge to any environment with its charged, player tracking lasers and customizability.

](https://dev.epicgames.com/documentation/fortnite/using-scout-spire-devices-in-fortnite)
- [

Sedan Spawner Devices

Place a sedan vehicle in your game for your players to drive.

](https://dev.epicgames.com/documentation/fortnite/using-sedan-spawner-devices-in-fortnite-creative)
- [

Sentry Devices

Spawn customized sentries that attack players.

](https://dev.epicgames.com/documentation/fortnite/using-sentry-devices-in-fortnite-creative)
- [

Shopping Cart Spawner Devices

Create shopping cart races for your players.

](https://dev.epicgames.com/documentation/fortnite/usingshoppingcartspawnerdevicesinfortnitecreative)
- [

Side Scroller Controls Devices

The Side Scroller Controls device can be used with camera devices to create side scrolling gameplay.

](https://dev.epicgames.com/documentation/fortnite/using-side-scroller-controls-devices-in-fortnite-creative)
- [

Siege Cannon Devices

Place these in strategic locations for players to use as heavy damage dealers or to make a quick escape.

](https://dev.epicgames.com/documentation/fortnite/using-siege-cannon-devices-in-fortnite-creative)
- [

Signal Remote Manager Devices

Give your players the ability to send signals to devices on your island and make things happen!

](https://dev.epicgames.com/documentation/fortnite/using-signal-remote-manager-devices-in-fortnite-creative)
- [

Skilled Interaction Devices

Raise the bar and create interactable user interfaces for minigames like lockpicking and fishing.

](https://dev.epicgames.com/documentation/fortnite/using-skilled-interaction-devices-in-fortnite-creative)
- [

Skydive Volume Devices

Create zones where players can be launched into the air, or use multiple zones to create unique ways to get around your island.

](https://dev.epicgames.com/documentation/fortnite/using-skydive-volume-devices-in-fortnite-creative)
- [

Skydome Devices

Change your island from bright and sunny, to cloudy, to eerie alien skies or dark and spooky nights.

](https://dev.epicgames.com/documentation/fortnite/using-skydome-devices-in-fortnite-creative)
- [

Slurp Plant Devices

Place a plant pod in the environment that players can hit with a pickaxe to toss healing toward team members.

](https://dev.epicgames.com/documentation/fortnite/using-slurp-plant-devices-in-fortnite-creative)
- [

Sportbike Spawner Devices

Place nimble racing bikes with a Neo-Tokyo theme around your island to give players a speedy, two-person motorcycle they can ride while engaging in combat.

](https://dev.epicgames.com/documentation/fortnite/using-sportbike-spawner-devices-in-fortnite-creative)
- [

Sports Car Spawner Devices

Place a sports car vehicle in your game for your players to drive.

](https://dev.epicgames.com/documentation/fortnite/using-sports-car-spawner-devices-in-fortnite-creative)
- [

Stat Counter Devices

Use the Stat Counter device to manage player statistics.

](https://dev.epicgames.com/documentation/fortnite/using-stat-counter-devices-in-fortnite-creative)
- [

Stat Creator Devices

Create sets of custom data to track and query in-game statistics.

](https://dev.epicgames.com/documentation/fortnite/using-stat-creator-devices-in-fortnite-creative)
- [

Stat Powerup Devices

Use Stat Powerup devices to grant pre-made or custom statistics to players.

](https://dev.epicgames.com/documentation/fortnite/using-stat-powerup-devices-in-fortnite-creative)
- [

Stink Flower Devices

Place a plant pod in the environment that players can hit with a pickaxe to toss a stink-bomb toward enemies.

](https://dev.epicgames.com/documentation/fortnite/using-stink-flower-devices-in-fortnite-creative)
- [

Supply Drop Spawner Devices

Spawn an aerial supply drop to provide players with weapons or supplies.

](https://dev.epicgames.com/documentation/fortnite/using-supply-drop-spawner-devices-in-fortnite-creative)
- [

Surfboard Spawner Devices

Place a Surfboard vehicle in your game for your players to ride.

](https://dev.epicgames.com/documentation/fortnite/using-surfboard-spawner-devices-in-fortnite-creative)
- [

SUV Spawner Devices

Spawn a rugged SUV on your island.

](https://dev.epicgames.com/documentation/fortnite/using-suv-spawner-devices-in-fortnite-creative)
- [

Switch Devices

Use this switch on devices players can turn on or off, or for other interactions.

](https://dev.epicgames.com/documentation/fortnite/using-switch-devices-in-fortnite-creative)
- [

Sword in the Stone Devices

Let a player claim the Infinity Blade to destroy enemies with a single blow!

](https://dev.epicgames.com/documentation/fortnite/using-sword-in-the-stone-devices-in-fortnite-creative)
- [

Tank Spawner Device

Add a mighty tank to your arena for high-powered fun!

](https://dev.epicgames.com/documentation/fortnite/using-tank-spawner-devices-in-fortnite-creative)
- [

Target Dummy Devices

Use target dummies to create a shooting gallery, practice range, or minigames.

](https://dev.epicgames.com/documentation/fortnite/using-target-dummy-devices-in-fortnite-creative)
- [

Target Dummy Track Devices

Use target Dummy Tracks to create a moving target for shooting galleries, practice ranges, or mini-games.

](https://dev.epicgames.com/documentation/fortnite/using-target-dummy-track-devices-in-fortnite-creative)
- [

Taxi Spawner Devices

Place a Taxi vehicle in your game for your players to drive.

](https://dev.epicgames.com/documentation/fortnite/using-taxi-spawner-devices-in-fortnite-creative)
- [

Team Settings and Inventory Devices

Use this device to customize the settings and starting inventory for one or more teams.

](https://dev.epicgames.com/documentation/fortnite/using-team-settings-and-inventory-devices-in-fortnite-creative)
- [

Teleporter Devices

Create a customizable rift that allows players to move instantly between locations.

](https://dev.epicgames.com/documentation/fortnite/using-teleporter-devices-in-fortnite-creative)
- [

Third Person Controls Devices

Use the Third Person Controls device to remap or reconfigure player controls while you are using camera devices.

](https://dev.epicgames.com/documentation/fortnite/using-third-person-controls-devices-in-fortnite-creative)
- [

Timed Objective Devices

When this device is triggered, it starts a countdown. If it reaches the end of the countdown, it sends a message on a specific channel.

](https://dev.epicgames.com/documentation/fortnite/using-timed-objective-devices-in-fortnite-creative)
- [

Timer Devices

Timer Devices can be controlled manually, or integrated with other devices using direct event binding.

](https://dev.epicgames.com/documentation/fortnite/using-timer-devices-in-fortnite-creative)
- [

Tracker Devices

Create and track custom objectives for your players to complete.

](https://dev.epicgames.com/documentation/fortnite/using-tracker-devices-in-fortnite-creative)
- [

Trick Tile Devices

Place a trap device that removes the attached tile when activated.

](https://dev.epicgames.com/documentation/fortnite/using-trick-tile-devices-in-fortnite-creative)
- [

Trigger Devices

This configurable device can be used to relay signals to other devices.

](https://dev.epicgames.com/documentation/fortnite/using-trigger-devices-in-fortnite-creative)
- [

UFO Spawner Devices

Turn your island into Area 51 and race UFOs!

](https://dev.epicgames.com/documentation/fortnite/using-ufo-spawner-devices-in-fortnite-creative)
- [

Vehicle Mod Box Spawner Devices

When players crash their vehicles into this device, the vehicles get better, not worse!

](https://dev.epicgames.com/documentation/fortnite/using-vehicle-mod-box-spawner-devices-in-fortnite-creative)
- [

Vehicle Service Station Devices

If your island has vehicles, use this device to give players a way to repair and refuel them.

](https://dev.epicgames.com/documentation/fortnite/using-vehicle-service-station-devices-in-fortnite-creative)
- [

Vending Machine Devices

Make items available for purchase during games, or give them to players for free!

](https://dev.epicgames.com/documentation/fortnite/using-vending-machine-devices-in-fortnite-creative)
- [

VFX Creator Devices

Create and modify your own customized visual effects.

](https://dev.epicgames.com/documentation/fortnite/using-vfx-creator-devices-in-fortnite-creative)
- [

VFX Spawner Devices

Integrate custom visual effects into your gameplay.

](https://dev.epicgames.com/documentation/fortnite/using-vfx-spawner-devices-in-fortnite-creative)
- [

Video Player Devices

Spice up your gameplay by adding videos!

](https://dev.epicgames.com/documentation/fortnite/using-video-player-devices-in-fortnite-creative)
- [

Visual Effect Powerup Devices

Use Visual Effect Powerups to create a visual effect when your players do something cool.

](https://dev.epicgames.com/documentation/fortnite/using-visual-effect-powerup-devices-in-fortnite-creative)
- [

Volume Devices

Use the Volume to create large areas where events can be triggered upon entering or exiting.

](https://dev.epicgames.com/documentation/fortnite/using-volume-devices-in-fortnite-creative)
- [

Voting Group and Voting Options Devices

Set up a voting system on your island that players can participate in!

](https://dev.epicgames.com/documentation/fortnite/using-voting-group-and-voting-options-devices-in-fortnite)
- [

War Bus Spawner Devices

This rugged and compact War Bus gives your players a moving fortress they can use offensively and defensively.

](https://dev.epicgames.com/documentation/fortnite/using-war-bus-spawner-devices-in-fortnite-creative)
- [

Water Devices

Create bodies of water like lakes, ponds or canals that players can swim and fish in, or drive boats on!

](https://dev.epicgames.com/documentation/fortnite/using-water-devices-in-fortnite-creative)
- [

Weapon Mod Bench Devices

Give your players a fun and easy way to customize moddable weapons.

](https://dev.epicgames.com/documentation/fortnite/using-weapon-mod-bench-devices-in-fortnite-creative)
- [

Wildlife Spawner Devices

Populate your island with animals — some nice and some not so nice — that you can herd, hunt, tame or dodge!

](https://dev.epicgames.com/documentation/fortnite/using-wildlife-spawner-devices-in-fortnite-creative)
- [

Zipline Devices

Use ziplines to give your players fun and interesting ways to traverse the environment on your island.

](https://dev.epicgames.com/documentation/fortnite/using-zipline-devices-in-fortnite-creative)

---

## Creating Gameplay with Devices in Fortnite

**כותרת מקורית:** Creating Gameplay with Devices in Fortnite  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/creating-gameplay-with-devices-in-fortnite  
**מקור קלט:** `06_יסודות_Devices_ואירועים(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `creating-gameplay-with-devices-in-fortnite`

For any game, gameplay is controlled by [game mechanics](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#game-mechanics). Each mechanic covers a specific aspect of the game's functionality. These can range from general rules that define the what a player has to do to win the game ([win conditions](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#win-condition)) to specific things like where a player spawns on the island, how players can move, and what items can be granted to a player and when.

A device is a set of pre-programmed game mechanics in a single package that you can place on an island. Most devices have a visual representation — either as a mesh [asset](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#asset) or as an icon. Some are visible in-game, some are visible only when editing the island, and for some, you can set the visibility on or off for gameplay.

[
](https://dev.epicgames.com/community/api/documentation/image/adb243b9-db08-4f24-afe7-f0761f6ab22d?resizing_type=fit) The device on the left is the Down But Not Out device, and is represented by an icon. The one on the right is the Character device and has a mesh.

### Out of the Box, and Then Some!

Devices add interactivity by detecting player actions, triggering events, managing game states, and creating simple-to-complex interactions within the island.

You can use the default Fortnite devices as they are, or you can expand their functionality by customizing them, either through device options or with Verse.

### The History of Fortnite Devices

Devices were originally designed specifically for making games and other experiences in Fortnite Creative, which launched in December of 2018.

FN Creative provided a [sandbox environment](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#sandbox-game) where developers create and save their own games and share them with friends.

Many of the device mechanics were pulled directly from **Fortnite Battle Royale**, and early developer-made games were simple modes like racing and shooter games.

The number of devices has expanded exponentially since that first launch, along with the sophistication of the devices themselves and the experiences developers can create with them.

### Learn What Different Devices Do

With devices, you can prototype gameplay and modify them to suit your needs. It's worth taking a minute to [see what devices are available](https://dev.epicgames.com/documentation/fortnite/using-devices-in-fortnite) before trying to use pure code to reinvent a functionality that already exists. Using and customizing an existing device can streamline your development workflow and save you hours of programming and testing since the available devices have already been proven to work. And if the device doesn't do everything you want, check the [Verse API Reference](https://dev.epicgames.com/documentation/fortnite/verse-api) to see what functionality you can add with Verse!

Some devices are only available in UEFN. For a list of these and the pages that describe them, see [UEFN-Only Devices](https://dev.epicgames.com/documentation/fortnite/uefnonly-devices-in-fortnite). UEFN-only devices cannot be placed on your island from Creative, but once you have placed them in UEFN, options for most of the devices can be modified in Creative during a [Live Edit](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#live-edit) session.

### Using Device Functions and Events

One of the great features of Fortnite devices is that you can set them up to perform specific functions when they are triggered by [events ](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#event)from other devices.

When one device is [bound ](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#binding)to another device, it can send a signal to the other device. The transmission of this signal is called an **event**. An event triggers one or more devices to do a particular thing or set a particular condition, and that action or condition is called a **function**.

For example, you could set up a **Button **device to trigger a **Customizable Light** to **On **when a player interacts with the button. Once this device is set up, you can copy-paste it to create a duplicate, then change the copied device to turn the light **Off**. You might even be able to customize one device to do both actions as an **On-Off** toggle.

**So much faster than coding from scratch — these built-in functions and events can dramatically speed up your design productivity!**

### Ready for More?

For more on how to find and modify devices in UEFN or Creative, and how to set up event triggers:

- [
*

Getting Started with Devices

Learn how to add and modify devices in Fortnite, and how to use Verse to expand device functionality!

](https://dev.epicgames.com/documentation/fortnite/getting-started-with-devices-in-fortnite)

, see **[Getting Started with Devices](https://dev.epicgames.com/documentation/fortnite/getting-started-with-devices-in-fortnite)**.

If you're looking for some cool inspiration, check out [Device Design Examples](https://dev.epicgames.com/documentation/fortnite/device-design-examples-in-fortnite-creative) for some great ideas on how you can use devices to create fun and unusual game mechanics!

---

## Getting Started with Devices in Fortnite

**כותרת מקורית:** Getting Started with Devices in Fortnite  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/getting-started-with-devices-in-fortnite  
**מקור קלט:** `06_יסודות_Devices_ואירועים(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `getting-started-with-devices-in-fortnite`

Devices are the core building blocks of [game mechanics](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#game-mechanics). The games you can build in Fortnite are vast when you have a clear understanding of the devices and how they work!

 shortcuts to how to find, place, and modify devices, jump to:

-
[Devices in UEFN](https://dev.epicgames.com/documentation/fortnite/getting-started-with-devices-in-fortnite#devices-in-uefn)

-
[Devices in Creative](https://dev.epicgames.com/documentation/fortnite/getting-started-with-devices-in-fortnite)

### General Device Categories
**

The categories below follow the categories laid out in the UEFN Content Browser. Creative uses tags to sort and filter devices that differ from the UEFN categories.

In UEFN, devices fall into one of these categories:

 Category What They Do
!****Experimental**

Devices that are available for testing, but not for publishing. To see this category in the browser, you must first enable the experimental feature from the project settings.

To enable an experimental feature:

-
From the toolbar near the top of the window, click the **Project **dropdown.

-
Select **Project Settings**.

-
Scroll down to the **Experimental Access** section, then toggle the feature you want to enable.

These features can range from devices to island settings. The options also change periodically as features are moved into production readiness and new experimental features are added.

**!Beta**

Still in development, but available for devs to explore and use.

**AI**

Contains characters, enemies, wildlife, and friendly NPCs you can hire. Example devices include Creature Spawner, AI Patrol Path Node, and Creature Manager.

**Audio**

Devices that produce sound or music.

**Audio > Patchwork**

A suite of devices that you can use to create and manipulate music and visuals. Patchwork devices are a subcategory of Audio.

**Environment**

Elements that belong to the world rather than a player character, but that the player can interact with. For example, a player can collect fireflies from a Firefly Spawner and use them against other players to take away health points. Also, fruits from a Healing Cactus device can restore player health.

**Environment > Hazard**

Can deal damage. Examples include Bomb Flower and Explosive devices.

**Gameplay**

General gameplay ingredients that interact with the player. Examples include the Teleporter device — a rift that moves a player instantly to another location on the island, and the Target Dummy device that players can use to practice shooting ranged weapons.

**Item**

Devices that provide items to players or take them away.

**Logic**

Help build game logic. Includes devices like timers, triggers, and trackers.

**Mode**

Devices that support specific game modes. For example, Race Checkpoint and Race Manager devices support racing games.

**Physics**

Emulate the effects of real-world physics, such as gravity and movement.

**Power Up**

Devices that grant power-ups.These usually give buffs like extra damage or health. For example, The Damage Amplifier Powerup device can multiply the damage a player can deal to another player or NPC.

**System**

System devices can be used for things like changing a player's team, class, score, or analytics that let the developer track data. Examples of system devices include the Player Spawner, which determines where on the island a player will spawn or respawn, and the Changing Booth, which lets a player access their locker and change outfits mid-game.

**Trap**

Devices that can be used to trap or damage players or enemy AI.

**In Creative**, the only trap device is the Trick Tile, which destroys any object it is placed on when it's activated. Creative also has traps included in the Content Items category, but these cannot be customized the way a trap device can.

**In UEFN**, there are many more trap devices available in UEFN. Examples include the Environmental Trap - Ice Block, which can cause players to slip and slide on the ice. And the Environmental Trap - Launch Pad, which shoots players up into the air.

**Traversal**

Things that provide movement across an island, but that aren't vehicles. Examples include devices like Zipline or D-Launcher.

**UI**

Devices that communicate information to players, like Beacon devices that indicate locations of things, or Billboard devices that display customized text like onboarding instructions or directions.

Other UI devices can be used for gameplay interactions, like the Skilled Interaction device, that you can use to create button press interactions that vary based on user input, and Conversation devices (UEFN only) for creating interactive dialogs between players and NPCs.

**Vehicle**

Spawns vehicles that range from surfboards to war buses, with a lot in between.

**Vehicle > Gameplay**

Vehicle-related devices that affect gameplay that involves vehicles, like fuel pumps and service stations.

To learn more about a specific device and its modifiable options, see the pages under [Using Devices](https://dev.epicgames.com/documentation/fortnite/using-devices-in-fortnite) or [UEFN-Only Devices](https://dev.epicgames.com/documentation/fortnite/uefnonly-devices-in-fortnite) for those devices only available in UEFN.

### Device Functions and Events

When you place **props **on an island, they are primarily thematic decoration, and are only involved in gameplay in a static (unmoving) way — like building barriers for a parkour-mode game, or creating paths for a maze adventure. Otherwise, props are there primarily to set the **theme **of the island.

Unlike props, which are passive, **devices do things** when they are triggered. The things they do are called **functions**.

When one device sends a **signal **to another device, this is called an **event**. An event triggers one or more devices to **do a specific thing or set a particular condition**, and that action or condition is called a **function**.

 A function can be **triggered **when the device receives a signal from another device **event**. Events can be **instigated **(started) by player actions, time triggers, or other devices.
**

In the image above:

-
A player interacts with a button, which

-
sends a signal to

-
a light source that's set to OFF by default.

-
This triggers an event that

-
turns on the light source.

To make these mechanics work between devices, the device functions and events have to be [bound](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#binding)**.
**

In UEFN**, you can bind functions to events for other devices, but you can't bind events to functions.**
In Creative (Live Edit)**, you can bind functions to events or events to functions.

### Devices in UEFN

In UEFN, Fortnite devices are kept together in a folder named **Fortnite > Devices**. This folder can be accessed either from the **Content Drawer** or a **Content Browser**.
**

If you're coming into UEFN from Unreal Engine (UE), the user interface will be familiar in many ways, but not identical. See [Editor User Interface](https://dev.epicgames.com/documentation/fortnite/getting-to-know-the-user-interface-in-unreal-editor-for-fortnite) for more information.

In UEFN, Fortnite devices are kept together in a folder named Fortnite > Devices**. This folder can be accessed either from the **Content Drawer** or a **Content Browser**.

#### Find and Place a Device

To find an place a device in UEFN:
**
[
](https://dev.epicgames.com/community/api/documentation/image/3532561d-01d2-4f56-9bfe-5d8e97b7bc92?resizing_type=fit) The path to devices is All > Fortnite > Devices. Each folder contains groupings of similar devices. Clicking the folder shows the devices in that group.

-
Open a Content Browser** panel.

-
Find the **Fortnite **folder and click to expand.

-
Click **Devices **to expand.

-
The easiest way to find a device is to use the **search bar**.

-
To browse devices, click a folder to expand it, find the device you want, and drag it into the viewport.

#### Modify Device Options

To customize options for a device:

-
Select the device in your **viewport **or on the **Outliner **panel.

-
View the available options in the **Details **panel.

-
Click **All **to ensure all available options are shown. The other tabs are filters that limit the options that display.

-
Not all devices have the same options available.

-
Some options are nested inside other options.

-
Some options only become available when another option is enabled.

#### Bind Functions to Events

Functions and events are also found on the **Details **panel.

Events are shown for information only, which means you can retrieve/receive or "read" the value (event in this case), but cannot set, alter, or modify it. In UEFN, you can only bind a function to an event.

**

In UEFN, binding functions to events involves selecting array elements**. In UEFN, an **element **is a single component in a group of components. An **array **is a container for storing similar elements. When setting up your functions, you can select the array element you want to bind the function to.

-
With a device selected, scroll down through the **Details **panel, then click the **User Options - Functions** to expand it.
**

-
Click the function you want to modify.

The list of functions varies based on the device you've selected.

-
From the list of available functions, click the + (plus)** icon to add an **array element**. The array shows the functions available for that device.

-
Click the first dropdown, and select a device. If you have a lot of devices, you can use the search bar to find one more easily.

-
Click the second dropdown, and select the event you want to bind to this function.

### Expand Device Functionality with the Verse API Reference

An application programming interface, or API, is a set of program instructions that can be used or modified in an existing software application. The [Verse API Reference](https://dev.epicgames.com/documentation/fortnite/verse-api) is an API library that provides ways to customize devices in UEFN by using Verse.

Extending a device's functionality using Verse can be more efficient than trying to program gameplay in Verse entirely.

Every device in UEFN has a corresponding Verse API that you can use to add or change device features beyond the default option modifications available in UEFN.

Not all devices have the same degree of customization available in the API. The customization available varies based on how much of the device code is accessible (exposed) in the API.

#### API Terms

There are a few basic concepts that can help you make best use of the Verse API Reference.
**

The definitions below are specific to Verse, and may have slightly different meanings in other areas of Fortnite.

 Term What It Means
module**

An atomic unit of code that can be reused. You can import a module into a Verse file in UEFN, and modify that code to customize it without breaking any dependencies to other units of code.

**class**

In Verse, a class is a template for creating objects that have similar properties and behaviors, defined by fields (variables) and methods (functions). Each device is a class.

**hierarchy**

Levels (hierarchies) of rank, importance, or control. Common hierarchical relationships are parent/child or superclass/subclass. Objects lower in the hierarchy inherit properties and methods from objects above it.

**inheritance**

In Verse, you can create a new class that extends an existing class definition by adding or modifying properties. This is often called subclassing or inheritance, because one class inherits definitions from the other class.

**variable**

A value that can be changed during runtime.

**function**

The code that provides instructions for performing an action.

**member**

In Verse, a member is a variable or function that is part of a composite data structure, such as a class or module. Member variables are sometimes called fields, and member functions are sometimes called methods.

**Verse-authored device**

A device for use in UEFN that is programmed directly using Verse.

**struct**

A struct (short for structure), is a user-defined type that allows you to group several related variables together. Several structs are available in the API. A common use of structs is for error messages, where message text and relevant data from the failed function are grouped

#### Find a Device API
**

The device categories do not match the categories in the UEFN Content Browser. The device names also do not always match the name of the device in UEFN or Creative.

To find the API for a device in the Table of Contents:

-
Go to the [Verse API Reference](https://dev.epicgames.com/documentation/fortnite/verse-api).

-
Find the Fortnite.com module**, then the [Devices module](https://dev.epicgames.com/documentation/en-us/fortnite/verse-api/fortnitedotcom/devices) underneath it.

You can also search for the device by name or key words in the search bar.

For some good examples of how you can use the Verse API to expand device functionality, see the [Spice Up the Gameplay with Verse](https://dev.epicgames.com/documentation/fortnite/first-island-05-spice-up-the-gameplay-with-verse-in-fortnite) page of the [Build Your First Island in Fortnite](https://dev.epicgames.com/documentation/fortnite/build-your-first-island-in-fortnite) tutorial.

To learn more about Verse, see the Verse Language Reference.

#### How the API Reference Pages Work

When you drill all the way down in the API to a device page, the important information to look for is:

-
**Verse using statement: **This is the statement you need to include in your Verse device to make use of the given module. For devices, it’s always:

using { /Fortnite.com/Devices }

-
**Inheritance hierarchy: **This is a parent-child structure where child classes (subclasses) inherit variables and functions from the classes above it in the hierarchical structure.

**
[
](https://dev.epicgames.com/community/api/documentation/image/e478b84f-e9e4-4558-a41d-b3aabfeb4517?resizing_type=fit) In this image, health_powerup_device_ inherits from powerup_device, which inherits from creative_device_base, and so on.

To follow how a typical API page is organized, see the [health_powerup_device_class](https://dev.epicgames.com/documentation/en-us/fortnite/verse-api/fortnitedotcom/devices/health_powerup_device) page.

[
](https://dev.epicgames.com/community/api/documentation/image/e07e3cb8-ae47-436e-b998-b0206546aa86?resizing_type=fit) The menu on the right provides quick navigation to information. The information on the left under each topic gives the name and description.

The topics covered for each device are:

-
Inheritance Hierarchy:** The device hierarchal structure.

-
**Members:** Broken down by Data and Functions.

-
**Data: **Includes variables and events that you can use to trigger behavior — for example, ItemPickedUpEvent is based on when a player picks up an item, which triggers something else to occur.

-
**Functions: ** All of the device functions that are exposed by the API.

#### Make Your Own Device with Verse

In UEFN, you can also create your own [Verse-authored device](https://dev.epicgames.com/documentation/fortnite/verse-glossary#verse-authored-device) to create custom game mechanics from the ground up to address the unique requirements of your island. This can range from something as simple as a counter to track player eliminations to something complex like tying several devices together to leverage their combined functionalities.

To learn more about how to create your own device with Verse, see [Modify and Run Your First Verse Program](https://dev.epicgames.com/documentation/fortnite/modify-and-run-your-first-verse-program-in-unreal-editor-for-fortnite).

### Devices in Creative

The devices in Creative are mostly the same as those available in UEFN, but the way you find, place, and modify them is very different.

#### Find a Device

To find a device:

-
From [Create mode](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#create-mode), press the **M **key, then click **Content**.

-
Select the **Devices **category on the left. From here, you can browse the entire inventory of devices, or narrow your search.
**

-
Narrow your search (optional):

Use the search bar to search by device name.

-
Filter devices in the right panel with tags.

-
Click the Sort **button to sort the results alphabetically.

#### Place a Device

There are different ways you can place a device on your island.
**

-
Select the device then:

Click the Quick Bar** tile,

-
Press the corresponding tile number, or

-
Drag the device on to the tile.

The device should display on the Quick Bar when you return to your island.
-
Click **Place Now**. This places the device directly onto your island, and returns you to the island.

-
Click **Equip **to add it to the next available tile on your Quick Bar.

-
Click Exit to return to your island.

For more on how to place, resize, copy, and delete devices (plus a whole lot more!), see [Hotkeys and Keybinding Shortcuts](https://dev.epicgames.com/documentation/fortnite/hotkey-and-keybinding-shortcuts-in-fortnite-creative). The device should display on the Quick Bar when you return to your island.Click Equip to add it to the next available tile on your Quick Bar.Click Exit to return to your island.

#### Modify Device Options

Because Creative can be used on multiple gaming devices, from PCs to consoles and handheld devices, the UI is more visual — and larger — compared to UEFN.

To customize device options in Creative, approach a device and press **E** to open the **Customize **panel.
**

The panel has tabs **that you can use to navigate between the different options:
**

 Options Tab Name Description
1**

Basic Options

These are the most common options that you can customize.

**2**

All Options

This tab shows options available for the device.

**3**

Modified Options

This shows the modifications you’ve made.

**4**

Functions

Use this tab to bind a function to an event.

**5**

Events

Use this tab to bind an event to a function.

**6**

Search

Some devices have a lot of available options. If you know the option name, you can use the Search tab to find a specific option.

#### Bind Functions and Events

In Creative, you can bind functions to events or events to functions.

-
With the **Customize **device panel open, click the **Functions **tab.

-
Select a function then click **Add**.
**

-
Click Select Device** and select from the Device dropdown menu.

-
Click **Select Event** to bind the device to an event that triggers the function for the device.

If more than one device or event triggers a function, click the Add button to add a line and repeat these steps.

You can also bind devices from the **Events **tab.

### Tips for Customizing Devices in Creative

Every device has its own specific settings that you can modify, but there are a few useful features common to most devices.

Click the **settings (gear) icon** at the bottom of the panel to open a settings menu.

#### Rename

Give the device a **custom name** or **reset to the default** name.

 You can also rename the device at the top of the Customize panel.

Giving a device a unique name is helpful if you are using multiple versions of the same device. For example, if you have multiple Wildlife Spawner devices, naming each one based on the type of wildlife it spawns makes it easier to find the right device if you want to change your customizations later.

Renaming devices is also helpful when you use the [Event Browser](https://dev.epicgames.com/documentation/fortnite/event-browser-in-fortnite-creative).

#### Reset All

Most devices have multiple settings that you can customize. This resets all of the options back to default. This also resets the device name if you've changed it.

#### Reset Properties

This resets any option values back to the defaults, but does not change the device name.

#### Reset Functions

This only resets any functions you've defined for a device.

#### Reset Events

This only resets any events you've defined for a device.

The resets are great for when you want to start over on device customization, or if you want to make two of the same device with very different settings.

---

## Getting Started with Direct Event Binding in Fortnite Creative

**כותרת מקורית:** Getting Started with Direct Event Binding in Fortnite Creative  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/getting-started-with-direct-event-binding-in-fortnite-creative  
**מקור קלט:** `06_יסודות_Devices_ואירועים(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `getting-started-with-direct-event-binding-in-fortnite-creative`

### Why Device Communication is Changing

Direct event binding will expand the possibilities for what you can accomplish in Creative. With direct event binding, devices can communicate directly. It makes your workflow more intuitive, giving you the freedom to really pursue your design ideas. Switching to this system is the next step in creating game mechanics that are more complex and diverse.

The direct event binding system eliminates limitations inherent in the channel communication system. You no longer have to worry about reaching the maximum channel limit. Because the devices communicate directly with event binding, you don't have to preplan your channel allocation when designing an island. When you copy-paste devices, you no longer need to edit them to change the channel assignments — the events and functions set in the original carry over to the copies.

### Introducing Events and Functions

Instead of transmitting and receiving signals, devices use **events** and **functions**. When a device activates, or a player performs an action, that's an example of an **event**. Events trigger other devices to do a particular thing or set a particular condition, and that action or condition is a **function**. You bind an event in one device to a function in another device. For the most part, former transmitter options are now events, and former receiver options are now functions.

### How Direct Event Binding Works

Instead of assigning channels, direct event binding uses device names to specify events and functions that occur between multiple devices. Devices are automatically assigned a unique identifier, but these are just a string of letters and numbers. It will be important to rename your devices with meaningful and descriptive names.

Below is an illustration comparing the channel system to the direct event binding system, which can help you see how they are similar and how they are different.

### Converting Your Existing Islands

Direct event binding is currently an opt-in system, although eventually it will be the default. When you want to convert an existing island to the new system, you should make a copy of the island and test the conversion on that copy first.

Once you have converted an island from the channel system to the direct event binding system, it cannot be switched back to the channel system! Resetting the island will not switch it back to the channel system.

To switch an existing island to the new system, open **My Island** and click the **Tools** tab. Locate the **Event System** setting and click **Convert**.

This automatic conversion will assign unique IDs (a random string of letters and numbers) to any unnamed devices. Devices that were connected in the channel system will automatically be connected with events and functions in the conversion process.

When you open a device's **Customize** panel to view the options, you will see an **Events** tab and a **Functions** tab instead of the **Channels** tab. This is where you will find the connections between devices on your island.

### Additional Advantages of Direct Event Binding

The direct event binding system dramatically speeds up your workflow for building islands, and helps you make important changes all at once.

As an example, let's say you have set up a Button device to turn on a Customizable Light when a player interacts with the button. On the Events tab, you have selected the event **On Interact Send Event To**. Under the event, you have selected the **Customizable Light** device, and next to the device you have selected **Turn On** as the function.

If you want to add another Button to turn off the light, you can just copy and paste the first Button device, then go to the **Events** tab and click **Turn On** to open the menu. Select **Turn Off** from the list, and you're done! You can then rename the two Button devices to **Light On** and **Light Off** to make it clear which is which.

With the channel system, you can copy-paste devices — but you'll have to edit each one to different channel pairings. If you have highly complex game mechanics that involve multiple devices, this can take enormous amounts of time. And if you get things mixed up, it takes even more time to fix whatever is broken.

But with direct event binding, you have fewer things to change, meaning your work goes faster. And it's a lot easier to create large interconnected groups of devices, meaning your games can make use of more sophisticated game mechanics. And with no channels, there's no maximum number of channels to keep in mind and work around. You can copy and paste one device or a whole group without concerns for channel limitations.

### What's Next

Check out the [official Fortnite blog](https://www.epicgames.com/fortnite/en-US/news/introducing-direct-event-binding-for-creating-fortnite-islands) for a Direct Event Binding FAQ. Share your creations with us on Twitter by tagging us [@FNCreate](https://twitter.com/FNCreate)!

---

## Using Attribute Evaluator Devices in Fortnite Creative

**כותרת מקורית:** Using Attribute Evaluator Devices in Fortnite Creative  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/using-attribute-evaluator-devices-in-fortnite-creative  
**מקור קלט:** `07A_קלט_טריגרים_תנאים_והחלטות(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `using-attribute-evaluator-devices-in-fortnite-creative`

**
The **Attribute Evaluator** only works with signals received from other devices. It acts as [branching logic](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary), and checks whether the player that sent the signal passes all of the tests that are set up for this trigger. Then the [trigger](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) sends a signal on either a success channel or a failure channel. With this trigger, you can test whether a player has reached a specific condition, and determine what happens when that occurs.

The attribute evaluator checks against the stats of the player at the point it is activated. If it receives a signal from an event that changes one of the player's stats (for example, if it receives a signal from the Elimination Manager that a player has just eliminated an enemy), the player's stats might not have been updated from that event. See [Loo Roll Rush](https://dev.epicgames.com/documentation/fortnite/loo-roll-rush-in-fortnite-creative) for an example of this problem.

 For help on how to find the Attribute Evaluator** device, see [Using Devices](https://dev.epicgames.com/documentation/en-us/fortnite-creative/using-devices-in-fortnite-creative).

### Device Options

You can configure this device with the following options.
**

Default values are in **bold**.

**אפשרויות, ערכים ותיאורים:**

##### Activating Team**

- **Value / Values:** **Any**, Pick or enter a number.
- **Description:** Determines which team can activate the device. This replaces the Affects Team option.

##### Invert Team Selection

- **Value / Values:** **Off**, On
- **Description:** If set to **On**, the device will count all teams except the selected team.

##### Activating Class

- **Value / Values:** **Any**, Pick or enter a number
- **Description:** Determines which class can activate the device. This replaces the Affects Class option.

##### Invert Class Selection

- **Value / Values:** **Off**, On
- **Description:** If set to **On**, the device will count all but the selected class.

##### Min Player Eliminations

- **Value / Values:** **0**, Pick or enter a number
- **Description:** Set the minimum amount of eliminations the instigating player must have to pass this check.

##### Tracked Stat

- **Value / Values:** **Score**, Select a stat
- **Description:** Determines which statistic this device will track for the **Team Stat** and **Player Stat** options.

##### Min Player Stat

- **Value / Values:** **0**, Pick or enter a number
- **Description:** Sets the minimum amount of score the instigating player must have to pass this check.

##### Min Team Stat

- **Value / Values:** **0**, Pick or enter a number
- **Description:** Sets the minimum amount of score the instigating player's team must have to pass this check.

##### Enabled at Game Start

- **Value / Values:** **On**, Off
- **Description:** Determines whether the device is enabled when the game starts.

##### Times Can Trigger

- **Value / Values:** **Infinite**, Pick a number
- **Description:** Determines how many times the device can be triggered before it is disabled.

##### Trigger Delay

- **Value / Values:** **Instant**, Pick or enter a number
- **Description:** Determines the length of time the device will wait between being triggered and sending a signal. This option replaces the Delay option.

##### Reset Delay

- **Value / Values:** **None**, Pick an amount of time
- **Description:** After the device is activated, it is disabled for this amount of time before being usable again.

##### Visible In Game

- **Value / Values:** **On**, Off
- **Description:** Determines whether the device is visible during the game.

##### Trigger SFX

- **Value / Values:** **Enabled**, Disabled
- **Description:** Determines if audio effects are played when the device is activated.

##### Trigger VFX

- **Value / Values:** **On**, Off
- **Description:** Determines whether visual effects are displayed when the device is activated.

##### Transmit Every X Trigger

- **Value / Values:** **1**, Pick or enter a number
- **Description:** Sets the device to only send a signal after being triggered the specific number of times.

### Direct Event Binding

**Direct event binding** allows devices to communicate directly, which makes your workflow more intuitive, and gives you more freedom to focus on your design ideas.

Below are the [functions](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) and [events](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) for this device.

#### Functions

A [**function**](https://dev.epicgames.com/documentation/en-us/fortnite-creative/fortnite-creative-glossary#function) listens for an event on a device then performs an action.

-
For any function, click the option, then Select Device to access and select from the Device dropdown menu.

-
Once you've selected a device, click Select Event and select the event that triggers this function.

-
If more than one device or event triggers a function, press the Add button to add a line and repeat these steps.

**אפשרויות ותיאורים:**

##### Enable When Receiving From

This function enables the device when an event occurs. Select the device and event that will enable the device. If more than one device or event can enable the device, you can click the **Add** button for this option, which adds another line.

##### Disable When Receiving From

This function disables the device when an event occurs. Select the device and event that will disable the device. If more than one device or event can disable the device, you can click the **Add** button for this option, which adds another line.

##### Reset Times Triggered When Receiving From

This function resets the number of times the device has been activated (to reset the **Transmit Every X Triggers** and **Times Can Trigger** options).

##### Evaluate Player When Receiving From

This function evaluates players against the list of attributes when receiving an event.

#### Events

Direct event binding uses events as transmitters. An event tells another device to perform a function.

-
For any event option, click the option, then Select Device to access and select from the Device dropdown menu.

-
Once you've selected a device, click Select Function to bind the event to a function for that device.

-
If more than one function is triggered by the event, press the Add button and repeat.

**אפשרויות ותיאורים:**

##### On Pass Send Event To

When a player passes a check, the device sends an event to the selected device.

##### On Fail Send Event To

If a player fails a check, the device send an event to the selected device.

### Gameplay Examples Using Attribute Evaluators

-
[Tug of War](https://dev.epicgames.com/documentation/fortnite/tug-of-war-in-fortnite-creative)

-
[Loo Roll Rush](https://dev.epicgames.com/documentation/fortnite/loo-roll-rush-in-fortnite-creative)

-
[Top Scorer In Class](https://dev.epicgames.com/documentation/fortnite/top-scorer-in-class-in-fortnite-creative)

---

## Using Button Devices in Fortnite Creative

**כותרת מקורית:** Using Button Devices in Fortnite Creative  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/using-button-devices-in-fortnite-creative  
**מקור קלט:** `07A_קלט_טריגרים_תנאים_והחלטות(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `using-button-devices-in-fortnite-creative`

You can use a [Button](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) device to activate other [devices](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary). In its [default](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) state, the button does nothing, but when configured to work with another device, the button can activate another [device](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) when a player interacts with it.

For help on how to find the Button device, see [Using Devices](https://dev.epicgames.com/documentation/fortnite/using-devices-in-fortnite).

**Looking for more inspiration?** See [**Button Device Design Examples**](https://dev.epicgames.com/documentation/fortnite/button-device-design-examples-in-fortnite-creative) to kick off your imagination!

If you're using multiple copies of a device on an island, it can be useful to [rename](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) them. Choosing names that relate to a device's purpose makes it easier to remember what each one does, and easier to find a specific device when using the [Event Browser](https://dev.epicgames.com/documentation/fortnite/event-browser-in-fortnite-creative).

### Device Options

To pair a button with another device, you need to specify the [event binding](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) for the player interaction with the button. See [Direct Event Binding](https://dev.epicgames.com/documentation/fortnite/using-button-devices-in-fortnite-creative) for the settings.

You can configure this device with the following options.

Default values are in **bold**.

**אפשרויות, ערכים ותיאורים:**

##### Interact Time

- **Value / Values:** **Instant**, Pick an amount of time
- **Description:** Determines the length of interaction required to activate the device.

##### Activating Team

- **Value / Values:** **Any**, Pick a team number
- **Description:** This indicates which team can interact with the button. Use the arrows to choose a team, or click in the field to type in a team number.

##### Invert Team Selection

- **Value / Values:** On, **Off**
- **Description:** If set, the device can by used by all but the selected team.

##### Allowed Class

- **Value / Values:** **Any**, No Class, Pick a class
- **Description:** Determines what class can interact with the device. Use the arrows to choose a class, or click in the field to type in a class number.

##### Invert Class Selection

- **Value / Values:** On, **Off**
- **Description:** If set, the device can by used by all but the selected class.

##### Times Can Trigger

- **Value / Values:** **Infinite**, Pick a number
- **Description:** The number of times the button can be [triggered](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) before it's [disabled](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary). Use the arrows to choose, or click in the field to type in a number.

##### Delay

- **Value / Values:** **Instant**, Pick an amount of seconds
- **Description:** How long the button waits to transmit its signal after it's triggered. Use the arrows to choose, or click in the field to choose an amount.

##### Reset Delay

- **Value / Values:** **Instant**, Pick an amount of seconds
- **Description:** This is the amount of time where the button can't be triggered after it transmits its signal. Use the arrows to choose, or click in the field to choose an amount.

##### Trigger Sound

- **Value / Values:** **Enabled**, Disabled
- **Description:** The sound that plays when the button is triggered.

##### Enabled at Game Start

- **Value / Values:** **Enabled**, Disabled
- **Description:** Whether the button is automatically enabled when the game starts.

##### Interaction Text

- **Value / Values:** Enter text
- **Description:** This text displays when the player is close to the button and looks at it. The text field is limited to 64 characters.

##### Visible During Game

- **Value / Values:** **Yes**, No
- **Description:** If you want the button to be generally visible during the game, choose Yes. You can also choose to make the button invisible and attach it to a [prop](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary), so it looks like the prop activates another device. In that case, choose No.

##### Interaction Radius

- **Value / Values:** **Button**, Pick a size
- **Description:** If you choose to make the button visible in the game, choose **Button**. If you choose not to make the button visible, you need to indicate how close the player must be to interact with the prop your button is attached to. Use the arrows to choose a distance, or click in the field to type in a number.

### Direct Event Binding

Following are the [direct event binding](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) options for this device.

#### Functions

A [function](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) listens for an event on a device then performs an action.

-
For any function, click the option, then Select Device to access and select from the Device dropdown menu.

-
Once you've selected a device, click Select Event to bind the device to an event that will trigger the function for the device.

-
If more than one device or event triggers a function, press the Add button to add a line and repeat these steps.

**אפשרויות ותיאורים:**

##### Enable When Receiving From

Enable the button.

##### Disable When Receveing From

Disable the button.

#### Events

Direct event binding uses events as transmitters. An event tells another device to perform a function.

-
For any event option, click the **option**, then **Select Device** to access and select from the **Device dropdown menu**.

-
Once you've selected a device, click **Select Function** to bind the timer to a function for that device.

-
If more than one function is triggered by the event, press the **Add** button and repeat.

**אפשרויות ותיאורים:**

##### On Interact Send Event To

Sends an event to a linked device when a player interacts with the button.

### Gameplay Examples Using Buttons

-
[Dungeon Crawler](https://dev.epicgames.com/documentation/fortnite/dungeon-crawler-gameplay-example-in-fortnite-creative)

-
[Shooting Gallery](https://dev.epicgames.com/documentation/fortnite/shooting-gallery-in-fortnite-creative)

-
[Spawner123](https://dev.epicgames.com/documentation/fortnite/spawner-123-in-fortnite-creative)

---

## Using Channel Devices in Fortnite Creative

**כותרת מקורית:** Using Channel Devices in Fortnite Creative  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/using-channel-devices-in-fortnite-creative  
**מקור קלט:** `07A_קלט_טריגרים_תנאים_והחלטות(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `using-channel-devices-in-fortnite-creative`

The **Channel** device is a simple relay, with only one [event](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) and one [function](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary). It works much like a [Trigger device](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary), but it is easier to connect multiple devices using one Channel device.

When you have complex connections between many devices on your island, using a Channel device instead of multiple Triggers could simplify your setup.

Here are some ways you can use the Channel device:

-
Streamline connections between one group of many devices and another group of many devices.

-
Swap different devices connected to the Channel device to test different game mechanics for your island, or test multiple player actions.

-
Replicate the previous [channel](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) system instead of using [direct event binding](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary).

To find the Channel device, go to the **Creative inventory** and select the **Devices** tab. From there, you can search or browse for the device. For more information on finding devices see [Using Devices](https://dev.epicgames.com/documentation/fortnite/using-devices-in-fortnite).

If you're using multiple copies of a device on an island, it can be helpful to [rename](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) them. You can choose names that relate to each device's purpose, so it's easier to remember what each one does.

### Device Options

You can configure this device with the following options.

Default values are **bold**.

**אפשרויות, ערכים ותיאורים:**

##### Show Debug Message

- **Value / Values:** **Off**, On
- **Description:** Shows a debug message for non-published islands when the device is channeling an event. The debug message will display in the message feed.

##### Broadcast Global Event Name

- **Value / Values:** Enter text up to 150 characters
- **Description:** An event name entered here is broadcast globally to all other channel devices. Any devices listening for and receiving this event name will be activated. Text entered is not case sensitive.

##### Listen for Global Event Name

- **Value / Values:** Enter text up to 150 characters
- **Description:** The event name entered here will be listened for by this device. When received, the device will send it's event. Text entered is not case sensitive.

### Direct Event Binding

Following are the [direct event binding](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) options for this device.

#### Functions

A [function](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) listens for an event on a device then performs an action.

-
For any function, click the **option**, then **Select Device** to access and select from the Device dropdown menu.

-
Once you've selected a device, click **Select Event** to bind the device to an event that will trigger the function for the device.

-
If more than one device or event triggers a function, press the **Add** button to add a line and repeat these steps.

**אפשרויות ותיאורים:**

##### Transmit When Receiving From

When the selected event occurs, this will activate Broadcast Global Event.

#### Events

Direct event binding uses events as transmitters. An event tells another device to perform a function.

-
For any event option, click the **option**, then **Select Device** to access and select from the **Device dropdown menu**.

-
Once you've selected a device, click **Select Function** to bind the timer to a function for that device.

-
If more than one function is triggered by the event, press the **Add** button and repeat.

**אפשרויות ותיאורים:**

##### On Received Transmit

Broadcasts an event when the Broadcast Global Event function is received.

---

## Using Conditional Button Devices in Fortnite Creative

**כותרת מקורית:** Using Conditional Button Devices in Fortnite Creative  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/using-conditional-button-devices-in-fortnite-creative  
**מקור קלט:** `07A_קלט_טריגרים_תנאים_והחלטות(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `using-conditional-button-devices-in-fortnite-creative`

A **Conditional Button** is a [Button device](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) that a player can only activate when carrying specific items. Unlike the regular Button device, the Conditional Button requires the player to possess a specific item or number of items to activate it. Without the specified item, the Conditional Button does not [trigger](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary).

To [register](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) an item to the Conditional Button, drop the item onto the device once the device has been [placed](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary).

For more on how to find this device, see [Using Devices](https://dev.epicgames.com/documentation/fortnite/using-devices-in-fortnite).

ooking for some fun ideas on how to use this device? See [Conditional Button Device Design Examples](https://dev.epicgames.com/documentation/fortnite/conditional-button-device-design-examples-in-fortnite-creative) for inspiration!

### Contextual Filtering

Some devices are affected by a feature called **contextual filtering**. This feature hides or displays options depending on the values selected for certain related options. This reduces clutter in the Customize panel and makes options easier to manage and navigate. To help identify them, values that trigger contextual filtering are in *italic*.

All options are listed, including those affected by contextual filtering; if they are hidden or displayed based on a specific option's value, there will be a note about it in the Description field for that option.

### Device Options

In its [default](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) state, the Conditional Button does nothing until you drop items onto the device to register them. You will also need to specify an event for the device that triggers another device's function when a player interacts with the button.
**

Default values are **bold**. Values that trigger contextual filtering are *italic*.

You can configure this device with the following options.

**אפשרויות, ערכים ותיאורים:**

##### Activating Team

- **Value / Values:** **Any**, Pick a team
- **Description:** Determines which team can activate the device.

##### Allowed Class

- **Value / Values:** No Class, **Any**, Pick a class
- **Description:** Determines which [class](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) can activate the device.

##### Can Be Used By

- **Value / Values:** **Owning Team**, Other Teams, All
- **Description:** Determines which teams can use the device.

##### Allow Interaction

- **Value / Values:** **On**, Off
- **Description:** Determines of players can interact directly with the device.

##### Interact Time

- **Value / Values:** **Instant**, Do Not Interact, Pick a time
- **Description:** Determines the length of time a player must hold down the interaction control to activate the device.

##### Reset Delay

- **Value / Values:** **Instant**, None, Pick a time
- **Description:** Sets the amount of time the device must wait after sending a signal, before the device can be triggered again.

##### Color Type

- **Value / Values:** ***Direct Color***, Team Color
- **Description:** When **Direct Color** is selected, a color can be selected in the next option, **Direct Color**. If you select **Team Color**, the Direct Color option goes away, and the default team color will be used.

##### Direct Color

- **Value / Values:** **White**, Team Color, Various Colors
- **Description:** Changes the color of the device to help players tell one device from another.

##### Use Color For Hologram

- **Value / Values:** Yes, **No**
- **Description:** Sets the hologram to display the same color as the device when it can be interacted with. Invalid interactions will show the color red.

##### Interact Text

- **Value / Values:** Enter Text
- **Description:** Enter the text that appears when players approach the device. Limit is 150 characters.

##### Missing Items Text

- **Value / Values:** Enter Text
- **Description:** Enter the text that shows when requirements are not met. Limit is 150 characters.

##### Show Item Rarity on Missing Item List**

- **Value / Values:** On, **Off**
- **Description:** Determines whether to display the item's rarity to the player or not if they are missing resources.

##### Display Main Icon

- **Value / Values:** **Exclamation**, Select an icon
- **Description:** Shows the chosen icon on the window and base hologram.

##### Use Alt Display Icon

- **Value / Values:** **Off**, *On*
- **Description:** Shows the chosen icon on the "Action" hologram. If you choose **On**, it uses the icon defined in the **Alt Display Main Icon** option below.

##### Alt Display Icon

- **Value / Values:** **Default**, Select an icon
- **Description:** Shows the chosen icon on the "Action" hologram. If you choose **Default**, it uses the icon defined in the **Display Main Icon** option.

##### Toggle Icon on Use

- **Value / Values:** Yes, **No**
- **Description:** Each icon has an alternate version which can be displayed when the button is successfully activated. Use this to choose whether or not to switch to the alternate icon on activation.

##### Disable After Use

- **Value / Values:** Yes, **No**
- **Description:** Sets the device to become disabled after successful activation. The device can be reset or re-enabled using receivers.

##### Remain Unlocked After Activation

- **Value / Values:** On, **Off**
- **Description:** Allows other players to interact without needing keys after activation. You will need to reset the device using the **Reset When Receiving From** option in order to lock the device again.

##### Show Key Item

- **Value / Values:** **Only Key**, Key And Icon, Unknown Key, Only Icon, Unknown Key and Icon
- **Description:** Determines whether the device displays a hologram of the item type players need to unlock it.

##### Number of Key Item Slots

- **Value / Values:** **1**, 2, 3
- **Description:** Sets the number of key items the device requires. Hit the device with your pickaxe in **Create mode** to select an item slot.

##### Key Items Required

- **Value / Values:** **Use Stack Size**, Pick a number
- **Description:** Sets the quantity of the key item required in Slot 1 to activate the button.

##### Second Key Items Required

- **Value / Values:** **Use Stack Size**, Pick a number
- **Description:** Sets the quantity of the key item required in Slot 2 to activate the button.

##### Third Key Items Required

- **Value / Values:** **Use Stack Size**, Pick a number
- **Description:** Sets the quantity of the key item required in Slot 3 to activate the button.

##### Consume Key Items

- **Value / Values:** **On**, Off
- **Description:** Determines whether key items are removed from inventory when the button is pressed.

##### All Key Items Required at Once

- **Value / Values:** **On**, Off
- **Description:** Determines whether the full quantity of key items must be in the player's inventory at once, or whether they can be delivered in batches. This requires that **Consume Key Items** be set to **On**.

##### Require Holding Item

- **Value / Values:** **Off**, On
- **Description:** Determines if the player must be holding a key item in order to interact with the button. Requires that at least one of the key items be an item that can be held by a player.

##### Enabled at Game Start

- **Value / Values:** **On**, Off
- **Description:** Determines whether the device is enabled when the game starts. Disabled devices ignore all events except being Enabled.

##### Visible During Game

- **Value / Values:** **Yes**, No, Hologram Only
- **Description:** Determines whether the device will be visible during the game.

##### Interaction Radius

- **Value / Values:** **Button**, Pick a Radius
- **Description:** Allows players to interact by looking at any point within a radius of the specified size, rather than looking directly at the button.

##### Show Keycard Direction

- **Value / Values:** **Yes**, No
- **Description:** Shows the direction to this device if it is the closest and requires the keycard held.

##### Activated by Sequencers

- **Value / Values:** **On**, Off
- **Description:** Determines whether the trigger is activated when it is touched by a Sequencer or RNG Device pulse.

##### Add Consumed Items to Score

- **Value / Values:** On, **Off**
- **Description:** When a player interacts with the button, if the button consumes the key item it is added to the Player or Team's Score.

##### Score On Key Item 1 Consumed

- **Value / Values:** **0**, Pick an amount
- **Description:** If the Add Consumed Items to Score option is set to On, this determines the score amount granted to the Player or Team when Key Item 1 is consumed.

##### Score On Key Item 2 Consumed

- **Value / Values:** **0**, Pick an amount
- **Description:** If the Add Consumed Items to Score option is set to On, this determines the score amount granted to the Player or Team when Key Item 2 is consumed.

##### Score On Key Item 3 Consumed

- **Value / Values:** **0**, Pick an amount
- **Description:** If the **Add Consumed Items to Score** option is set to **On**, this determines the score amount granted to the Player or Team when Key Item 3 is consumed.

##### Invalid Team/Class Text

- **Value / Values:** Enter text in field
- **Description:** Enter the text that shows when requirements are not met. Limit is 150 characters.

### Direct Event Binding

Following are the [direct event binding](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) options for this device.

#### Functions

A [function](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) listens for an event on a device then performs an action.

-
For any function, click the **option**, then **Select Device** to access and select from the Device dropdown menu.

-
Once you've selected a device, click **Select Event** to bind the device to an event that will trigger the function for the device.

-
If more than one device or event triggers a function, click the **Add** button to add a line and repeat these steps.

**אפשרויות ותיאורים:**

##### Enable When Receiving From

This function enables the conditional button when an event occurs.

##### Disable When Receiving From

This function disables the conditional button when an event occurs.

##### Reset When Receieing From

This function resets the conditional button when an event occurs.

##### Activate When Receiving From

This function activates the conditional button when an event occurs.

##### Toggle When Receiving From

This function toggles the conditional button's state when an event occurs.

#### Events

Sends an event to a linked device when a player interacts with the button.
Direct event binding uses events as transmitters. An event tells another device to perform a function.

-
For any event option, click the **option**, then **Select Device** to access and select from the Device dropdown menu.

-
Once you've selected a device, click **Select Function** to bind the timer to a function for that device.

-
If more than one function is triggered by the event, click the **Add** button to add a line and repeat these steps.

**אפשרויות ותיאורים:**

##### On Activate Send Event To

When the device activates, it sends an event to the selected device, which triggers the selected function.

##### Not Enough Items Send Event To

When the player does not have enough items for the conditional button, it sends an event to the selected device, which triggers the selected function.

---

## Using Input Trigger Devices in Fortnite Creative

**כותרת מקורית:** Using Input Trigger Devices in Fortnite Creative  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/using-input-trigger-devices-in-fortnite-creative  
**מקור קלט:** `07A_קלט_טריגרים_תנאים_והחלטות(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `using-input-trigger-devices-in-fortnite-creative`

**
The **Input Trigger** device is a way to trigger events when players press or release a particular control input. You can use the device to capture when an input is pressed, and which player pressed it.

Response time for input defined in the input trigger device is dependent on the round-trip time between the player's client and the server. Because of this, input can take up to a second depending on the player's internet connection, so keep this in mind when using the input trigger device for your game.

You can use [event binding](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#direct-event-binding) in the Creative toolset, connections in the **Details** panel in UEFN, or Verse code, to trigger other device functions such as blowing up a barrel, changing cameras, or other gameplay that is triggerable.

For help finding the Input Trigger device, see **[Using Devices](https://dev.epicgames.com/documentation/fortnite/using-devices-in-fortnite)**.

If you're using multiple copies of a device on an island, it can be helpful to [rename](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#rename-a-device) them. Choosing names that relate to a device's purpose makes it easier to remember what each one does, and easier to find a specific device when using the [Event Browser](https://dev.epicgames.com/documentation/fortnite/event-browser-in-fortnite-creative)**.

### How the Creative Input Option Works

When you customize the Input Trigger device options, you'll see the **Creative Input** option listed first. This option's values correspond to a number of new input actions that can be configured by players. The way this works is a little complicated, so this section provides a more detailed explanation than the Device Options table has room for.

Players can find and rebind these inputs in the **Creative Input Action** section of the **Keyboard Controls** and **Controller Mapping** tabs in the Settings Menu.

Open the **sidebar**, click the **gear** icon to open the **Setting Menu**, then click either the **Keyboard Controls** or the **Controller Mapping** icons. You can find the **Creative Input Action** section of the settings by scrolling down the list in the left navigation area. This is where players can change which actions map to which controls. These settings apply across all of your Fortnite experiences.

For people on mobile platforms, these inputs always appear as new buttons displayed on the screen. The Input Trigger device has options you can use to customize the icon and color of this button, and whether you want it to display text.

### Contextual Filtering

Some devices are affected by a feature called **contextual filtering**. This feature hides or displays options depending on the values selected for certain related options. This reduces clutter in the Customize panel and makes options easier to manage and navigate. To help identify them, values that trigger contextual filtering are in *italic*.

All options are listed, including those affected by contextual filtering; if they are hidden or displayed based on a specific option's value, there will be a note about it in the Description field for that option.

### Device Options

Default values are **bold**. Values that trigger contextual filtering are *italic*.

You can configure this device with the following options.

**אפשרויות, ערכים ותיאורים:**

##### Input Type

- **Value / Values:** **Creative Input Action**, *Standard Action*
- **Description:** Determines if this device tracks a standard input or a custom input. Standard inputs are used for common game actions. If **Standard Actions** is set as the Input Type, this device will listen for whether inputs bound to those actions are pressed or released. **Creative Input Actions** are custom actions only used by the Input Trigger.

##### Creative Input

- **Value / Values:** Custom 1 (Fire), Custom 2 (Target), Custom 3 (Crouch), Custom 4 (Jump), Custom 5 (Sprint), **Custom 6 (Interact)**, *Custom 7 (Forward/Back)*, *Custom 8 (Left/Right)*, Custom 9 (Previous Item), Custom 10 (Next Item), Custom 11 (Swap Quickbar), Custom 12 (Harvesting Tool)
- **Description:** If the **Input Type** option is set to **Creative Input Actions**, this defines the input control this device is listening for. For more information about how this works, see the **How the Creative Input Option Works** section above. If you select **Custom 7** or **Custom 8**, an additional option is displayed below.

##### Axis Direction

- **Value / Values:** Negative, **Any**, Positive
- **Description:** This option only displays if the Creative Input option is set to **Custom 7** or **Custom 8**. If the input control selected in the **Creative Input** option is a directional axis, this determines which direction the device is listening for. **Negative** is left or backwards, **Positive** is right or forwards.

##### Standard Input

- **Value / Values:** **Fire**, Target, Crouch, Sprint, Jump
- **Description:** This option only displays if the **Input Type** is set to **Standard Action**. These are inputs are the same ones bound to normal player actions. This device only listens for whether these inputs are pressed or released. In cases where a mobile device doesn't have these inputs, a custom button is created.

##### Consume Input

- **Value / Values:** On, **Off**
- **Description:** If set to **On**, this stops the input being read by other actions bound to that input.

##### Show on HUD

- **Value / Values:** **On**, Off
- **Description:** Determines if the input is shown on the HUD.

##### HUD Description

- **Value / Values:** **{input}**, Enter text
- **Description:** If **Show on HUD** is set to **On**, this is the text that will show on the HUD. The text field has a character limit of 24. The default text **{input}** will show the current input.

##### Enabled At Game Start

- **Value / Values:** **On**, Off
- **Description:** Determines if the device is enabled when the game starts.

##### Selected Team

- **Value / Values:** **Any**, Pick a team
- **Description:** Determines which team can activate the input.

##### Selected Class

- **Value / Values:** No Class, **Any**, Pick a class
- **Description:** Determines which classes can activate the input.

##### Invert Team Selection

- **Value / Values:** On, **Off**
- **Description:** If this is set to **On**, the input can be activated by all teams except the one chosen in the **Selected Team** option.

##### Invert Class Selection

- **Value / Values:** On, **Off**
- **Description:** If this is set to **On**, the input can be activated by all classes except the one chosen in the **Selected Class** option.

##### Registered Player Behavior

- **Value / Values:** **Add Registered**, Require Registered, Ignore Registered
- **Description:** Determines how registered players are counted by the device.

#### -
**Add Registered**: Players can either be registered or counted by the device.

- **Value / Values:** -
**Require Registered**: Players must be both registered and counted by the device.
- **Description:** -
**Ignore Registered**: Players must be counted, but not registered by the device.

#### Mobile Options

If you're looking to build an experience that runs smoothly on mobile, the following options allow you to customize button layouts, scaling and to add mobile icons.

 Option Value Description
**Mobile Has Text**

On, Off

This option only displays if the Input Type is set to Creative Input Action. For players on mobile, this determines if the interaction icon shows the description text.

**Mobile Icon**

Hand, Pick an icon

This option only displays if the Input Type is set to Creative Input Action. For players on mobile, this determines what icon is used for the interaction icon. If you select None, the Hand icon will be used. Click the arrow to open the Icon Picker. Click in the search field and type text to find an icon, or use the scroll bar to browse through the collection. Click to select an icon, then click the checkmark to close the Icon Picker.

**Mobile Color**

White, Pick a color

This option only displays if the Input Type is set to Creative Input Action. Determines the color of the icon selected in the Mobile Icon option. Click the arrow to open the Color Picker. Click in the search field and type text to find a color, or use the scroll bar to browse through the collection. Click a color swatch, then click the checkmark to close the Color Picker.

**Mobile Pressed Icon**

**None**, Pick an icon

This determines what icon is used for the interaction icon when the button is pressed. If you select **None**, the Mobile Icon will be used.

**Mobile Use Direct Placement**

On, **Off**

When set to **On**, allows you to change the mobile button placement by changing the **Mobile Offset X **and **Mobile Offset Y **coordinates.

**Mobile Scale**

**1.0 **- 10.0

### Direct Event Binding

Following are the [direct event binding](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#direct-event-binding) options for this device.

#### Functions

A [function](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#function) listens for an event on a device then performs an action.

-
For any function, click the **option**, then **Select Device** to access and select from the **Device dropdown menu**.

-
Once you've selected a device, click **Select Event** and select the event that triggers this function.

-
If more than one device or event triggers a function, press the **Add** button to add a line and repeat these steps.

**אפשרויות ותיאורים:**

##### Enable When Receiving From

Enables the device when an event occurs.

##### Disable When Receiving From

Disables the device when an event occurs.

##### Register Player When Receiving From

Registers the instigating player when an event occurs. Registered players can be added or removed from the list of counted players depending on the **Registered Player Behavior** option's value.

##### Unregister Player When Receiving From

Removes the instigating player from the list of registered players when an event occurs.

##### Unregister All Players When Receiving From

Clears all players from the registered players list when an event occurs.

#### Events

Direct event binding uses events as transmitters. An event tells another device to perform a function.

-
For any event option, click the **option**, then **Select Device** to access and select from the **Device dropdown menu**.

-
Once you've selected a device, click **Select Function** to bind the event to a function for that device.

-
If more than one function is triggered by the event, press the **Add** button and repeat.

**אפשרויות ותיאורים:**

##### On Input Pressed Send Event To

When the input control is pressed, an event is sent to the selected device, which triggers the selected function.

##### On Input Released Send Event To

When the input control is released, an event is sent to the selected device, which triggers the selected function.

### Using the Input Trigger Device in Verse

You can use the code below to control an Input Trigger device in **[Verse](https://dev.epicgames.com/documentation/fortnite/onboarding-guide-to-programming-with-verse-in-unreal-editor-for-fortnite)**. This code shows how to use events and functions in the Input Trigger device API. Modify it to fit the needs of your experience.

using { /Fortnite.com/Devices }

using { /UnrealEngine.com/Temporary/Diagnostics }

using { /Verse.org/Simulation }

## A Verse-authored creative device that can be placed in a level

input_trigger_device_verse_example := class(creative_device):

**Expand code Copy full snippet(67 lines long)

To use this code in your UEFN experience, follow these steps.

-
Drag an **Input Trigger** device onto your island.

-
Create a new Verse device named **input_trigger_device_verse_example**. See [Create Your Own Device Using Verse](https://dev.epicgames.com/documentation/fortnite/create-your-own-device-using-verse-in-unreal-editor-for-fortnite)** for steps.

-
In Visual Studio Code, open **input_trigger_device_verse_example.verse** in Visual Studio Code and paste the code above.

-
Compile your code and drag your Verse-authored device onto your island. See **Adding Your Verse Device to Your Level** for steps.

-
Add a reference for the Input Trigger device on your island to your Verse device. See the **Adding a Verse Reference to a Creative Device in Your Level** section in [Editable Properties](https://dev.epicgames.com/documentation/fortnite/editable-properties-in-verse) for steps.

-
Save your project and click **Launch Session** to playtest.

#### Input Trigger Device Verse API

See the [input_trigger_device API Reference](https://dev.epicgames.com/documentation/en-us/uefn/verse-api/fortnitedotcom/devices/input_trigger_device) for more information on using the Input Trigger device in Verse.

---

## Using Perception Trigger Devices in Fortnite Creative

**כותרת מקורית:** Using Perception Trigger Devices in Fortnite Creative  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/using-perception-trigger-devices-in-fortnite-creative  
**מקור קלט:** `07A_קלט_טריגרים_תנאים_והחלטות(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `using-perception-trigger-devices-in-fortnite-creative`

With the **Perception Trigger**, you can drive gameplay using [line of sight](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#line-of-sight) between the device and players. When conditions related to line-of-sight checks are satisfied, the Perception Trigger transmits a signal through a channel to activate other devices.

 For help on finding the Orbit Camera device in Creative, see [Using Devices](https://dev.epicgames.com/documentation/fortnite/using-devices-in-fortnite).

 If you're using multiple copies of a device on an island, it can be useful to [rename](https://dev.epicgames.com/documentation/fortnite/rename-a-device) them. Choosing names that relate to a device's purpose makes it easier to remember what each one does, and easier to find a specific device when using the [Event Browser](https://dev.epicgames.com/documentation/fortnite/event-browser-in-fortnite-creative).

### Device Options

In its [default](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#default) state, the Perception Trigger does nothing. You must use event binding for this device to be effective. You can configure the device to trigger only for certain classes or teams, to trigger a limited number of times, and you can add a trigger delay and a reset delay. You can also configure the device to display a visual effect or play a sound when triggered.

You can configure this device with the following options.

Default values are **bold**.

**אפשרויות, ערכים ותיאורים:**

##### Times Can Trigger

- **Value / Values:** **Infinite**, Pick a number
- **Description:** Determines the number of times this device can trigger before it is disabled.

##### Device Sees A Player Times Can Trigger

- **Value / Values:** **Infinite**, Pick a number
- **Description:** Determines the number of times this device can trigger "Device Sees A Player" before it is disabled.

##### Device Loses Sight Of A Player Times Can Trigger

- **Value / Values:** **Infinite**, Pick a number
- **Description:** Determines the number of times this device can trigger "Device Loses Sight Of A Player" before it is disabled.

##### Player Looked At Times Can Trigger

- **Value / Values:** **Infinite**, Pick a number
- **Description:** Determines the number of times this device can trigger "Player Looked At" before it is disabled.

##### Player Looked Away Times Can Trigger

- **Value / Values:** **Infinite**, Pick a number
- **Description:** Determines the number of times this device can trigger "Player Looked Away" before it is disabled.

##### Activating Team

- **Value / Values:** **Any**, Pick a team
- **Description:** Determines which team can activate this device.

##### Allowed Class

- **Value / Values:** No Class, **Any**, Pick a class
- **Description:** Determines which class can activate this device.

##### Player Looked At Transmit Every X Triggers

- **Value / Values:** **1**, Pick a number
- **Description:** Sets the device to only send "Player Looked At" after being triggered the specified number of times.

##### Player Looked Away Transmit Every X Triggers

- **Value / Values:** **1**, Pick a number
- **Description:** Sets the device to only send "Player Looked Away" after being triggered the specified number of times.

##### Device Sees A Player Transmit Every X Triggers

- **Value / Values:** **1**, Pick a number
- **Description:** Sets the device to only send "Device Sees A Player" after being triggered the specified number of times.

##### Device Loses Sight Of A Player Transmit Every X Triggers

- **Value / Values:** **1**, Pick a number
- **Description:** Sets the device to only send "Device Loses Sight Of A Player" after being triggered the specified number of times.

##### Delay

- **Value / Values:** **None**, Pick a delay time
- **Description:** After being triggered, the device will wait this amount of time (in seconds or minutes) before sending a signal.

##### Reset Delay

- **Value / Values:** **None**, Pick a reset time
- **Description:** Specifies the length of time the device must wait after being triggered before it can be triggered again.

##### Trigger Sound

- **Value / Values:** **Enabled**, Disabled
- **Description:** Determines whether a sound is played when the device is triggered.

##### Trigger VFX

- **Value / Values:** **Enabled**, Disabled
- **Description:** Determines whether visual effects are displayed when the device is triggered.

##### Enabled on Game Start

- **Value / Values:** **Enabled**, Disabled
- **Description:** Determines whether or not the device is enabled when the game starts.

##### Trigger Sound

- **Value / Values:** Enabled, Disabled
- **Description:** Determines whether or not the device triggers an audio effect.

##### Visible in Game

- **Value / Values:** Yes, No
- **Description:** Whether or not the device will be visible during the game.

### Direct Event Binding

**Direct event binding** allows devices to communicate directly, which makes your workflow more intuitive, and gives you more freedom to focus on your design ideas. With this system, devices communicate directly with other devices.

Below are the functions and events for this device.

#### Functions

A [function](https://dev.epicgames.com/documentation/en-us/fortnite-creative/fortnite-creative-glossary) listens for an event on a device then performs an action.

-
For any function, click the option, then Select Device to access and select from the Device dropdown menu.

-
Once you've selected a device, click Select Event to bind the device to an event that will trigger the function.

-
If more than one device or event triggers a function, click the Add button to add a line and repeat these steps.

**אפשרויות ותיאורים:**

##### Enable When Receiving From

Enables the device when an event occurs.

##### Disable When Receiving From

Disables the device when an event occurs.

##### Reset Times Triggered When Receiving From

Resets the number of times the trigger has been activated when an event occurs. This resets the **Transmits Every X Triggers** and **Times and Trigger** options.

#### Events

An [event](https://dev.epicgames.com/documentation/en-us/fortnite-creative/fortnite-creative-glossary) tells another device when to perform a function.

-
For any event, click the option, then Select Device to access and select from the Device dropdown menu.

-
Once you've selected a device, click Select Function to bind this event to a function for that device.

-
If more than one function is triggered by the event, click the Add button to add a line and repeat these steps.

**אפשרויות ותיאורים:**

##### On Device Sees a Player Send Event To

Sends an event when the device has a direct line of sight to a player.

##### On Device Loses Sight of a Player Send Event To

Sends an event when the device loses line of sight to a player.

##### On Player Looks at Device Send Event To

Sends an event when a player has line of sight to the device.

##### On Player Looks Away From Device Send Event To

Sends an event when a player loses line of sight to the device.

### Design Examples

Here are some examples of how you can use the Perception Trigger device.

-
[Hide and Seek](https://dev.epicgames.com/documentation/fortnite/using-perception-trigger-devices-in-fortnite-creative)

-
[Moving Target](https://dev.epicgames.com/documentation/fortnite/using-perception-trigger-devices-in-fortnite-creative)

#### Hide and Seek

Create a [hide-and-seek](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#hide-and-seek) game using the Perception Trigger as the seeker. To make the game more interesting, turn the Perception Trigger on and off every 5 seconds to give the player opportunities to move around the room.

**Devices used:**

-
1 x **Perception Trigger**

-
1 x [**Damage Volume**](https://dev.epicgames.com/documentation/fortnite/using-damage-volume-devices-in-fortnite-creative)

-
1 x [**HUD Message**](https://dev.epicgames.com/documentation/fortnite/using-hud-message-devices-in-fortnite-creative)

-
2 x [**Timed Objective**](https://dev.epicgames.com/documentation/fortnite/using-timed-objective-devices-in-fortnite-creative)

-
Create a simple hide-and-seek area with different obstacles to block the seeker’s sightline.

-
Place a **Damage Volume** in the center of the play area and customize it to the following settings:

 Option Value Description
Zone Width

7

The Damage Volume will be 7 tiles wide. Adjust this setting so the Damage Volume encompasses the entire area of the game.

Zone Depth

3

The Damage Volume will be 3 tiles deep. Adjust this setting so that the Damage Volume encompasses the entire area of the Hide and Seek game.

Damage Type

Elimination

If a player is inside of the Damage Volume, they will be immediately eliminated.

Enabled During Phase

None

The Damage Volume will begin disabled.

-
Place a **HUD Message** outside of the play area and customize it to the following settings:

**אפשרויות, ערכים ותיאורים:**

##### Message

- **Value / Values:** You’ve Been Spotted!
- **Description:** This message will show when the player is spotted by the Perception Trigger.

##### Time From Round Start

- **Value / Values:** Off
- **Description:** The message will not be shown automatically after the round starts.

#### -
Place a large **Perception Trigger** toward one end of the play area and customize it to the following settings:

- **Value / Values:** Option Value Description
Enabled on Game Start
- **Description:** Disabled

##### The Perception Trigger will be disabled when the game starts.

- **Value / Values:** -
Set the direct event bindings of the Perception Trigger to the following:
- **Description:** Function Device Event Description
On Device Sees A Player Send Event To

##### DamageVolume

- **Value / Values:** Enable
- **Description:** When the player is spotted, the Damage Volume will turn on, eliminating them.

##### On Device Sees A Player Send Event To

- **Value / Values:** SeenHUDMessage
- **Description:** Show

##### When the player is spotted, they will be shown a HUD Message telling them that they were spotted.

- **Value / Values:** -
To create the effect of the eye turning on and off every 5 seconds, you will use two Timed Objectives. Place a **Timed Objective** outside of the play area. This will be the device that **enables** the Perception Trigger, so give it a clear name. Customize it to the following settings:
- **Description:** Option Value Description
Start When Round Starts

##### Yes

- **Value / Values:** The Timed Objective will begin counting when the round starts.
- **Description:** Time

##### 5 Seconds

- **Value / Values:** The Timed Objective will complete after 5 seconds.
- **Description:** Timer Label Text

##### The eye will see in…

- **Value / Values:** The HUD will display this label before the countdown.
- **Description:** Visible During Game

##### No

- **Value / Values:** The Timed Objective itself will not be visible during gameplay.
- **Description:** Completion Behavior

##### Reset

- **Value / Values:** After completing the countdown, the Timed Objective will reset and will be ready to be started again.
- **Description:** Audio Effects

##### Off

- **Value / Values:** The Timed Objective will not play any audio effects.
- **Description:** -
Place another **Timed Objective** outside of the play area. This will be the device that **disables** the Perception Trigger, so give it a clear name that differentiates it from the other Timed Objective. Customize it to the following settings:

#### Option Value Description
Time

- **Value / Values:** 5 Seconds
- **Description:** The Timed Objective will complete after 5 seconds.

##### Timer Label Text

- **Value / Values:** The eye will stop looking in…
- **Description:** The HUD will display this label before the countdown.

##### Visible During Game

- **Value / Values:** No
- **Description:** The Timed Objective itself will not be visible during gameplay.

##### Completion Behavior

- **Value / Values:** Reset
- **Description:** After completing the countdown, the Timed Objective will reset and will be ready to be started again.

##### Audio Effects

- **Value / Values:** Off
- **Description:** The Timed Objective will not play any audio effects.

#### -
Set the direct event bindings of the **first** Timed Objective to the following:

- **Value / Values:** Function Device Event Description
On Completed Send Event To
- **Description:** PerceptionTrigger

##### Enable when Receiving From

- **Value / Values:** When this Timed Objective completes, it enables the Perception Trigger.
- **Description:** On Completed Send Event To

##### StopLookingTimedObjective

- **Value / Values:** Start
- **Description:** When this Timed Objective completes, it starts the countdown on the other Timed Objective.

#### -
Set the direct event bindings of the **second** Timed Objective to the following:

- **Value / Values:** Function Device Event Description
On Completed Send Event To
- **Description:** PerceptionTrigger

##### Disable when Receiving From

- **Value / Values:** When this Timed Objective completes, it disables the Perception Trigger.
- **Description:** On Completed Send Event To

##### StartLookingTimedObjective

- **Value / Values:** Start
- **Description:** When this Timed Objective completes, it starts the countdown on the other Timed Objective.

##### Here’s an overview of how devices communicate in this example:

- **Value / Values:** Device A Function Device B Event Explanation
**DamageVolume**
- **Description:** Enable

##### PerceptionTrigger

- **Value / Values:** On Device Sees A Player Send Event To
- **Description:** When the player is spotted, the Damage Volume will turn on, eliminating them.

##### SeenHUDMessage

- **Value / Values:** Show
- **Description:** **PerceptionTrigger**

##### On Device Sees A Player Send Event To

- **Value / Values:** When the player is spotted, they will be shown a HUD Message telling them that they were spotted.
- **Description:** **PerceptionTrigger**

##### Enable when Receiving From

- **Value / Values:** **StartLookingTimedObjective**
- **Description:** On Completed Send Event To

##### When this Timed Objective completes, it enables the Perception Trigger.

- **Value / Values:** **StopLookingTimedObjective**
- **Description:** Start

##### StartLookingTimedObjective

- **Value / Values:** On Completed Send Event To
- **Description:** When this Timed Objective completes, it starts the countdown on the other Timed Objective.

##### PerceptionTrigger

- **Value / Values:** Disable when Receiving From
- **Description:** **StopLookingTimedObjective**

##### On Completed Send Event To

- **Value / Values:** When this Timed Objective completes, it disables the Perception Trigger.
- **Description:** **StartLookingTimedObjective**

##### Start

- **Value / Values:** **StopLookingTimedObjective**
- **Description:** On Completed Send Event To

##### When this Timed Objective completes, it starts the countdown on the other Timed Objective.

- **Value / Values:** You now have the basic functionality for a hide and seek game using the Perception Trigger.
- **Description:** This basic functionality could be extended and applied in many different game modes for interesting results. You could create a game where the player needs to reach a certain objective without being spotted. Or consider exploring a competitive multiplayer mode in which players have to battle one another while avoiding being seen by the eye. There are many possibilities, so try to find creative ways to combine different game mechanics in new and unexpected ways.

#### Moving Target

Use the Perception Trigger’s player sightline functionality to change the game based on where the player is looking. In this example, create targets that disappear one second after the player first sees them.

**Devices used:**

-
3 x **Perception Trigger**

-
1 x [**Item Granter**](https://dev.epicgames.com/documentation/fortnite/using-item-granter-devices-in-fortnite-creative)

-
1 x [**Player Spawner**](https://dev.epicgames.com/documentation/fortnite/using-player-spawn-pad-devices-in-fortnite-creative)

-
3 x [Prop Manipulator](https://dev.epicgames.com/documentation/fortnite/using-prop-manipulator-devices-in-fortnite-creative)

-
3 x [**Trigger**](https://dev.epicgames.com/documentation/fortnite/using-trigger-devices-in-fortnite-creative)

-
1 x [Random Number Generator](https://dev.epicgames.com/documentation/fortnite/using-random-number-generator-devices-in-fortnite-creative)

-
Place an **Item Granter** and, while standing near it, drop a Tactical Assault Rifle to register the weapon.

-
Place a **Player Spawner** in a central location and keep the default settings. Set the direct event bindings to the following:

 Function Device Event Description
On Player Spawned Send Event To

ItemGranter

Grant Item

When the player spawns, they will be granted the Tactical Assault Rifle.

-
Place a target prop and attach a **Prop Manipulator** to it. Customize the Prop Manipulator to the following settings:

 Option Value Description
Start Hidden

Yes

At the beginning of the game, the target will be invisible.

Prop Health

Invulnerable

The target will not be destructible.

-
In front of the target prop, place a **Perception Trigger** and customize it to the following settings:

**אפשרויות, ערכים ותיאורים:**

##### Delay

- **Value / Values:** 1 Second
- **Description:** The Perception Trigger will send an event 1 second after it is triggered.

##### Visible in Game

- **Value / Values:** No
- **Description:** The Perception Trigger will not be visible during gameplay.

##### Enabled on Game Start

- **Value / Values:** Disabled
- **Description:** The Perception Trigger will start the game disabled.

#### -
Place a **Trigger** and customize it to the following settings:

- **Value / Values:** Option Value Description
Trigger Sound
- **Description:** Disabled

##### The Trigger will not make a sound when it is triggered.

- **Value / Values:** -
Set the direct event bindings of the Trigger to the following:
- **Description:** Function Device Event Description
On Triggered Send Event To

##### PropManipulator1

- **Value / Values:** Show Props
- **Description:** When this Trigger is triggered, the Prop Manipulator will show the target prop.

##### On Triggered Send Event To

- **Value / Values:** PerceptionTrigger1
- **Description:** Enable when Receiving From

##### When this Trigger is triggered, the corresponding Perception Trigger will be enabled.

- **Value / Values:** -
Place a **Random Number Generator** away from the play area and customize it to the following settings:
- **Description:** Option Value Description
Value Limit 2

##### 3

- **Value / Values:** The Random Number Generator will choose a value between 1 and 3.
- **Description:** Roll Time

##### Instant

- **Value / Values:** The Random Number Generator will not have any delay when picking a number.
- **Description:** Pick Each Number Once

##### Yes (Reset on Game Start)

- **Value / Values:** The Random Number Generator will not repeat the same number twice until it has chosen all available numbers.
- **Description:** Zone

##### Forward

- **Value / Values:** A trigger zone will extend out in front of the Random Number Generator.
- **Description:** Length

##### 3

- **Value / Values:** The trigger zone will be 3 tiles long.
- **Description:** Play Audio

##### No

- **Value / Values:** The Random Number Generator will not play any audio.
- **Description:** Activate on Game Phase

##### Game Start

- **Value / Values:** The Random Number Generator will automatically activate when the game begins.
- **Description:** -
Set the direct event bindings of the Perception Trigger to the following:

#### Function Device Event Description
On A Player Looks At Device Send Event To

- **Value / Values:** PropManipulator1
- **Description:** Hide Props

##### 1 second after the player looks at the Perception Trigger, the target prop will be hidden.

- **Value / Values:** On A Player Looks At Device Send Event To
- **Description:** PerceptionTrigger1

##### Disable when Receiving From

- **Value / Values:** 1 second after the player looks at the Perception Trigger, the Perception Trigger itself will be disabled.
- **Description:** On A Player Looks At Device Send Event To

##### RandomNumberGenerator

- **Value / Values:** Activate
- **Description:** 1 second after the player looks at the Perception Trigger, the Random Number Generator will be activated to choose a new target to enable.

#### -
Select the target prop, Prop Manipulator, Perception Trigger, and Trigger, then duplicate them two more times in different areas around the player.

- **Value / Values:** -
Move each of the three Triggers that correspond with the different targets into the three different trigger zone areas of the Random Number Generator.
- **Description:** Here’s an overview of how devices communicate in this example:

#### Device A Function Device B Event Explanation
**ItemGranter**

- **Value / Values:** Grant Item
- **Description:** **PlayerSpawner**

##### On Player Spawned Send Event To

- **Value / Values:** When the player spawns, they will be granted the Tactical Assault Rifle.
- **Description:** **PropManipulator1-3**

##### Show Props

- **Value / Values:** **Trigger1-3**
- **Description:** On Triggered Send Event To

##### When a Trigger is triggered, the corresponding Prop Manipulator will show the target prop.

- **Value / Values:** **PerceptionTrigger1-3**
- **Description:** Enable when Receiving From

##### Trigger1-3

- **Value / Values:** On Triggered Send Event To
- **Description:** When a Trigger is triggered, the corresponding Perception Trigger will be enabled.

##### PropManipulator1-3

- **Value / Values:** Hide Props
- **Description:** **PerceptionTrigger1-3**

##### On A Player Looks At Device Send Event To

- **Value / Values:** 1 second after the player looks at a Perception Trigger, the corresponding target prop will be hidden.
- **Description:** **PerceptionTrigger1-3**

##### Disable when Receiving From

- **Value / Values:** **PerceptionTrigger1-3**
- **Description:** On A Player Looks At Device Send Event To

##### 1 second after the player looks at a Perception Trigger, the Perception Trigger itself will be disabled.

- **Value / Values:** **RandomNumberGenerator**
- **Description:** Activate

##### PerceptionTrigger1-3

- **Value / Values:** On A Player Looks At Device Send Event To
- **Description:** 1 second after the player looks at a Perception Trigger, the Random Number Generator will be activated to choose a new target to enable.

##### You now have the basic functionality for targets that disappear based on when the player looks at them.

- **Value / Values:** To spruce up the gameplay in this example, explore using Prop Movers to create targets that also move when they are enabled. Explore adding obstacles and barricades to force the player to move around in the area as well.
- **Description:** When using the Perception Trigger, be very aware of how objects are placed on your island. This example would be much less effective if all of the targets were close to one another and the player could see all three at once. Additionally, if the player moves outside of the center of the three targets, the same issue will occur. Be intentional about the level design of your island to ensure that the player can only go where you intend them to.

---

## Using Player Counter Devices in Fortnite Creative

**כותרת מקורית:** Using Player Counter Devices in Fortnite Creative  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/using-player-counter-devices-in-fortnite-creative  
**מקור קלט:** `07A_קלט_טריגרים_תנאים_והחלטות(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `using-player-counter-devices-in-fortnite-creative`

Using the **Player Counter**, you can find out how many players of a certain team or [class](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#class) are in the game, or how many are in a specific area. The device can send [signals](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) based on that count. Some examples of how you can use this device include:

-
Balancing teams if a lot of players leave at one time.

-
Creating areas on your island that require a certain amount of players (such as for a [minigame](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#mini-game)).

-
Creating events that only start if the required number of players are present.

To find the Player Counter device, see [****](https://dev.epicgames.com/documentation/fortnite/using-devices-in-fortnite-creative)**[Using Devices](https://dev.epicgames.com/documentation/fortnite/using-devices-in-fortnite)**.

If you're using multiple copies of a device on an island, it can be helpful to [rename](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#rename-a-device) them. Choosing names that relate to a device's purpose makes it easier to remember what each one does, and easier to find a specific device when using the [Event Browser](https://dev.epicgames.com/documentation/fortnite/event-browser-in-fortnite-creative).

### Contextual Filtering

Some devices are affected by a feature called **contextual filtering**. This feature hides or displays options depending on the values selected for certain related options. This reduces clutter in the Customize panel and makes options easier to manage and navigate. To help identify them, values that trigger contextual filtering are in *italic*.

All options are listed, including those affected by contextual filtering; if they are hidden or displayed based on a specific option's value, there will be a note about it in the Description field for that option.

### Device Options

This device has some basic functionality, like setting a target value, and criteria for comparisons. Additionally, there are some advanced options, like determining when the count comparison occurs, which team or class is counted, and whether the device transmits when the comparison happens.

You can configure this device with the following options.

Default values are **bold**. Values that trigger contextual filtering are *italic*.

 Option Value Description
**Compare Player Count**

Do Not Compare, Fewer Than, Equal or Fewer, Not Equal To, **Equal To**, Equal or More, More Than

Determines how the counted players need to be compared to the target player count. The comparison determines whether the **When Count Succeeds Transmit On** or **When Count Fails Transmit On** options are activated.

**Target Player Count**

**2 Players**, Pick or enter a number of players

This is the required amount of players for the zone. Use the arrows to choose a number, or click in the field to type in a number. If the player count reaches this number, the **When Count Succeeds Transmit On** option is activated; if the player count does not reach this number, the **When Count Fails Transmit On** option is activated.

**Compare at Game Start**

**No**, Yes

Determines whether the device automatically compares counted players against the target number when the game starts.

**Compare on Count Change**

**Yes**, No, During Game

Determines whether the device compares the player count to the target number each time a player is counted or removed. If you choose **During Game**, players are only counted while the game is in progress.

**Transmit on Player Counted/Removed**

**Every Time**, Once Per Player, Signal Only

Determines when the device activates a transmit option for players being Counted or Removed. If you choose **Once Per Player**, each transmitter sends a signal once for each player in a game, even if they leave the game and return. If you choose **Signal Only**, the transmitter only activates when a signal from **Transmit for All** is received.

**Transmit for on Compare Result Change**

**Last Instigator**, None, Random Counted Player, All Counted Players

Determines what happens when a compare test succeeds or fails.

-
**Last Instigator**: Transmits once using the last player to interact with the device as the instigator.

-
**None**: Does not transmit any player instigator.

-
**Random Counted**: Chooses a random player that is currently being counted and transmits that player as the instigator.

-
**All Counted Players**: Transmits once for each player counted.

**Counted Team**

**Any**, Pick a team

Players on the selected team are counted. Use the arrows to pick a team number, or click in the field to type in a number.

-
**Only Selected**: Only the team chosen in the **Counted Team** option is affected.

-
**All But Selected**: All teams are affected except the team chosen in the **Counted Team** option.

**Invert Team Selection**

On, **Off**

If set, the device will count all but the selected team.

**Counted Class**

**Any**, No Class, Pick a class

Players with the selected class assigned are counted. Use the arrows to pick a class number, or click in the field to type in a class number. If you choose **No Class**, only players who are not assigned a class are counted. If you choose **Any**, all players with an assigned class are counted.

-
**Only Selected**: On the class chosen in the **Counted Class** option is affected.

-
**All But Selected**: All classes are affected except the class chosen in the **Counted Class** option.

**Invert Class Selection**

On, **Off**

If set to **On**, the device will count all but the selected class.

**Enabled On Phase**

**Always**, None, Pre-Game Only, Gameplay Only

Determines the phases in which the device is enabled. **Pre-Game Only** includes all phases that occur before the game starts.

**Include Spectators**

**Yes**, No

Determines whether the device includes spectators as counted players when checking all players on the island.

**Info Panel Visible**

**On**, Off

Determines whether the panel that shows the player count is visible to players during the game.

**Icon Scale**

**1.0x**, Pick a scale multiplier

Determines the size of the Counter Icon. This is not related to the size of the device. Use the arrows to choose a multiplier, or click in the field to type in a number.

**Info Panel Icon**

**Player Icon**, Pick an icon

Determines the icon that is displayed on the Player Counter info panel. Click the icon to open the Icon Library Picker. You can choose an icon by scrolling through the Icon Library, or type a word into the Search box to search for a specific icon. Select an icon, then click the checkmark.

**Base Color**

**Default Red**, Pick a color

Determines the color of the icon and the zone. This color is also used for the numbers when the counter is not counting, or when the count has not yet succeeded. Click the color swatch to open the Color Picker. Each color swatch has its Hex Code next to the swatch. You can also type a Hex Code into the Search bar to find a specific color. Select a color, then click the checkmark.

**Success Color**

**Default Blue**, Pick a color

Determines the color of the icon and the zone. This color is also used for the numbers when the counter is not counting, or when the count has not yet succeeded. Click the color swatch to open the Color Picker. Each color swatch has its Hex Code next to the swatch. You can also type a Hex Code into the Search bar to find a specific color. Select a color, then click the checkmark.

**Count Registered Players**

**Union**, Intersection, Difference

Determines how the set of players counted by the device (Counted) and the set of players tracked manually (Tracked) are combined.

-
**Union**: The set of Counted players and the set of Tracked Players are combined.

-
**Intersection**: Players must be in both the set of Counted players, and the set of Tracked players.

-
**Difference**: Players must be in the set of Counted players but not in the set of Tracked players.

**Use Zone**

On, **Off**

The default is for the device to count all players on the island. If you select **On**, additional options are displayed below this one.

**Zone Shape**

**Box**, Cylinder

This option only displays if the **Use Zone** option is set to **On**. Determines the shape of the defined zone.

**Time in Zone to Count**

**Instant**, Pick a number of seconds

This option only displays if the **Use Zone** option is set to **On**. When players are counted in a zone, this determines how long players need to be in the zone in order to be counted. Use the arrows to choose an amount, or click in the field to type in an amount.

**Zone Visible During Game**

**No**, Yes

This option only displays if the **Use Zone** option is set to **On**. Determines whether the defined zone is visible to players during the game.

**Size Units**

**Tiles**, *Meters*

This option only displays if the **Use Zone** option is set to **On**. Determines whether the size of the defined zones is measured in tiles or in Meters. If you choose **Meters**, the **Zone Width**, **Zone Depth**, and **Zone Height** options will have "Meters" in parentheses instead of "Tiles".

**Zone Width (Tiles)**

**1 Tile**, Select a zone width

This option only displays if the **Use Zone** option is set to **On**. This determines the width of the defined zone. Use the arrows to choose, or click in the field to type in a number.

**Zone Depth (Tiles)**

**1 Tile**, Select a zone depth

This option only displays if the **Use Zone** option is set to **On**. This determines the depth of the defined zone. Use the arrows to choose, or click in the field to type in a number.

**Zone Height (Tiles)**

**1 Tile**, Select a zone height

This option only displays if the **Use Zone** option is set to **On**. This determines the height of the defined zone. Use the arrows to choose, or click in the field to type in a number.

**Zone Width (Meters)**

**5.0M**, Select a zone width

This option only displays if the **Use Zone** option is set to **On** and the **Size Units** option is set to **Meters**. This determines the width of the defined zone. Use the arrows to choose, or click in the field to type in a number.

**Zone Depth (Meters)**

**5.0M**, Select a zone depth

This option only displays if the **Use Zone** option is set to **On** and the **Size Units** option is set to **Meters**. This determines the depth of the defined zone. Use the arrows to choose, or click in the field to type in a number.

**Zone Height (Meters)**

**4.0M**, Select a zone height

This option only displays if the **Use Zone** option is set to **On** and the **Size Units** option is set to **Meters**. This determines the height of the defined zone. Use the arrows to choose, or click in the field to type in a number.

**Zone Offset Forward/Back**

**0%**, Pick a positive or negative percentage

This option only displays if the **Use Zone** option is set to **On**. This determines how far forward or back the defined zone is from the base of the device. Use the arrows to choose, or click in the field to type in a number.

**Zone Offset Left/Right**

**0%**, Pick a positive or negative percentage

This option only displays if the **Use Zone** option is set to **On**. This determines how far to the left or right the defined zone is from the base of the device. Use the arrows to choose, or click in the field to type in a number.

**Zone Offset Up/Down**

**0%**, Pick a positive or negative percentage

This option only displays if the **Use Zone** option is set to **On**. This determines how far up or down the defined zone is from the base of the device. Use the arrows to choose, or click in the field to type in a number.

### Direct Event Binding

Direct event binding allows devices to communicate directly, which makes your workflow more intuitive, and gives you more freedom to focus on your design ideas.

Below are the following direct event binding options for this device.

#### Functions

A [function](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#function) listens for an event on a device then performs an action.

-
For any function, click the **option**, then **Select Device** to access and select from the **Device dropdown menu**.

-
Once you've selected a device, click **Select Event** and select the event that triggers this function.

-
If more than one device or event triggers a function, press the **Add** button to add a line and repeat these steps.

**אפשרויות ותיאורים:**

##### Compare Players to Target When Receiving From

This function compares the player count to the target number when an event occurs, and triggers either the **On Count Succeed** or the **On Count Fail** events.

##### Enable When Receiving From

This function enables the device when an event occurs.

##### Disable When Receiving From

This function disables the device when an event occurs.

##### Transmit for All Counted Players When Receiving From

When an event occurs, this function sends the **On Player Counted** event for every player currently counted. This will override the setting for the **Transmit On Player Counted/Removed** function, and will always send a signal for every player currently counted.

##### Increment Target Player Count When Receiving From

When an event occurs, this function increases the Target Player Count number by 1. This immediately triggers a new comparison.

##### Decrement Target Player Count When Receiving From

When an event occurs, this function reduces the Target Player Count number by 1. This immediately triggers a new comparison.

##### Reset Target Player Count When Receiving From

When an event occurs, this function returns the Target Player Count to its original number. If the Target Player Count was previously increased or decreased, this reset immediately triggers a new comparison.

##### Register Player When Receiving From

This function registers the instigating player when an event occurs. Registered players may be added or removed from the set of Counted players depending on the value set for the **Count Registered Players** option.

##### Unregister Player When Receiving From

This function unregisters the instigating player when an event occurs. Unregistered players may be added or removed from the set of Counted players depending on the value set for the **Count Registered Players** option.

##### Unregister All Players When Receiving From

This function clears all players from the registered list. Unregistered players may be added or removed from the set of Counted players depending on the value set for the **Count Registered Players** option.

#### Events

Direct event binding uses events as transmitters. An event tells another device to perform a function.

-
For any event option, click the **option**, then **Select Device** to access and select from the **Device dropdown menu**.

-
Once you've selected a device, click **Select Function** to bind the event to a function for that device.

-
If more than one function is triggered by the event, press the **Add** button and repeat.

**אפשרויות ותיאורים:**

##### On Count Succeeds Send Event To

If the player count matches the Target Player Count number, an event is sent to the selected device.

##### On Count Fails Send Event To

If the player count does not match the Target Player Count number, an event is sent to the selected device.

##### On Player Counted Send Event To

If a valid player enters the zone and is counted, an event is sent to the selected device. It uses the rule in the value for the **Transmit On Player Counted/Removed** option, unless this event is triggered by the **Transmit for All Counted Players When Receiving From** function.

##### On Player Removed Send Event To

When a player is no longer counted by this device (such as when they leave the zone, leave the game, or are assigned to a different Team or Class), an event is sent to the selected device.

---

## Using Pulse Trigger Devices in Fortnite Creative

**כותרת מקורית:** Using Pulse Trigger Devices in Fortnite Creative  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/using-pulse-trigger-devices-in-fortnite-creative  
**מקור קלט:** `07A_קלט_טריגרים_תנאים_והחלטות(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `using-pulse-trigger-devices-in-fortnite-creative`

The **Pulse Trigger** is a device you can use to damage players who collide with it. You can also use it as a trigger to activate other devices.

The device creates a representation of a metronome. Based on the BPM (beats per minute) you select, the activated pulse trigger sends out a pulse that travels down a line and triggers devices within its path.

For help on how to find the **Pulse Trigger** device, see [Using Devices](https://dev.epicgames.com/documentation/fortnite/using-devices-in-fortnite).

If you're using multiple copies of a device on an island, it can be helpful to [rename](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#rename-a-device) them. You can choose names that relate to each device’s purpose, so it’s easier to remember what each one does.

### Contextual Filtering

Some devices are affected by a feature called **contextual filtering**. This feature hides or displays options depending on the values selected for certain related options. This feature will reduce clutter in the Customize panel and make options easier to manage and navigate.

However, it may not be easy to recognize which options or values trigger contextual filtering. To help you identify them, in our device docs we use *italic* for any values that trigger contextual filtering. All options will be listed, including those affected by contextual filtering; if they are hidden or displayed based on a specific option’s value, there will be a note about that in the Description field for that option.

### Device Options

The pulse trigger has some basic functionality, like the size of the zone, how many times the pulse trigger loops, the amount of damage it deals to players, and the direction of the pulse. Additionally, there are some advanced options, like which game phase the pulse trigger activates in, the activation type, and whether player information is sent.

Default values are **bold**. Values that trigger contextual filtering are *italic*.

**אפשרויות, ערכים ותיאורים:**

##### Loop Infinitely

- **Value / Values:** On, ***Off***
- **Description:** Determines if the device loops infinitely. If this is set to **On**, the **Number of Loops** option is displayed below this one.

##### Number of Loops

- **Value / Values:** **1**, Pick or enter a number
- **Description:** This only displays if the **Loop Infinitely** option is set to **Off**. Determines how many times the pulse trigger will loop before stopping.

##### Tempo (BPM)

- **Value / Values:** **110**, Pick or enter a number
- **Description:** Determines how fast (in beats per minute or BPM) the pulse travels.

##### Length

- **Value / Values:** **4**, Pick or enter a number
- **Description:** Sets the number of tiles long the pulse trigger volume is.

##### Width

- **Value / Values:** **1.0**, Pick a number
- **Description:** Sets the number of tiles wide the pulse trigger volume is.

##### Height

- **Value / Values:** **1.0**, Pick a number
- **Description:** Sets the number of tiles high the pulse trigger volume is.

##### Zone Direction

- **Value / Values:** None, **Forward**, Left, Right, Backwards
- **Description:** Determines the direction the zone lies in relation to the device.

##### Activation Type

- **Value / Values:** **Send Pulse**, Toggle Pulse On/Off, Toggle Pulse Play/Pause
- **Description:** Determines whether activating the device sends a new pulse every time, toggles the pulse between running and stopping, or toggles the pulse between playing and pausing.

##### Zone Visible During Game

- **Value / Values:** On, **Off**
- **Description:** Determines whether or not the zone is visible during the game.

##### Disable Activation While Running

- **Value / Values:** On, **Off**
- **Description:** Determines whether the device can be activated again while a pulse is already in motion.

##### Active When Paused

- **Value / Values:** On, **Off**
- **Description:** Determines whether a paused trigger will stay active and trigger anything that walks into it.

##### Pulse Direction

- **Value / Values:** **Forward**, Backwards, Bounce Forward, Up, Down, Bounce Up
- **Description:** Determines which direction the pulse will travel when the device is activated. If you choose **Bounce**, the pulse will reverse direction when it reaches the end of the zone.

##### Damage

- **Value / Values:** **0.0**, Pick or enter a number
- **Description:** Determines the level of damage the pulse should deal to players it hits.

##### Use Flashing Warning Signs

- **Value / Values:** On, **Off**
- **Description:** Determines if flashing warning signs are displayed when a player is damaged by the pulse.

##### Activate on Phase

- **Value / Values:** **None**, Waiting for Players, Game Countdown, Game Start
- **Description:** Determines in which phase the pulse trigger is activated.

##### Send Player Information

- **Value / Values:** **On**, Off
- **Description:** When the pulse trigger activates another device, this determines whether or not the pulse trigger identifies the activating player as an instigator and sends that information to the other device.

##### Enabled On Phase

- **Value / Values:** None, **Always**, Pre-Game Only, Gameplay Only, Create Only
- **Description:** Determines the phase in which the device is enabled.

##### Custom Pulse Style

- **Value / Values:** On, **Off**
- **Description:** If you set this option to **On**, the visual style of the pulse is more solid than the standard translucent pulse. This makes it easier to see the progress of the pulse.

### Direct Event Binding

Following are the [direct event binding](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#direct-event-binding) options for this device.

#### Functions

A [function](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#function) listens for an event on a device then performs an action.

-
For any function option, click the **option**, then **Select Device** to access and select from the **Device dropdown menu**.

-
Once you've selected a device, click **Select Event** to bind the timer to an event that will trigger the function for the device.

-
If more than one device should be affected by a function, press the **Add** button and repeat.

**אפשרויות ותיאורים:**

##### Start Pulse When Receiving From

This function starts the pulse when an event occurs.

##### Stop Pulse When Receiving From

This function stops the pulse when an event occurs.

##### Resume Pulse When Receiving From

This function restarts the pulse when an event occurs.

##### Enable When Receiving From

This function enables the device when an event occurs.

##### Disable When Receiving From

This function disables the device when an event occurs.

#### Events

An [event](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#event) tells another device when to perform a function.

-
For any event option, click the **option**, then **Select Device** to access and select from the **Device dropdown menu**.

-
Once you've selected a device, click **Select Function** to bind the timer to a function for that device.

-
If more than one device is affected by the function, press the **Add** button and repeat.

**אפשרויות ותיאורים:**

##### On Player Hit Send Event To

Click the arrow to display a list of available devices.

##### Click the arrow to display a list of available functions.

When a player is hit by the pulse, the device sends an event to the selected device, which triggers the selected function.

### Gameplay Examples Using the Pulse Trigger

-
[Color Switch Challenge](https://dev.epicgames.com/documentation/fortnite/color-switch-challenge-gameplay-example-in-fortnite-creative)

-
[Mix Tape](https://dev.epicgames.com/documentation/fortnite/mix-tape-in-fortnite-creative)

---

## Using Random Number Generator Devices in Fortnite Creative

**כותרת מקורית:** Using Random Number Generator Devices in Fortnite Creative  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/using-random-number-generator-devices-in-fortnite-creative  
**מקור קלט:** `07A_קלט_טריגרים_תנאים_והחלטות(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `using-random-number-generator-devices-in-fortnite-creative`

**
The **Random Number Generator** device randomly rolls a number in the range between two numbers you choose. The result can then be [transmitted](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) to other devices to activate them.

You also have an option to use a [volume](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#volume) to trigger other devices placed within the volume.

For help on how to find the Random Number Generator (RNG)** device, see [Using Devices](https://dev.epicgames.com/documentation/fortnite/using-devices-in-fortnite).

If you're using multiple copies of a device on an island, it can be useful to rename them. Choosing names that relate to a device's purpose makes it easier to remember what each one does, and easier to find a specific device when using the [Event Browser](https://dev.epicgames.com/documentation/fortnite/event-browser-in-fortnite-creative).

### Contextual Filtering

Some devices are affected by a feature called contextual filtering. This feature hides or displays options depending on the values selected for certain related options. This feature will reduce clutter in the Customize panel and make options easier to manage and navigate.

However, it may not be easy to recognize which options or values trigger contextual filtering. To help you identify them, in our device docs we use *italic* for any values that trigger contextual filtering. All options will be listed, including those affected by contextual filtering; if they are hidden or displayed based on a specific option's value, there will be a note about that in the Description field for that option.

### Device Options

The device options determine the value limits for the number rolled, the winning value, and other details of the device's appearance and behavior.

In its [default](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#default) state, this device rolls a number from 1 to 6 when the player steps onto it. Its default outcome does nothing, since no signals are transmitted unless options are set.

Default values are in **bold**. Values that trigger contextual filtering are *italic*.

#### Basic Options

**אפשרויות, ערכים ותיאורים:**

##### Value Limit 1

- **Value / Values:** **0**, Pick a number
- **Description:** Defines the minimum number the device can roll.

##### Value Limit 2

- **Value / Values:** **6**, Pick a number
- **Description:** Defines the maximum number the device can roll.

##### Winning Value

- **Value / Values:** **4**, Pick a number
- **Description:** If the device rolls a number equal to or higher than this value, it's a win.

##### Pick Each Number Once

- **Value / Values:** **No**, Yes (Reset on Game Start), Yes (Reset on Round Start)
- **Description:** Once a number is chosen. don't choose it again until there are no more numbers to pick. The numbers will reset either on round start or game start, depending on the value set in this option.

##### Activating Team

- **Value / Values:** **Any, **Pick a number
- **Description:** Determines which Team can activate the device.

#### All Options (Additional)

**אפשרויות, ערכים ותיאורים:**

##### Roll Time

- **Value / Values:** Instant, **3 seconds**, Pick an amount of seconds
- **Description:** How long the device takes after it starts calculating to determine a result.

##### Reset After Use

- **Value / Values:** **On**, *Off*
- **Description:** Determines if the device will reset after it has been used. If false, the device will disable itself after use, and must be enabled to use again.

##### Reset Delay

- **Value / Values:** Never Reset, **Instant**, Pick an amount of time
- **Description:** The amount of time it takes for the device to be ready after it is activated. If you select **Never Reset**, the device will be disabled after it has been activated once.

##### Award Score

- **Value / Values:** **Never**, *Always*, *On Win*, *On Loss*
- **Description:** Defines when [score](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#score) is awarded.

##### Result Multiplier

- **Value / Values:** **1**, Pick a number
- **Description:** Multiplies the roll's result by the selected value. This is mainly used for awarding a Score.

##### Score Type

- **Value / Values:** **Add**, Subtract, Set
- **Description:** Defines how score is awarded.

##### Score Value

- **Value / Values:** **Roll Amount**, Pick a number
- **Description:** Defines the amount of score awarded.

##### Zone Direction

- **Value / Values:** **None**, *Forward*, *Left*, *Right*, *Backwards*
- **Description:** Determines if there is a zone associated with the device, and if there is which direction the zone lies.

##### Length

- **Value / Values:** **4**, Pick a number
- **Description:** Sets the length of the volume in tiles. This length will be split into a number of equal sections based on the number of potential outputs.

##### Width

- **Value / Values:** **Normal (1.0)**, Pick a number
- **Description:** Sets the width of the volume in tiles.

##### Height

- **Value / Values:** **Normal (1.0)**, Pick a number
- **Description:** Sets the height of the volume in tiles.

##### Visible During Game

- **Value / Values:** **Yes**, No
- **Description:** Determines whether or not the device is visible during the game.

##### Play Audio

- **Value / Values:** **Yes**, No
- **Description:** Determines whether or not the device plays a sound.

##### Activating Team

- **Value / Values:** **Any**, Pick a number
- **Description:** Determines which team can activate this device.

##### Enabled During Phase

- **Value / Values:** None, **Always**, Pre-Game Only, Gameplay Only
- **Description:** Determines which phases in which the device will be enabled. Pre-Game includes all phases prior to the game starting.

##### Activate on Game Phase

- **Value / Values:** **None**, Waiting for Players, Game Countdown, Game Start
- **Description:** Activates the device during the selected game phase.

### Direct Event Binding

Following are the direct event binding options for this device.

#### Functions

A [function](https://dev.epicgames.com/documentation/fortnite/function) listens for an event on a device then performs an action.

-
For any function, click the **option**, then **Select Device** to access and select from the **Device** dropdown menu.

-
Once you've selected a device, click **Select Event** to bind the device to an event that will trigger the function.

-
If more than one device or event triggers a function, click the **Add** button to add a line and repeat these steps.

**אפשרויות ותיאורים:**

##### Enable When Receiving From

Enables the device, allowing it to generate numbers.

##### Disable When Receiving From

Disables the device, stopping it from being able to generate numbers, and cancelling any active rolls.

##### Cancel When Receiving From

Cancels any in progress generation.

##### Activate When Receiving From

Starts generating a random number.

#### Events

An [event](https://dev.epicgames.com/documentation/fortnite/event) tells another device when to perform a function.

-
For any event, click the **option**, then **Select Device** to access and select from the **Device** dropdown menu.

-
Once you've selected a device, click **Select Function** to bind this event to a function for that device.

-
If more than one function is triggered by the event, click the **Add** button to add a line and repeat these steps.

**אפשרויות ותיאורים:**

##### On Win Send Event To

Sends an event to any linked devices when a winning score is rolled.

##### On Lose Send Event To

Sends an event to any linked devices when a losing score is rolled.

##### On Rolled Max Send Event To

Sends an event to any linked devices when the maximum score is rolled.

##### On Rolled Min Send Event To

Sends an event to any linked devices when the minimum score is rolled.

---

## Using Signal Remote Manager Devices in Fortnite Creative

**כותרת מקורית:** Using Signal Remote Manager Devices in Fortnite Creative  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/using-signal-remote-manager-devices-in-fortnite-creative  
**מקור קלט:** `07A_קלט_טריגרים_תנאים_והחלטות(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `using-signal-remote-manager-devices-in-fortnite-creative`

A **Signal Remote** is a device players can carry and use to send signals to other devices. You can use the **Signal Remote Manager** to manage how and where these signals are sent. This gives players the ability to send signals from held items [in-game](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary).

For example, a player can activate their Signal Remote to send a signal that teleports them back to their base area.

### Finding and Placing the Signal Remote Manager

[
](https://dev.epicgames.com/community/api/documentation/image/36aed0c9-0790-402e-9043-1410e39c1627?resizing_type=fit) Finding the Signal Remote Manager Device

*Click image to enlarge.*

-
From [Create mode](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary), press the **Tab** key to open the [CREATIVE inventory](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) screen.

-
Click the **DEVICES** tab. You can scroll to select the device, use the **Search** box to look up the device by name, or the **Categories** in the panel on the left.

-
Click **PLACE NOW** to [place](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) immediately, or put the device in the [QUICK BAR](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) to place later.

-
Press **Esc** to return to your island in Create mode. Use your [phone](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) to position the device, then click to place it. Press **Esc **to detach the device from your phone.

-
Point at the device with your phone. If the **CUSTOMIZE** popup doesn't open immediately, move closer until it does, then press **E** to open the Customize panel.

### Finding and Placing a Signal Remote

You need to use a Signal Remote with the Signal Remote Manager. Although it doesn't look like a weapon, the Signal Remote is found on the **Weapons** tab in the Creative inventory.

You need to grant your players a Signal Remote using a [Class Designer](https://dev.epicgames.com/documentation/fortnite/using-class-designer-devices-in-fortnite-creative), an [Item Granter](https://dev.epicgames.com/documentation/fortnite/using-item-granter-devices-in-fortnite-creative) device, or a [chest](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary). This Signal Remote can "fire" signals on two channels: a primary and a secondary.

[
](https://dev.epicgames.com/community/api/documentation/image/b8515020-582f-4341-ab83-954a8886397c?resizing_type=fit) Finding the Signal Remote

*Click image to enlarge.*

-
From **Create mode**, press the **Tab** key to open the **Creative inventory** screen.

-
Click the **WEAPONS** tab. You can scroll to find the Signal Remote, or use the **Search** box to look it up.

-
Click **EQUIP** to place the Signal Remote in your Player Equipment bar.

-
Press **Esc** or **Tab** to return to your island in Create mode.

-
Walk up to the Signal Remote Manager device. Press the **Tab** key to open Creative inventory, but this time, click **Play** in the [top navigation bar](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) to display the [Play inventory](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary).

-
Drag the Signal Remote off the [Equipment bar](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) to drop it on the Signal Remote Manager. This registers the Signal Remote with the device. It should look like the image below.

If you're using multiple copies of a device on an island, it can be helpful to [rename](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) them. You can choose names that relate to each device's purpose so it's easier to remember what each one does.

### Device Options

When you customize the options on the Signal Remote Manager, the values will affect how the Signal Remote works.

You can configure the Signal Remote Manager with the following options.

Default values are **bold**.

#### Device Options

**אפשרויות, ערכים ותיאורים:**

##### Enabled at Game Start

- **Value / Values:** **On**, Off
- **Description:** Determines whether the device is [enabled](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) at the start of the game.

##### Cooldown Time

- **Value / Values:** 3 seconds, Pick or enter an amount of time
- **Description:** Determines the length of time the [cooldown](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) lasts after you activate the Signal Remote.

##### Signal Remote Tier

- **Value / Values:** Common, **Uncommon**, Rare, Epic, Legendary
- **Description:** Determines the rarity tier of the signal remote this device is paired with.

##### Activate Events Immediately

- **Value / Values:** On, **Off**
- **Description:** Determines whether the event activates as soon as the player presses the input control.

##### Remote Sound Enabled

- **Value / Values:** **On**, Off
- **Description:** Determines whether the device should play default SFX or not.

### Direct Event Binding

[Direct event binding](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) allows devices to communicate directly, which makes your workflow more intuitive, and gives you more freedom to focus on your design ideas.

Below are the [functions](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) and [events](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) for this device.

#### Functions

Direct event binding uses functions as receivers. A function listens for one device's event to tell another device to perform a function.

 Option Select Device Select Event Description
**Enable When Receiving From**

Click the arrow to display a list of available devices.

Click the arrow to display a list of available events.

This function enables the device when an event occurs. If more than one device or event can enable this device, click **Add** to add a new line.

**Disable When Receiving From**

Click the arrow to display a list of available devices.

Click the arrow to display a list of available events.

This function disables the device when an event occurs. If more than one device or event can disable this device, click **Add** to add a new line.

#### Events

Direct event binding uses events as transmitters. An event tells another device to perform a function.

 Option Select Device Select Event Description
**On Primary Activation Send Event To**

Click the arrow to display a list of available devices.

Click the arrow to display a list of available functions.

When the player activates the Signal Remote's primary function, the device sends an event to the selected device, which triggers the selected function.

**On Secondary Fire Send Event To**

Click the arrow to display a list of available devices.

Click the arrow to display a list of available functions.

When the player activates the Signal Remote's secondary function, the device sends an event to the selected device, which triggers the selected function.

### Design Examples

Here are some examples of how you can use the Signal Remote Manager.

-
[Door Lock](https://dev.epicgames.com/documentation/fortnite/using-signal-remote-manager-devices-in-fortnite-creative)

-
[Restock Remote](https://dev.epicgames.com/documentation/fortnite/using-signal-remote-manager-devices-in-fortnite-creative)

-
[Remote Hacking](https://dev.epicgames.com/documentation/fortnite/using-signal-remote-manager-devices-in-fortnite-creative)

The Signal Remote Manager device requires one of the Signal Remote A through D weapons to be registered to it in order to transmit signals correctly. This means you can have four different Signal Remote Manager devices within the same map, one per Signal Remote weapon. Then, through either a Class Manager, Item Spawner or Item Granter, you need to give this to the player to use.

For these examples, all three use the Class Designer device. Place a Class Designer anywhere on the map and customize it with the following settings.

 Option Value Description
**Class Identifier**

1

This will be used as the default class for all examples.

**Equip Granted Item**

First Item

The Signal Remote will be automatically equipped upon spawning.

Next, go to the Game tab in your My Island settings and make sure to set the Default Class Identifier as follows. This will ensure that you spawn with the Signal Remote weapon at the beginning of each design example.

[
](https://dev.epicgames.com/community/api/documentation/image/db4ba5c4-e457-488e-b6fb-64ceb4e09188?resizing_type=fit) My Island Game Tab, Default Class Identifier

*Click image to expand.*

 Which Tab in My Island Option Value Description
Game

**Default Class Identifier**

1

This will be used as the default class for all examples.

#### Door Lock

The most basic functionality of the Signal Remote Manager device is in sending two signals — such as one to open or unlock a door, and the other to close it. This is demonstrated in the following example and video.

You will need the following devices.

-
1 x **Signal Remote Manager** and **Signal Remote** weapon

-
1 x [Lock](https://dev.epicgames.com/documentation/fortnite/using-lock-devices-in-fortnite-creative)

-
Create a wall with a door, and add the Lock device adjacent to the door. Customize the lock to the following settings.

**אפשרויות, ערכים ותיאורים:**

##### Visible During Game

- **Value / Values:** Off
- **Description:** The Lock device is not visible during gameplay.

##### Unlock When Receiving From

- **Value / Values:** Channel 1
- **Description:** The primary fire of the Signal Remote will unlock the door.

##### Lock When Receiving From

- **Value / Values:** Channel 2
- **Description:** The secondary fire of the Signal Remote will lock the door.

##### Open When Receiving From

- **Value / Values:** Channel 1
- **Description:** The primary fire of the Signal Remote will open the door.

##### Close When Receiving From

- **Value / Values:** Channel 2
- **Description:** The secondary fire of the Signal Remote will close the door.

#### -
Place a set-up Signal Remote Manager device anywhere on your island. Customize it with the following settings.

- **Value / Values:** Option Value Description
**Cooldown Time**
- **Description:** 1 Second

##### Time between transmitting signals on the Signal Remote.

- **Value / Values:** **On Primary Activation Transmit On**
- **Description:** Channel 1

##### Transmits the signal to unlock and open the door on primary fire of the Signal Remote.

- **Value / Values:** **On Secondary Fire Transmit On**
- **Description:** Channel 2

##### Transmits the signal to lock and close the door on secondary fire of the Signal Remote.

- **Value / Values:** You now have a lockable door operated by a Signal Remote weapon.
- **Description:** You can also use this game mechanic for enabling and disabling other devices. Lock a car remotely so nobody else can use it. Make walls vanish and reappear with a toggle for an advanced line of defense. These openings can be used as shortcuts on the team, and restricted to certain classes or globally used.

#### Restock Remote

You can use Signal Manager devices to set primary and secondary fire to trigger Teleporter devices. This gives players a way to restock immediately during a firefight without being eliminated, and provides a way to teleport to a central location..

You will need the following devices.

-
1 x **Signal Remote Manager** and **Signal Remote**

-
2 x [Teleporter](https://dev.epicgames.com/documentation/fortnite/using-teleporter-devices-in-fortnite-creative)

-
Multiple [Vending Machines](https://dev.epicgames.com/documentation/fortnite/using-vending-machine-devices-in-fortnite-creative)

-
Create a resupply depot and a secure place to teleport near the front lines of your arena. Place a Teleporter device inside the resupply depot. Customize it to the following settings.

 Option Value Description
**Teleporter Group**

None

There is no manually activated teleporter network for this device when you walk into it.

**Teleporter Target Group**

None

There is no manually activated targeted teleporter network for this device when you walk into it.

**Teleporter Rift Visible**

No

The teleporter rift is not visible during gameplay.

**Play Sound Effects**

No

The teleporter sound effects are not played when used.

**Face Player In Teleporter Direction**

Yes

The player is faced in a specific direction to make sure they are properly oriented when using the teleporter.

**Teleport To When Receiving From**

Channel 2

Teleports the player when using the alternate fire of the Signal Remote.

-
Copy the teleporter, and place a second one down in the secure front lines section of your arena. Adjust only the following setting.

**אפשרויות, ערכים ותיאורים:**

##### Teleport To When Receiving From

- **Value / Values:** Channel 1
- **Description:** Teleports the player when using the primary fire of the Signal Remote.

#### -
Populate the resupply depot with the vending machines and equipment you want, using the default device settings.

- **Value / Values:** You now have a Signal Remote weapon able to teleport the player between two different locations.
- **Description:** Game modes with longer respawns or limited lives can benefit from this method of re-engagement, where running in and being eliminated might not be the best way to get back in the fight. There can also be two assault points that a player can choose between after respawning.

#### Remote Hacking

You can use more complex interactions with a signal manager. They can be used offensively in game modes like Capture the Flag, Search and Destroy or Domination to give a unique identity to certain classes.
*
You will use the following devices.

-
1 x **Signal Remote Manager** and **Signal Remote**

-
Multiple [**Customizable Lights**](https://dev.epicgames.com/documentation/fortnite/using-customizable-light-devices-in-fortnite-creative)

-
1 x [Timed Objective Device](https://dev.epicgames.com/documentation/fortnite/using-timed-objective-devices-in-fortnite-creative)

-
Build a structure to house an objective, such as a flag or Capture Area device. Set the time of day and optionally use additional lighting such as a Skydome device to darken the map.

-
Place a Customizable Light device within the building. Customize the following settings.

 Option Value Description
**Light Intensity**

10%

Make sure to set a desired light intensity. This setting was used for demonstration purposes.

**Turn On When Receiving From**

Channel 2

Automatically turns the lights back on with a Timed Objective device a short duration after being shut off.

**Turn Off When Receiving From**

Channel 1

The Signal Remote primary fire will turn off the lights and set the automatic reboot from the Timed Objective device.

-
Duplicate the customizable light and populate the interior with copies until it is well lit.

-
Place a Timed Objective device anywhere on the island. Customize it to the following settings.

**אפשרויות, ערכים ותיאורים:**

##### Time

- **Value / Values:** 15 Seconds
- **Description:** The duration of the Timed Objective timer.

##### Timer Label Text

- **Value / Values:** Rebooting Power...
- **Description:** The HUD display for the timer being counted down.

##### Urgency Mode Start Time

- **Value / Values:** 3
- **Description:** The remaining duration before the timer countdown begins to play urgent sound effects.

##### Start When Receiving From

- **Value / Values:** Channel 1
- **Description:** The timer is begun when the primary button of the Signal Remote is hit that deactivates the lights.

##### When Completed Transmit On

- **Value / Values:** Channel 2
- **Description:** After completing, transmits a signal to turn all the Customizeable Lights back on.

#### -
Finally, place a set-up Signal Remote Manager device anywhere on your island. Customize it with the following settings.

- **Value / Values:** Option Value Description
**Cooldown Time**
- **Description:** 1 Second

##### Time between transmitting signals on the Signal Remote.

- **Value / Values:** **On Primary Activation Transmit On**
- **Description:** Channel 1

##### Transmits the signal to turn off the lights and activate the Timed Objective device automatically rebooting it.

- **Value / Values:** You have now set up a Signal Remote weapon that operates as a remote hacking device.
- **Description:** Set the cooldown time longer than 1 second. This was used for demonstration, but the actual class should have a longer cooldown. You could also combine the above elements, to open shortcuts that are normally locked and might be poorly defended. Alternatively, you can set classes to temporarily activate Sentry devices on a cooldown, which help defend the base when it is attacked.

---

## Using Skilled Interaction Devices in Fortnite Creative

**כותרת מקורית:** Using Skilled Interaction Devices in Fortnite Creative  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/using-skilled-interaction-devices-in-fortnite-creative  
**מקור קלט:** `07A_קלט_טריגרים_תנאים_והחלטות(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `using-skilled-interaction-devices-in-fortnite-creative`

Use the **Skilled Interaction** device to create skill-based interactions as mini-games for your players. Customize this device's settings to create good, perfect, or bad zones for players to target, which can trigger individual events attached to other devices.

For help on how to find the Skilled Interaction device, see [**Using Devices**](https://dev.epicgames.com/documentation/fortnite/using-devices-in-fortnite-creative).

If you're using multiple copies of a device on an island, it can be helpful to [rename](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#rename-a-device) them. You can choose names that relate to each device’s purpose, so it’s easier to remember what each one does.

### Interaction Types

You can alter this device's settings to create charge and release, timed, and quick press interactions.

#### Charge and Release

The following settings were altered to create a skilled interaction where players can press and hold a command to target good and perfect zones that grant success when hit.

[
](https://dev.epicgames.com/community/api/documentation/image/e85d0f40-909d-4b3f-a4f5-7b0b8f12878e?resizing_type=fit) Customize these settings to create the example displayed above.

#### Timed

The following settings were altered to create an interaction where players must hit a set target at the correct time.

[
](https://dev.epicgames.com/community/api/documentation/image/23caf28b-e978-4fe7-9266-c056ac928731?resizing_type=fit) Customize these settings to create the example displayed above.

#### Quick Press

The following settings were altered to create an interaction to target moving zones.

[
](https://dev.epicgames.com/community/api/documentation/image/7c4cbd2b-1996-44b1-8516-2ec5e00f3b5b?resizing_type=fit) Customize these settings to create the example displayed above.

### Single and Multiplayer

The Skilled Interaction device includes the options for single and multiplayer skill checks.

Activating one of the **Queue Execution Type** options enables multiplayer quick time events. For multiplayer, if there is no room for that round, players are placed in a queue based on the order that they join. You set the queue limit with the **Maximum Queued Players** option. If there are no active players at the time of the call for interaction, then the player skips to the interaction.

[
](https://dev.epicgames.com/community/api/documentation/image/0ec2d8cf-6791-49c4-8ba1-519c76696253?resizing_type=fit) Multiplayer quick time event diagram

### Contextual Filtering

Some devices are affected by a feature called **contextual filtering**. This feature hides or displays options depending on the values selected for certain related options. This reduces clutter in the Customize panel and makes options easier to manage and navigate.

However, it may not be easy to recognize which options or values trigger contextual filtering. To help you identify them, in our device docs, we use *italic* for any values that trigger contextual filtering. All options will be listed, including those affected by contextual filtering; if they are hidden or displayed based on a specific option’s value, there will be a note about that in the Description field for that option.

### Device Options

You can configure this device with the following options.
**

Default values are **bold**. Values that trigger contextual filtering are *italic*.

**אפשרויות, ערכים ותיאורים:**

##### Header Text

- **Value / Values:** Enter text
- **Description:** Displays the main text for the interaction.

##### Description Text

- **Value / Values:** Enter text
- **Description:** Sets the text for the interaction.

##### Text Position

- **Value / Values:** **Top**, Bottom, Left, Right
- **Description:** Displays the text position relative to the meter.

##### Interaction Type

- **Value / Values:** **Normal**, Charge and Release
- **Description:** Displays the type of interaction for the device. **Normal** is an automatic animation, which triggers upon button press. **Charge and Release** animates while holding down the button and triggers upon release.

##### UI Type

- **Value / Values:** **Circular**, Pulsing, *Bar*
- **Description:** Sets the type of user interface to display. If you select Bar**, an additional option displays.

##### Meter Thickness

- **Value / Values:** **40** (for Circular), **70 **(for Pulsing), Pick or enter a value
- **Description:** This option displays if the **UI Typ**e option is set to **Circular** or **Pulsing**. Determines the thickness in pixels for the circular type.

##### Scrubber Thickness

- **Value / Values:** **4**, Pick or enter an amount
- **Description:** This option only displays if the **UI Type** option is set to **Pulsing**. Determines the thickness of the scrubber, in pixels.

##### Set Custom Size

- **Value / Values:** On, **Off**
- **Description:** This option only displays if the UI Type option is set to Pulsing. If this is set to **On**, the meter will use a custom height and width. The custom height and width can only be set using UEFN.

##### Movement Type

- **Value / Values:** **Linear**, PingPong, Wiggle
- **Description:** This option only displays if the UI Type option is set to Pulsing. Determines the movement pattern for the pulsing meter. If this is set to **Wiggle**, two additional options display below this one.

##### Wiggle Time Min

- **Value / Values:** **0.5 seconds**, Pick or enter an amount
- **Description:** Determines the minimum amount of time the meter wiggles before movement.

##### Wiggle Time Max

- **Value / Values:** **1.0 seconds**, Pick or enter an amount
- **Description:** Determines the maximum amount of time the meter wiggles before movement.

##### Widget Orientation

- **Value / Values:** Vertical, **Horizontal**
- **Description:** This option only displays if the **UI Type** option is set to **Bar**. Determines whether the meter displays horizontally or vertically.

##### Movement Speed

- **Value / Values:** **50%**, Pick or enter a value
- **Description:** Determines how fast the meter moves across the interaction in percent per second.

##### Good Zone Size

- **Value / Values:** **50%**, Pick or enter a value
- **Description:** Sets the good zone's size as a percent of the total meter.

##### Good Zone Position

- **Value / Values:** **50%**, Pick or enter a value
- **Description:** Sets the position of the good zone.

##### Position Zone Randomly

- **Value / Values:** *On*, **Off**
- **Description:** Determines whether the good zone positions itself randomly.

##### Perfect Zone Size

- **Value / Values:** **25%**, Pick or enter a value
- **Description:** Determines the perfect zone's size as a percent of the good zone.

##### Perfect Zone Position

- **Value / Values:** **50%**, Pick or enter a value
- **Description:** Determines the position of the perfect zone.

##### Allowed Team

- **Value / Values:** **Any**, Pick or enter a team number
- **Description:** Determines which team can activate the device.

##### Allowed Class

- **Value / Values:** **Any**, Pick or enter a class number
- **Description:** Determines which class can activate the device.

##### Invert Team Selection

- **Value / Values:** On, **Off**
- **Description:** If set to **Off**, only the selected team can activate the device. If set to **On**, all teams except the selected team can activate the device.

##### Invert Class Selection

- **Value / Values:** On, **Off**
- **Description:** If set to **Off**, only the selected class can activate the device. If **True**, all classes except the selected class can activate the device.

##### Interaction Label

- **Value / Values:** Enter text
- **Description:** Determines the text label shown on the input panel.

#### Additional UEFN-Only Option

 Option Values Description General
**Starts Enabled**

**True**, False

Determines whether or not the device is enabled automatically.
 UI
**Custom Widget**

**Don't Override**, Pick a widget

Select a custom widget to use for the interaction.

**Screen Anchor**

**Center**, Pick a position

Determines where on the screen the UI will align and anchor to.

**Placement Horizontal**

**0.0**, Pick or enter a position

Determines how far away from the anchor the widget will be. Negative numbers will move to the left.

**Placement Vertical**

**0.0**, Pick or enter a position

Determines how far away from the anchor the widget will be. Negative numbers will move upwards.

**Background Color**

**000000FF**, Pick a color

Sets the background color of the meter UI.

**Background Opacity**

**80%**, Pick or enter an amount

Sets the background opacity as a percentage. If set to **0%**, there will be no background shown.

**Background Corners Type**

Square, **Round**

Sets the type of background color to apply.

**Hide HUD**

**True**, False

If set to On, the game HUD will be hidden when the interaction is active.

**Active Player Color**

**FFFFFFFF**, Pick a color

Determines the color of the player actively interacting with the device.

**Waiting Player Color**

**FFFFFF99**, Pick a color

Determines the color of the player waiting to interact with the device.

**Fail Player Color**

**E33243FF**, Pick a color

Determines the color of a player who fails the interaction.

**Success Player Color**

**21FE99FF**, Pick a color

Determines the color of a player who succeeds the interaction.

**Show Player List**

True, False

Displays the list of players interacting with the device.

**Persist UI Duration**

**0.0 seconds**, Pick or enter an amount

Determines how long the interaction UI remains onscreen after a success or failure.

**Hide UI When**

**Player Interaction Complete**, All Interactions Complete.

Determines what condition must be met for the interaction UI to be hidden.

-
**Player Interaction Complete**: UI is hidden when the active player's interaction is succeeded or failed.

-
**All Interactions Complete**: UI is hidden when all players in the queue succeed or fail the interaction.

 Device
**Perfect Input Behavior**

**Instant Success**,** **Counts For Two, No Special Behavior

Determines what should happen when a perfect input occurs.

**Speed Up on Subsequent Interacts**

**Off**, Pick or enter a value

Determines how much to speed up on subsequent successful interactions. Resets when the device is retriggered.

**Shrink Zones on Subsequent Interacts**

**Off**, Pick or enter a value

Determines how much to shrink the zone on subsequent interactions. Resets when the device is retriggered.

**Success Target**

**None**, 1, 2, 3, 4, 5

Sets how many successful inputs are required for the minigame to complete.

**Show Successes**

True, **False**

Determines whether to display the success counter on screen.

**Success Counter Icon**

Small Checkmark, Large Checkmark, Select another icon

Determines the icon to use for the Success Target indicator.

**Success Counter Color**

**FFFFFFFF**, Pick a color

Determines the color of the Success Target indicator.

**Failure Limit**

*None*, **1**, 2, 3, 4, 5

Determines how many times a bad input can be provided before failing the minigame. If this is set to 0 (None), an additional option is available.

**Show Failures**

True, **False**

This option is only available if the **Failure Limit** option is set to **0 (None)**. Determines whether to display the fail counter on screen.

**Fail Counter Icon**

**X**, Pick an icon

Determines the icon to use for the Fail Limit indicator.

**Clear Successes on Fail**

True, **False**

If this is set to True, the Interaction Success Count resets on a bad input.

**Lock Out on Fail Time**

0.0 seconds, **1.0 seconds**, Enter an amount

If a bad input is provided, the interact will lock for the amount of time set. Set to 0 to disable this function.

**Waiting Icon**

Small None Icon, Large None Icon, Select another icon

Determines the icon to use for the waiting player indicator.

**Waiting Icon Color**

**FFFFFFFF**, Pick a color

Determines the color of the waiting player indicator icon.

**Active Icon**

Small Hourglass icon, Large Hourglass icon, Select another icon

Determines the icon to use for the active player indicator.

**Active Icon Color**

**FFFFFFFF**, Pick a color

Determines the color of the active player indicator icon.
 Meter
Meter Custom Width

**72**, Pick or enter a value

This only displays if you have set the Set Custom Size option to On. Determines the width of the meter.

**Meter Custom Height**

**72**, Pick or enter a value

This only displays if you have set the **Set Custom Size** option to **On**. Determines the height of the meter.

Meter Color

**0044CBFF**, Pick a color

Determines the meter's color.

Scrubber Color

**FFFFFFFF**, Pick a color

Determines the color of the meter scrubber.
 Zones
Good Zone Color

**5CAAFFFF**, Pick a color

Determines the good zone's color.

Perfect Zone Color

**32EDFEFF**, Pick a color

Determines the color of the perfect zone.
 Timer
**Interact Time Limit**

**0.0 seconds**, Pick or enter a value

Sets how long the player has to complete the interaction. Taking too long will result in failure.

**Show Timer**

**True**, False

If this is set to **True**, the timer will display on the screen.

**Timer Position**

**Top**, Bottom

Sets the timer's position.

**Timer Color**

**FFFFFFFF**, Pick a color

Determines the timer's color.

**Timer Size**

**Normal**, Large

Determines the timer's size.

**Timer Background Type**

None, **Transparent**, Opaque

Sets the transparency level of the timer's background.
 Sound
Interact Complete Sound

Pick a sound

Sets the sound that plays when the minigame is completed successfully.

Interact Failure Sound

Pick a sound

Sets the sound that plays when the minigame is completed unsuccessfully.

**Interact Interrupted Sound**

Pick a sound

Sets the sound that plays when the minigame is interrupted.

**Good Input Sound**

Pick a sound

Sets the sound that plays when a player hits within the success zone.

**Perfect Input Sound**

Pick a sound

Sets the sound that plays when a player hits within the perfect zone.

**Bad Input Sound**

Pick a sound

Sets the sound that plays when a player hits outside the success zone.

**Minigame Start Sound**

Pick a sound

Sets the sound that plays when the minigame starts.

**Minigame Looping Sound**

Pick a sound

Sets a looping sound that plays during the interaction.

**Looping Audio Pitch Multiplier**

**1.0**, Pick or enter a multiplier

Sets a pitch multiplier for the looping sound. This will increase by the selected amount each time a player gets a successful or perfect interaction. It will reset when the minigame is restarted.
 Queue
**Allow Duplicate Player Entries **

**True**, False

Determines if a player can make duplicate entries in the queue. Useful for re-initiating skill checks without restarting the quick time event.

**Next in Queue Delay**

**3.0 seconds**, Pick an amount

Sets the time between a player finishing an interaction and starting a new interaction with the next player in the queue.

**Queue Execution Type**

**None**, Synchronous, Random, Sequential

Sets the order for completing the quick time event.

-
Synchronous: Plays the skill check at the same time.

-
Random: Plays the skill check for one player.

-
Sequential: Plays the skill check in the order players joined.

**Synchronous Player Limit**

**5**, Enter a number

Sets the max number of players completing the skill check at the same time. This skips any duplicate entries.

**Maximum Queued Players**

**20**, Enter a number

Sets the total number of players that can join the queue for the event.

### Direct Event Binding

Following are the [direct event binding](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#direct-event-binding) options for this device.

#### Functions

A [function](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#function) listens for an event on a device and then performs an action.

-
For any function option, click the **option**, then **Select Device** to access and select from the **Device dropdown menu**.

-
Once you've selected a device, click **Select Event** to bind the timer to an event that will trigger the device's function.

-
If more than one device should be affected by a function, press the **Add** button and repeat.

**אפשרויות ותיאורים:**

##### Begin Interaction for Instigator

Activates the interaction for the instigating player.

##### End Interaction for Instigator

Deactivates the interaction for the instigating player.

##### Enable

Enables the device on triggered.

##### Disable

Disables the device on triggered.

#### Events

An [event](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#event) tells another device when to perform a function.

-
For any event option, click the **option**, then **Select Device** to access and select from the **Device dropdown menu**.

-
Once you've selected a device, click **Select Function** to bind the timer to that device's function.

-
If more than one device is affected by the function, press the **Add** button and repeat.

**אפשרויות ותיאורים:**

##### On Interact Success Transmit Event

Sets the event when the interaction is successful.

##### On Interact Fail Transmit Event

Sets the event when the interaction is failed, either because of bad inputs or timeout.

##### On Interact Bad Input Transmit Event

Sets the event when the player provides abad input.

##### On Interact Good Input Transmit Event

Sets the event when the player provides a good input.

##### On Interact Perfect Input Transmit Event

An event occurs when the player provides a perfect input.

##### On Interact Interrupted Transmit Event

An event occurs when the interaction is interrupted, either due to player elimination, manual deactivation, or disabled.

##### **On Interact Started **Transmit Event

When an interaction is started, an event occurs.

##### On Removed Agent From Queue ****Transmit ****Event

An event occurs when an agent is removed from the queue for the interaction.

##### On Queue Agent Transmit Event

An event occurs when an agent enters the queue.

##### On Advance Agent From Queue Transmit Event

An event occurs when an agent moves up in the queue.

##### On Group Interact Success Transmit Event

An event occurs when all members of a group succeed on an interaction.

##### On Group Interact Failed Transmit Event

An event occurs when all members of a group fail an interaction.

##### On All Interactions Complete Transmit Event

An event occurs when all players in the queue have completed the interaction.

---

## Using Switch Devices in Fortnite Creative

**כותרת מקורית:** Using Switch Devices in Fortnite Creative  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/using-switch-devices-in-fortnite-creative  
**מקור קלט:** `07A_קלט_טריגרים_תנאים_והחלטות(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `using-switch-devices-in-fortnite-creative`

There are two ways you can use a **Switch**.

-
As a physical switch that players can interact with, used with other devices so that players can open and close doors or turn lights off and on. If the Switch is made invisible, you can also use it to add interactivity to a prop!

-
As a method for filtering interactions with other devices. For example, if the state of the Switch is **On**, it send an event, and if the Switch is **Off**, it will send a different event.

To find the Switch device, see [Using Devices](https://dev.epicgames.com/documentation/fortnite/using-devices-in-fortnite).

### Contextual Filtering

Some devices are affected by a feature called **contextual filtering**. This feature hides or displays options depending on the values selected for certain related options. This feature will reduce clutter in the Customize panel and make options easier to manage and navigate.

However, it may not be easy to recognize which options or values trigger contextual filtering. To help you identify them, any values that trigger contextual filtering are in *italic*. All options will be listed, including those affected by contextual filtering; if they are hidden or displayed based on a specific option's value, there will be a note about that in the Description field for that option.

### Device Options

This device has some basic functionality, like setting switch visibility, and choosing what text the player sees when they interact with the switch. Additionally, there are some advanced options that you can use if the switch is able to save its state.

You can configure this device with the following options.

Default values are **bold**. Values that use contextual filtering are in *italics*.

 Option Value Description
**Enabled at Game Start**

**Yes**, No

Determines whether the device is [enabled](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) when the game starts. Disabled devices ignore all events except Enable.

**Initial State**

**Off**, On

This is the default starting state of the switch when there is no player-sourced state to override it.

**Visible During Game**

**Yes**, No

Determines whether the device is visible to players during the game.

**Turn On Text**

Enter text into field

Sets the text that displays when turning the Switch to the On position. The text field has a 150 character limit.

**Turn Off Text**

Enter text into field

Sets the text that displays when turning the Switch to the Off position. The text field has a 150 character limit.

**Device Model**

**Default**, Antique Lever, Toggle Switch, Default (Unlit), Antique Lever (Unlit), Red Button, Circuit Breaker, Ancient Lever, Checkbox

This is the visual model used for the switch.

**Sound**

**Enabled**, Disabled

Determines whether the switch makes a sound when it changes state (from Off to On, from On to Off).

**Allow Interaction**

**Yes**, No

Determines whether players can interact with the device.

**Interaction Time**

**Instant**, Pick or enter an amount of seconds

Determines how long the player interaction must be to activate the device.

**Limit Times Can Change**

**No**, *Yes*

Determines there is a limit to how many times the device can change. If this is set to **Yes**, an additional option displays below this one.

**Times Can Change**

**1**, Pick or enter a number

Determines the number of times the device can be toggled before it is disabled.

**Infinite Cooldown**

***No***, Yes

Determines the cooldown time between interactions with the device. If you set this to **Yes**, the **Cooldown Time** option does not display below this one.

**Cooldown Time**

**Instant**, Pick an amount of seconds

This option only displays when the **Infinite Cooldown** option is set to **No**. Determines the cooldown time between interactions.

**Allowed Class**

No Class, **Any**, Pick or enter a class

Determines which class can activate the device.

**Allowed Team**

**Any**, Pick or enter a team

Determines which team can activate the device.

**Interaction Radius**

**0**, Pick or enter a radius distance

Allows players to interact by looking at any point within a radius of the specified size, rather than having to look directly at the button. Use in conjunction with the **Visibility** setting to make it appear as though players are interacting with other props.

**State Reset Time**

**No Reset**, Pick or enter an amount of time

Determines the amount of time before the device resets to its default state.

**Mutually Exclusive**

**No Exclusivity**, Pick a number

Turning this switch to **On** will turn off any other switches that have the same Mutually Exclusive index number.

**Store State Per Player**

Yes, **No**

If this is set to **Yes**, each player will have their own switch state. If this is set to **No**, all players have the same switch state. If this is set to **No** and the **Use Persistence** option is set to **Use**, the switch will use the **Resolve Conflicts** option when the state attempts to load.

**Use Persistence**

**Do Not Use**, *Use*

Whether or not this device should load any data from the backend. If you choose **Use**, additional options are displayed in the All Options tab.

**Auto-Save**

Yes, **No**

This option only displays if the **Use Persistence** option is set to **Use**. Determines whether the switch state is automatically saved when it changes.

**Auto-Load**

On, **Off**

This option only displays if the **Use Persistence** option is set to **Use**. Determines whether the switch state is automatically loaded at Game Start, or if it must be loaded using event binding.

**Resolve Conflicts**

First Player, **Majority**, Prioritize On, Prioritize Off

This option only displays if the **Use Persistence** option is set to **Use**. Determines what happens when the state is loaded and the **Store State Per Player** option is set to **No**.

Values for this option:

-
**First Player**: The switch loads the state of the oldest active player.

-
**Majority**: The switch loads the state that is the most prevalent, with ties using the **Initial State** option's value.

-
**Prioritize On**: The switch loads the **On** state if at least one player has that state.

-
**Prioritize Off**: The switch loades the **Off** state if at least one player has that state.

**Check State at Game Start**

**Enabled**, Disabled

Determines if the switch will check its state at Game Start, triggering the **On Check Result On** or **On Check Result Off** events.

**Check Switch State When Disabled**

Yes, **No**

Determines whether the device will check its state even when it is disabled.

### Direct Event Binding

Direct event binding allows devices to communicate directly, which makes your workflow more intuitive, and gives you more freedom to focus on your design ideas.

Below are the following direct event binding options for this device.

#### Functions

A [function](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) listens for an event on a device then performs an action.

-
For any function, click the **option**, then **Select Device** to access and select from the **Device dropdown menu**.

-
Once you've selected a device, click **Select Event** to bind the device to an event that will trigger the function for the device.

-
If more than one device or event triggers a function, press the **Add** button to add a line and repeat these steps.

**אפשרויות ותיאורים:**

##### Enable When Receiving From

This function enables the device when an event occurs.

##### Disable When Receiving From

This function disables the device when an event occurs.

##### Turn On When Receiving From

This function turns the switch on when an event occurs.

##### Turn Off When Receiving From

This function turns the switch off when an event occurs.

##### Toggle State When Receiving From

This function toggles the switch when an event occurs.

##### Load State When Receiving From

This function loads the switch's state when an event occurs.

##### Save State When Receiving From

This function saves the switch's state when an event occurs.

##### Check State When Receiving From

This function checks the state of the switch when an event occurs.

##### Clear Player Persistence When Receiving From

This function clear's the instigating players persistence data when an event occurs.

##### Clear All Persistence Data For Current Players When Receiving From

This function clears all persistence data for all current players when an event occurs.

##### Save State For All When Receiving From

This function saves the switch state for all players when an event occurs.

##### Load State For All When Receiving From

This function loads the switch state for all players when an event occurs.

#### Events

Direct event binding uses events as transmitters. An event tells another device to perform a function.

-
For any event option, click the **option**, then **Select Device** to access and select from the **Device dropdown menu**.

-
Once you've selected a device, click **Select Function** to bind this event to a function for that device.

-
If more than one function is triggered by the event, click the **Add** button to add a line and repeat these steps.

**אפשרויות ותיאורים:**

##### On Turned On Send Event To

When the switch is turned on, an event is sent to the selected device, which triggers the selected function.

##### On Turned Off Send Event To

When the switch is turned off, an event is sent to the selected device, which triggers the selected function.

##### On Check Result On Send Event To

If the switch is on when the state is checked, an event is sent to the selected device, which triggers the selected function.

##### On Check Result Off Send Event To

If the switch is off when the state is checked, an event is sent to the selected device, which triggers the selected function.

##### On State Save Send Event To

When the switch state is saved, an event is sent to the selected device, which triggers the selected function.

##### On State Changes Send Event To

When the switch's state changes, an event is sent to the selected device, which triggers the selected function.

##### On State Load Send Event To

When the switch's state is loaded, an event is sent to the selected device, which triggers the selected function.

##### On Cleared Send Event To

When the switch's persistence data is cleared, an event is sent to the selected device, which triggers the selected function.

### Using Switch in Verse

You can use the code below to control a Switch device in [Verse](https://dev.epicgames.com/documentation/en-us/uefn/learn-programming-with-verse-in-unreal-editor-for-fortnite). This code shows how to use events and functions in the Switch device API. Modify it to fit the needs of your experience.

using { /Fortnite.com/Devices }
using { /Verse.org/Simulation }
using { /UnrealEngine.com/Temporary/Diagnostics }

## A Verse-authored creative device that can be placed in a level
switch_device_verse_example := class(creative_device):

 # Reference to the Switch Device in the level.
 # In the Details panel for this Verse device,
 # set this property to your Switch Device.

Expand code Copy full snippet(48 lines long)

To use this code in your UEFN experience, follow these steps.

-
Drag a Switch device onto your island.

-
Create a new Verse device named **switch_device_verse_example**. See [Create Your Own Device Using Verse](https://dev.epicgames.com/documentation/en-us/uefn/create-your-own-device-in-verse#creatinganewdevicewithverse) for steps.

-
In Visual Studio Code, open **switch_device_verse_example.verse** in Visual Studio Code and paste the code above.

-
Compile your code and drag your Verse-authored device onto your island. See [Adding Your Verse Device to Your Level](https://dev.epicgames.com/documentation/en-us/uefn/create-your-own-device-in-verse#addingyourversedevicetoyourlevel) for steps.

-
Add a reference for the Switch device on your island to your Verse device. See [Adding a Verse Reference to a Creative Device in Your Level](https://dev.epicgames.com/documentation/en-us/uefn/customize-device-properties-in-verse#addingaversereferencetoacreativedeviceinyourlevel) for steps.

-
Save your project and click **Launch Session** to playtest.

#### Switch Device Verse API

See the [switch_device API Reference](https://dev.epicgames.com/documentation/en-us/uefn/verse-api/fortnitedotcom/devices/switch_device) for more information on using the Switch device in Verse.

---

## Using Timer Devices in Fortnite Creative

**כותרת מקורית:** Using Timer Devices in Fortnite Creative  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/using-timer-devices-in-fortnite-creative  
**מקור קלט:** `07A_קלט_טריגרים_תנאים_והחלטות(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `using-timer-devices-in-fortnite-creative`

The **Timer device** provides a way for players to keep track of the time something has taken, either for scoreboard purposes or to trigger actions. It can be configured in several ways, and act either as a countdown to an event that is triggered at the end, or as a stopwatch for an action that needs to be completed before a set time runs out.

To find the Timer device, see the instructions in [Using Devices](https://dev.epicgames.com/documentation/fortnite/using-devices-in-fortnite).

### Timer States

The Timer device has different **states** it can be in at different times. The possible states are listed below, with descriptions. Some options move the device from one state to another, or trigger an action when the device enters a particular state.

 Timer State Description
**Start**

If a timer is **Paused**, this option will cause it to start ticking down to zero from its current time.

**Pause**

A **Paused** timer does not change time. It can be restarted.

**Reset**

When a timer is **Reset**, it sets the time remaining to the total duration and **Pauses** the timer.

**Stopped**

A **Stopped** timer does not change time. It cannot be restarted and must be reset.

**Complete**

Stops the timer and plays effects to let players know it has **completed**.

**Time-Out**

When a timer reaches zero seconds, it has **timed out** and stops counting down. This may or may not complete the timer, depending on the device settings used.

### Contextual Filtering

Some devices are affected by a feature called contextual filtering. This feature hides or displays options depending on the values selected for certain related options. This feature will reduce clutter in the Customize panel and make options easier to manage and navigate.

However, it may not be easy to recognize which options or values trigger contextual filtering. To help you identify them, in our device docs we use italic for any values that trigger contextual filtering. All options will be listed, including those affected by contextual filtering; if they are hidden or displayed based on a specific option’s value, there will be a note about that in the Description field for that option.

### Device Options

In its [default](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#default) state, the Timer device is a countdown clock. At the start of a game, the timer shows a one-minute countdown, but by default does not start counting down. You will need to adjust the device options to use it. Players can't interact directly with the device, although they can trigger it indirectly by interacting with other devices that are [bound](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#direct-event-binding) to the timer.

Configure this device with the following options.

Default values are in **bold**. Values that trigger contextual filtering are *italic*.

 Option Value Description
**Duration**

**1 minutes**, Pick an amount of time

This determines how long the timer runs.

**Timer Name**

Enter text into field

Type a name for the timer. The text field has a limit of 24 characters.

**Count Down Direction**

**Count Down**, Count Up

Determines whether the timer counts down from the **Duration** to zero, or up from zero to the **Duration**.

**Start at Game Start**

**Off**, On

Determines whether the timer starts when the game starts.

**Can Interact**

No, *Only Start*, *Only Complete*, ***Yes***

Determines if and when players can interact with the timer. If you choose **No** the **Interact Time** option does not display.

**Interact Time**

**Instant** (0), Pick a time

This option only displays if you have set the **Can Interact** option to **Yes**, **Only Complete**, or **Only Start**. Determines how long a player has to interact with the timer to start or complete the countdown.

**Activating Team**

**Any**, Pick a team number

Determines which team's players can activate the device. If you choose **Any**, any player can activate it.

**Applies To**

Player, **Everyone**

When a timer starts, this determines whether it is tracked for the activating player only, or if it is tracked for everyone. Saving and loading timers only works if this is set to **Player**.

**Success on Timer End**

**True**, False

If timer reaches the end of the countdown instead of being triggered by an event, whether this counts as a success (true) or failure (false). For example, a success would be making it to the end of the countdown for a survival-type game, but a failure for a timed-objective game.

**Completion Behavior**

Disable, **Stop**, Reset, Restart

Determines what happens when the timer finishes counting.

Values for this option are:

-
**Disable**: Puts the device into the Disabled state.

-
**Stop**: Leaves the timer in its end state, with the UI displaying success or failure; the timer cannot be restarted unless it is reset.

-
**Reset**: Returns the timer to its beginning state.

-
**Restart**: This resets the timer, then starts it again.

**Visible During Game**

Hidden, **Only Timer**, All

Determines whether players can see the device during the game.

**Timer Color**

**White**, Pick a color

If the timer is visible, this determines what color the timer is. Click the arrow to display a color picker.

**Display Time In**

**Minutes:Seconds**, Seconds Only

Determines if the time is displayed in minutes and seconds, or only in seconds.

**Timer Not Started Text**

Enter text into field

Type the text players will see if the timer is enabled, but has not started. This is displayed before the timer has begun for the first time, or after a reset. The text field has a limit of 24 characters.

**Timer Running Text**

Enter text into field

Type the text players will see if the timer is running. The text field has a limit of 24 characters.

**Paused Text**

Enter text into field

Type the text players will see if the timer is paused. The text field has a limit of 24 characters.

**Success Score Value**

**0**, Pick a positive or negative number

If the the **Result On Timer End** option is set to **Success**, the timer adds this much score.

**Failure Score Penalty**

**0**, Pick a positive or negative number

If the the **Result On Timer End** option is set to **Failure**, the timer adds this score penalty.

**Score Per Second Remaining**

**0**, Pick a positive or negative number

The timer awards the selected amount of score for each second remaining on the timer.

**Show on HUD**

**Yes**, No

Determines whether a running timer is displayed in the HUD.

**Timer Label Text Style**

**Default**, Bold, Pick a style

Sets the style for the countdown and any secondary text the timer has.

**Use Persistence**

Yes, **No**

Determines whether the timer state can be saved and loaded. If you set this option to **Yes**, additional options are displayed. This can only be set to **Yes** if **Applies To** is set to **Player**.

**Load Elapsed Time**

Yes, **No**

This option only displays if the **Use Persistence** option is set to **Yes**. If you set this option to **Yes**, when a saved timer is loaded, it will calculate the elapsed time since the timer was saved.

**Auto-Save**

**Off**, On

This option only displays if the **Use Persistence** option is set to **Yes**. Determines whether the timer is automatically saved when between game sessions, and automatically loaded when the player rejoins. If the **Save Timer** is set to **Save and Continue** the timer continues running while the player is gone, but completion behavior is delayed until the player rejoins the game.

**Auto-Load**

**On**, Off

This option only displays if the **Use Persistence** option is set to **Yes**. Determines whether the timer automatically loads when the player joins or rejoins the game. If set to **Off** the timer can only be loaded using event binding.

**Auto-Load When**

Join In Progress, **Always**

This option only displays if the **Use Persistence** option is set to **Yes**. Determines if the auto-load occurs only when the player joins a game in progress, or whether it always loads when a player joins or rejoins a game in progress.

**Enable Urgency Mode**

**Off**, On

Allows device to enter urgency mode at the time set in the **Urgency Mode Time** option. If this is set to **On** additional options display.

**Urgency Mode Time**

**Never**, Pick an amount of time

This option only displays if the **Enable Urgency Mode** option is set to **Yes**. Urgency mode begins the selected amount of time before the timer count ends.

**Urgency Text**

Enter text into field

This option only displays if the **Enable Urgency Mode** option is set to **Yes**. Type the text players will see when the timer is in Urgency Mode. The text field has a limit of 24 characters. *This option only appears when **Urgency Mode** is enabled*.

**Audio Effects**

**On**, Off

Determines whether the timer plays audio effects during the game.

**If Instigating Player Is Not Present**

**Random Player**, Empty Instigator

When an event is sent, and the original instigating player is no longer in the game, this determines which player is made the instigator.

**Set Lap Time on Success**

On, **Off**

If this is set to **On**, a lap time is set for the player whenever this timer completes successfully.

**Lap Time Style**

**Time Elapsed**, Time Remaining

When a lap time is set, you can choose to display either time elapsed (how many seconds have elapsed on the timer) or time remaining (how many seconds are left).

**Display Score Update on HUD**

**Off**, *On*

Determines whether score updates are displayed as a HUD message. If you choose **On**, several additional options are displayed.

**Reset HUD Message Score**

On, **Off**

When the device displays a score message on the HUD, this determines whether it starts at zero.

**HUD Score Update Message**

**Score!**, Enter text

Determines what message is displayed on the HUD with the score. Use the default, or enter custom text. The text field has a limit of 150 characters.

**HUD Score Update Message Score Color**

**#BFEBFFFF**, Pick a color

Determines the color of the score displayed on the HUD. Click the swatch to open the Color Picker. You can click to select a swatch, or enter a hex code in the search bar to find that color.

**HUD Score Update Message Color**

**#00BAFFFF**, Pick a color

Determines the color of the text in the message you set in the **HUD Score Update Message** option. Click the swatch to open the Color Picker. You can click to select a swatch, or enter a hex code in the search bar to find that color.

**Display Score Update if Score is 0**

On, **Off**

Determines if the Score Update displays on the HUD if the score is zero.

**Activating Class**

No Class, All, **Any**, Pick a class

If the **Applies To** option is set to **Everyone**, this determines which classes can activate the timer. If the **Applies To** option is set to **Player** the timer only starts if a player is assigned the activating class.

**Disable Timer if Failing Team or Class Check**

On, **Off**

If this is set to **On** and the **Applies To** option is set to **Everyone**, and the player who activated the timer changes to another class or team that is not allowed, the timer is disabled for everyone. If the **Applies To** option is set to **Player**, then each player with a personal timer will be monitored for class or team changes.

**Reset Timer if Failing Team or Class Check**

On, **Off**

If this is set to **On** and the **Applies To** option is set to **Everyone**, and the player who activated the timer changes to another class or team that is not allowed, the timer is reset for everyone. If the **Applies To** option is set to **Player**, then each player with a personal timer will be monitored for class or team changes.

### Direct Event Binding

Following are the [direct event binding](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#direct-event-binding) options for this device.

#### Functions

A [function](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#function) listens for an event on a device then performs an action.

-
For any function option, click the **option**, then **Select Device** to access and select from the **Device dropdown menu**.

-
Once you've selected a device, click **Select Event** and select the event that triggers this function.

-
If more than one device should be affected by a function, click the **Add** button and repeat these steps.

**אפשרויות ותיאורים:**

##### Start When Receiving From

Starts the timer when an event occurs.

##### Complete When Receiving From

Completes the timer when an event occurs.

##### Reset When Receiving From

Resets the timer when an event occurs.

##### Pause When Receiving From

Pauses the timer when an event occurs.

##### Resume When Receiving From

Resumes the timer when an event occurs.

##### Enable When Receiving From

Enables the timer when an event occurs.

##### Disable When Receiving From

Disables the timer when an event occurs. The timer pauses when disabled.

##### Start for All When Receiving From

Starts the personal timers for all players when an event occurs.

##### Pause for All When Receiving From

Pauses all personal timers when an event occurs.

##### Resume for All When Receiving From

Resumes all personal timers when an event occurs.

##### Complete for All When Receiving From

Sets all timers to a completed state when an event occurs and starts the completed behavior.

##### Reset for All When Receiving From

Resets all timers to their initial times, then stops them when an event occurs.

##### Save When Receiving From

Saves the time on the personal timer for the instigating player when an event occurs.

##### Load When Receiving From

Loads the saved time on the personal timer for the instigating player when an event occurs.

##### Clear Persistence Data When Receiving From

Clears saved data when an event occurs.

##### Clear Persistence Data for All When Receiving From

Clears saved data on all personal timers when an event occurs.

##### Set Lap Time for Player When Receiving From

Sets the lap time for for the instigating player when an event occurs.

##### Set Lap Time for All When Receiving From

Sets the lap time for all players with personal timers when an event occurs.

##### Save for All When Receiving From

Saves the time on personal timers for all players when an event occurs.

##### Load for All When Receiving From

Loads all saved times when an event occurs.

#### Events

An [event](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#event) tells another device when to perform a function.

-
For any event option, click the **option**, then **Select Device** to access and select from the **Device dropdown menu**.

-
Once you've selected a device, click **Select Function** to bind the timer to a function for that device.

-
If more than one device is affected by the function, press the **Add** button and repeat.

**אפשרויות ותיאורים:**

##### On Success Send Event To

When the timer completes or ends with success, it sends an event to the selected device, which triggers the selected function.

##### On Failure Send Event To

When the timer ends with a failure, it sends an event to the selected device, which triggers the selected function.

##### On Start Urgency Mode Send Event To

When the timer enters urgency mode, it sends an event to the selected device, which triggers the selected function.

##### On Saved Send Event To

Send an event to the selected device when timer data is saved.

##### On Loaded Send Event To

Send an event to the selected device when timer data is loaded.

##### On Cleared Send Event To

Send an event to the selected device when timer data is cleared.

### Gameplay Examples Using Timer Devices

-
[5 Rounds of Econ Lessons](https://dev.epicgames.com/documentation/fortnite/5-rounds-of-econ-lessons-in-fortnite-creative)

-
[Loo Roll Rush](https://dev.epicgames.com/documentation/fortnite/loo-roll-rush-in-fortnite-creative)

-
[Shooting Gallery](https://dev.epicgames.com/documentation/fortnite/shooting-gallery-in-fortnite-creative)

-
[Spawner 123](https://dev.epicgames.com/documentation/fortnite/spawner-123-in-fortnite-creative)

-
[Timed Door](https://dev.epicgames.com/documentation/fortnite/timed-door-in-fortnite-creative)

-
[Top Scorer In Class](https://dev.epicgames.com/documentation/fortnite/top-scorer-in-class-in-fortnite-creative)

---

## Using Trigger Devices in Fortnite Creative

**כותרת מקורית:** Using Trigger Devices in Fortnite Creative  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/using-trigger-devices-in-fortnite-creative  
**מקור קלט:** `07A_קלט_טריגרים_תנאים_והחלטות(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `using-trigger-devices-in-fortnite-creative`

**
When a **Trigger** device is triggered by a player, vehicle or [sequencer](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary), it can send a signal to another device that will initiate a specific action.

This device can be used with other devices, or alone.

For help on how to find the Trigger **device, see [Using Devices](https://dev.epicgames.com/documentation/fortnite/using-devices-in-fortnite).

### Device Options

In its default state, the trigger is set to be activated by any player, vehicle, or Sequencer. Its trigger effect is to play a sound, and by default it is not set up to trigger on a channel. However, all of this can be configured with the following options.

Default values are **bold**.

#### Basic Options

**אפשרויות, ערכים ותיאורים:**

##### Trigger Sound

- **Value / Values:** **Enabled**, Disabled
- **Description:** Determines whether a sound is played when the device is triggered.

##### Visible in Game

- **Value / Values:** **Yes**, No
- **Description:** Determines whether the device is visible during the game.

#### All Options (Additional)

**אפשרויות, ערכים ותיאורים:**

##### Activating Team

- **Value / Values:** **Any**, Pick a team
- **Description:** Can only be activated by this team.

##### Activating Class

- **Value / Values:** No Class, **Any**, Pick a class
- **Description:** Determines which [class](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#class) can activate the device.

##### Invert Class Selection

- **Value / Values:** On, **Off**
- **Description:** If set, the device will count all but the selected class.

##### Triggered by Player

- **Value / Values:** **On**, Off
- **Description:** Determines whether to trigger this channel when the player gets within the proximity of the device.

##### Triggered by Damage

- **Value / Values:** **Off**, On
- **Description:** Determines whether to trigger this channel when the object is damaged.

##### Triggered by Items

- **Value / Values:** **Off**, On
- **Description:** Determines whether to activate the trigger when an item hits it. This includes dropped items and projectiles.

##### Triggered by Vehicles

- **Value / Values:** **On**, Off
- **Description:** Determines whether to activate the trigger when a Vehicles gets within proximity of the device.

##### Triggered by Creatures

- **Value / Values:** On, **Off**
- **Description:** Determines whether or not to trigger this channel when a Creature or Wildlife gets within proximity of the device.

##### Triggered by Sequencers

- **Value / Values:** **On**, Off
- **Description:** Determines whether to activate the trigger when it is touched by Sequencer or RNG device pulse.

##### Triggered by Water

- **Value / Values:** **On**, Off
- **Description:** Determines whether or not to activate the trigger when it is touched by a Water device.

##### Triggered by Carryable Objects

- **Value / Values:** On, **Off **
- **Description:** Determines whether or not carriable objects activate the trigger.

##### Activate on Game Phase

- **Value / Values:** **None**, Game Countdown, Game Start
- **Description:** Sets the device to activate in the selected game phase.

##### Times Can Trigger

- **Value / Values:** **Off**, On, Pick a number
- **Description:** The number of times this device can trigger before being disabled.

##### Trigger Delay

- **Value / Values:** Pick a time interval
- **Description:** Determines the length of time the device will wait between being triggered and sending a signal.

##### Transmit Every X Triggers

- **Value / Values:** **1**, Pick a number
- **Description:** Sets the device to only send a signal after being triggered the specified number of times.

##### Reset Delay

- **Value / Values:** **None**, Pick a length of time
- **Description:** Specifies the length of time the device must wait after sending a signal before it can be triggered again.

##### Trigger Sound

- **Value / Values:** Disabled, **Enabled**
- **Description:** Determines whether a sound is played when the device is triggered.

##### Delayed Trigger Instigator Choice

- **Value / Values:** First, **Last**, Queue
- **Description:** Determines what happens when another player activates this trigger after it has already been activated and is waiting on a delay.

##### **First** will always send the first player that triggered this trigger.

- **Value / Values:** **Last** will always send the most recent player that triggered the trigger.
- **Description:** **Queue** will send all players that have triggered this trigger from first to last.

##### Receive Damage While Invisible

- **Value / Values:** **Do Not Take Damage**, Take Damage
- **Description:** Determines whether this object will take damage while it is hidden in a game. This will block projectiles from hitting things behind it.

##### Enabled on Game Start

- **Value / Values:** **On**, Off
- **Description:** Determines whether the device is enabled when the game starts.

#### Physics-Enabled Options

The following options become available when [Physics](https://dev.epicgames.com/documentation/fortnite/physics) are enabled in a project:

**אפשרויות, ערכים ותיאורים:**

##### Triggered by Physics Props

- **Value / Values:** On, **Off**
- **Description:** Determines whether to trigger events when a physics prop gets within range of the device.

### Direct Event Binding

Following are the direct event binding options for this device.

#### Functions

A [function](https://dev.epicgames.com/documentation/en-us/fortnite-creative/function) listens for an event on a device, and then performs an action.

**אפשרויות ותיאורים:**

##### Enable

Enables the device.

##### Disable

Disables the device.

##### Reset Times Triggered

Resets the number of times the Trigger has been activated.

##### Trigger

Activates the trigger.

#### Events

An [event](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#event) tells another device when to perform a function.

**אפשרויות ותיאורים:**

##### On Triggered

Sends an event to linked devices when the Trigger is activated.

### Gameplay Examples Using Triggers

-
[Color Switch Challenge](https://dev.epicgames.com/documentation/fortnite/color-switch-challenge-in-fortnite-creative)

-
[Loo Roll Rush](https://dev.epicgames.com/documentation/fortnite/loo-roll-rush-in-fortnite-creative)

-
[Storm Wars](https://dev.epicgames.com/documentation/fortnite/storm-wars-in-fortnite-creative)

-
[Timed Door](https://dev.epicgames.com/documentation/fortnite/timed-door-in-fortnite-creative)

---

## Using Volume Devices in Fortnite Creative

**כותרת מקורית:** Using Volume Devices in Fortnite Creative  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/using-volume-devices-in-fortnite-creative  
**מקור קלט:** `07A_קלט_טריגרים_תנאים_והחלטות(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `using-volume-devices-in-fortnite-creative`

Have you ever wanted to trigger specific devices or events for a whole area of your island? The **Volume** device is designed to help you do that. As a customizable and nestable [volume](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#volume), you can size and place multiple volumes that can trigger events or functions when a player, vehicle, creature, wildlife animal, or guard enters or leaves that volume.

There are lots of ways to use this device, but they work particularly well with the **Fixed Point Camera**, **Fixed Angle Camera**, and **Third Person Controls** devices. See [Designing with Cameras and Controls](https://dev.epicgames.com/documentation/fortnite/designing-with-cameras-and-controls-in-fortnite-creative) for more examples for how to use this device with camera and controls devices.

**Looking for a spark of creative freedom?** See [****](https://dev.epicgames.com/documentation/fortnite/down-but-not-out-device-design-example-in-fortnite-creative)**[Down But Not Out Device Design Example](https://dev.epicgames.com/documentation/fortnite/down-but-not-out-device-design-examples-in-fortnite-creative)** to liberate your imagination!

To find the Volume device, go to the Content Browser and select the **Devices** category. From there you can search or browse for the device. For more information on finding devices see [Using Devices](https://dev.epicgames.com/documentation/fortnite/using-devices-in-fortnite).

### Device Options

You can configure this device with the following options.
**

Default values are **bold**. Values that trigger contextual filtering are *italic*.

 Option Value Description
**Visible in Game**

On, **Off**

Determines whether the volume is visible during the game.

**Selected Team**

**Any**, Pick or enter a team

Determines which team is affected by the volume.

**Invert Team Selection**

On, **Off**

Determines if all teams except the selected team are affected by the volume.

**Selected Class**

**Any**, Pick or enter a class

Determines which class is affected by the volume.

**Invert Class Selection**

On, **Off**

Determines if all classes except the selected class are affected by the volume.

**Volume Shape**

**Box**, *Cylinder*, *Sphere*

Determines the shape of the volume.

When you select either Cylinde**r or **Sphere**, the **Volume Radius** option becomes available.

**Volume Width**

**1.0**, Pick or enter an amount

Determines the width of the volume, in tiles.

**Volume Depth**

**1.0**, Pick or enter an amount

Determines the depth of the volume, in tiles.

**Volume Height**

**1.0**, Pick or enter an amount

Determines the height of the volume, in tiles.

**Volume Radius**

**1.0**, Pick or enter an amount

This option is only available if the **Volume Shape** option is set to **Cylinder **or **Sphere**. Determines the radius of the volume, in tiles.

**Player Events Enabled**

**On**, Off

Determines if players trigger enter and exit events.

**Vehicle Events Enabled**

**On**, Off

Determines if vehicles trigger enter and exit events.

**External Volume**

**None**, Select an external volume

Provides a way to use a volume other than the default volume.

**Creature and Wildlife Events Enabled**

**On**, Off

Determines if creatures and wildlife trigger enter and exit events.

**Guard Events Enabled**

**On**, Off

Determines if guards trigger enter and exit events.

#### Additional UEFN Options

When you use this device in UEFN, additional user options are available.

**אפשרויות, ערכים ותיאורים:**

##### Custom Volume Mesh

- **Value / Values:** Select a volume mesh
- **Description:** Assigns a custom mesh for the volume to use, rather than a shape.

#### Physics-Enabled Options

The following options become available when the [Physics](https://dev.epicgames.com/documentation/fortnite/physics) feature is enabled in a project:

**אפשרויות, ערכים ותיאורים:**

##### Physics Events Enabled

- **Value / Values:** **On**, Off
- **Description:** Determines whether the volume triggered physics entered and exit events.

### Direct Event Binding

[Direct event binding ](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#direct-event-binding) allows devices to communicate directly, which makes your workflow more intuitive, and gives you more freedom to focus on your design ideas.

Below are the functions and events for this device.

#### Functions

This device has no functions.

#### Events

An [event](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#event) tells another device when to perform a function. In UEFN, events are not editable. In Creative, follow these steps to set an event.

-
For any event, click the **option**, then **Select Device** to access and select from the **Device** dropdown menu.

-
Once you've selected a device, click **Select Function** to bind the device to a function for that device.

-
If more than one device is affected by the event, press the **Add** button to add a line and repeat these steps.

**אפשרויות ותיאורים:**

##### On Enter Send Event To

When a valid entity enters the volume, an event is sent to the selected device, which triggers the selected function.

##### On Exit Send Event To

When a valid entity exits the volume, an event is sent to the selected device, which triggers the selected function.

##### On Physics Enter

When a physics prop enters the volume, an event is sent to the selected device, which triggers the selected function.

##### On Physics Exit

When a physics prop exits the volume, an event is sent to the selected device, which triggers the selected function.

### Using Volume Devices In Verse

You can use the code below to control a Volume device in Verse. This code shows how to use events and functions in the Volume device API. Modify it to fit the needs of your experience.

using { /Fortnite.com/Devices }
using { /UnrealEngine.com/Temporary/Diagnostics }
using { /Verse.org/Simulation }

## A Verse-authored creative device that can be placed in a level
volume_device_verse_example := class(creative_device):

 # Reference to the Volume device in the level.
 # In the Details panel for this Verse device,
 # set this property to your Volume device.

Expand code Copy full snippet(30 lines long)

To use this code in your UEFN experience, follow these steps.

-
Drag a Volume device onto your island.

-
Create a new Verse device named **volume_device_verse_example**. See [Create Your Own Device Using Verse](https://dev.epicgames.com/documentation/fortnite/create-your-own-device-using-verse-in-unreal-editor-for-fortnite) for steps.

-
In Visual Studio Code, open **volume_device_verse_example.verse** in Visual Studio Code and paste the code above.

-
Before you can drag your Verse device into the level, you have to compile your code. In the Menu Bar, go to Verse > Build Verse Code.

-
Save your project and click **Launch Session** to playtest.

#### Volume Device Verse API

See the [volume_device API Reference](https://dev.epicgames.com/documentation/en-us/fortnite/verse-api/fortnitedotcom/devices/volume_device) for more information on using the Volume device in Verse.

---

## Using Voting Group and Voting Options Devices in Fortnite

**כותרת מקורית:** Using Voting Group and Voting Options Devices in Fortnite  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/using-voting-group-and-voting-options-devices-in-fortnite  
**מקור קלט:** `07A_קלט_טריגרים_תנאים_והחלטות(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `using-voting-group-and-voting-options-devices-in-fortnite`

**
Use the Voting Group** and **Voting Options** devices to create a voting system for players in your game. These two devices work together, and you cannot use them individually. You need one Voting Options device for each available option a player can choose.

Some ways you can use this:

-
Create polls to get direct player feedback.

-
In games where players must identify an infiltrator, set up a vote for players to decide who the spy or traitor is.

-
Create an adversarial game where players periodically vote for who should stay in and who should be eliminated.

For help on how to find the Voting Group and Voting Options devices, see [Using Devices](https://dev.epicgames.com/documentation/fortnite/using-devices-in-fortnite).

If you're using multiple copies of a device on an island, it can be useful to rename them. Choosing names that relate to a device's purpose makes it easier to remember what each one does, and easier to find a specific device when using the [Event Browser](https://dev.epicgames.com/documentation/fortnite/event-browser-in-fortnite-creative).

### Using the Device

-
Decide what you want your players to vote on.

-
Place one **Voting Group** device for each vote you want players to participate in.

-
Name each Voting Group with a unique name or phrase in the Voting Group option. You can use the same name for that device.
**

For example, if the vote is for who is on what team, you could use Vote for Teams** as the Voting Group option value; then rename that Voting Group device with **Vote for Teams**.

-
Place a Voting Options device for each choice players have in a single vote (a minimum of two), and link the Voting Options devices to their specific Voting Group device.

-
Use [HUD Message](https://dev.epicgames.com/documentation/fortnite/using-hud-message-devices-in-fortnite-creative) devices or [Billboards](https://dev.epicgames.com/documentation/fortnite/using-billboard-devices-in-fortnite-creative) to give players instructions or more information about the vote.

-
Use the **Time Limit** option on the Voting Group device to limit the amount of time players have to make their decision and place their vote.
**

If you are using the Time Limit** option on the Voting Group device, the vote will end automatically when the time you set has passed. But you can also end the voting period using event binding or Verse.

-
Alternatively, use other devices to trigger the start of the voting period. Some examples of how you can do this include:

Place a **Trigger** device where a player will walk over to start the vote.

-
Define a space with a **Volume** device so that the voting period starts when a player enters that space.

-
Use a **Button** device to give players agency in when to start the vote.

-
Decide if you want gameplay events occur based on the results of the vote, and set up devices or write Verse code for that if needed.

### Voting Group Device Options

This section details the Voting Group **device options** (in Creative) or **user options** (in UEFN).

-
To customize options in Creative, approach a device and press **E** to open the **Customize** panel.

-
To customize options in UEFN, select the device in your viewport or in the Outliner. Options for this device are found in the **Details** panel, in the **User Options > Advanced** section.

**

Default values are bold**.

You can configure the Voting Group device with the following options.

**אפשרויות, ערכים ותיאורים:**

##### Voting Group

- **Value / Values:** **Default**, Enter text
- **Description:** Enter a name to identify the voting group. The **Voting Options** devices for this group need to have this name in their **Voting Group** device option.

##### Max Votes Per Player

- **Value / Values:** **1**, Pick or enter a number
- **Description:** Determines the number of times one player can vote. If this is set to a number greater than **1**, a player can vote for multiple options (but cannot switch a vote once cast). If the **Allow Vote Switching** option is set to **On** and this option is set to **1**, a player **can **change their vote after they have cast it.

##### Time Limit

- **Value / Values:** **0**, Pick or enter an amount
- **Description:** Sets a time limit for the voting period. The voting period ends when the set amount of time passes. Ending the voting period with event binding or Verse will override this option's value.

##### Setting the value to **0** means that to end the vote, you must use event binding or Verse to end the voting period.

- **Value / Values:** **Allow Vote Switching**
- **Description:** -
**Creative**: On, **Off**

#### -
**UEFN**: True (checked), **False (unchecked)**

- **Value / Values:** **
- **Description:** Determines whether a player can change their vote.

##### Poll Question**

- **Value / Values:** Enter Text
- **Description:** Optional text to display the poll question and prompt.

##### Custom Widget

- **Value / Values:** Select **class of User Widget** to display
- **Description:** The (optional) widget to display. You can bind your widget to **Device - Voting Group ViewModel **and include sub-widgets bound to **Device - Voting Option ViewModel** to update the widget automatically from this device.

### Voting Options Device Options

This section details the Voting Options device options (in Creative) or user options (in UEFN).

-
To customize options in Creative, approach a device and press **E** to open the **Customize **panel.

-
To customize options in UEFN, select the device in your viewport or in the Outliner. Options for this device are found in the **Details **panel, in the **User Options > Advanced** section.

**

 Default values are bold**.

You can configure the Voting Group device with the following options.

 Option Values Description
**Voting Group**

**Default**, Enter text

This links this Voting Options device to its corresponding **Voting Group** device.

The text in this field **must** match the text used in the **Voting Group** option in the associated **Voting Group** device.

**Voting Option Text**

Enter text

Enter a name for this voting option. It should be clear to the player what choice this option represents.

### Event Binding

Following are the functions and events for this device.

-
In **Creative**, the **functions **and **events **are customized in the **Customize **panel (like other device options).

-
In **UEFN**, you can find them in the **Details **panel under **User Options - Functions** and **User Options - Events**.

**

While you can set both functions and events in Creative (or in a Live Edit session in UEFN), you can only set functions in UEFN**, and **events are read-only**.

### Functions

A function listens for an event on a device, then performs an action.

**In Creative**, use the following steps to set a function.

-
For any function, click the option, then **Select Device** to access and select from the **Device** dropdown menu.

-
Click **Select Event** to bind the device to an event that will trigger the function for the device.

-
If more than one device or event triggers a function, click the **Add** button to add a line and repeat these steps.

**In UEFN**, use the following steps to set a function.

-
With a device selected, locate the **User Options - Functions** section in the **Details** panel, and expand it.

-
For any function, click the **+ (plus)** icon to add an array element.

-
Click the first dropdown, and select a device. If you have a lot of devices, you can use the search bar to find a device more easily.

-
Click the second dropdown, and select the event you want to bind to this function.

#### Voting Group Device Functions

**אפשרויות ותיאורים:**

##### Begin Vote When Receiving From

Begins the voting period when an event occurs.

##### End Vote When Receiving From

Ends the voting period when an event occurs.

#### Voting Options Device Functions

**Enable When Receiving From**

Enables this device when an event occurs. When the device is enabled, this option can be selected if the associated **Voting Group** device is active and the player is able to vote.

**Disable When Receiving From**

Disables this device when an event occurs. When the device is disabled, this option cannot receive any votes.

**Cast Vote When Receiving From**

Adds a vote for this option when an event occurs.

**Rescind Vote When Receiving From**

When an event occurs, subtracts a vote for this option if the instigating player voted for this option.

### Events

An event tells another device when to perform a function.
**

Events in UEFN are read-only**. They will be set automatically when you set a function on a device that binds to an event on this device.

**In Creative, follow these steps to set an event:**

-
For any function, click the option, then **Select Device** to access and select from the **Device** dropdown menu.

-
Click **Select Function** to bind this event to a function for that device.

-
If more than one function is triggered by the event, click the **Add** button to add a line and repeat these steps.

#### Voting Group Device Events

**אפשרויות ותיאורים:**

##### On Vote Begin Send Event To

When the voting period starts, an event is sent to the bound device.

##### On Vote End Send Event To

When the voting period ends, an event is sent to the bound device.

##### On Vote Tied Send Event To

When the vote is tied, an event is sent to the bound device.

#### Voting Options Device Events

**אפשרויות ותיאורים:**

##### On Voting Option Selected Send Event To

When a voting option is chosen by a player, an event is sent to the bound device.

##### On Vote Completed Winner Send Event To

When the voting period ends, if this option wins the vote an event is sent to the bound device.

##### On Voting Option Rescinded Send Event To

When a player rescinds their vote for this option, an event is sent to the bound device. This event is also triggered if a player switches their vote to another option.

##### On Failed to Vote Send Event To

When a player tries to vote, but the vote fails for any reason, an event is sent to the bound device.
