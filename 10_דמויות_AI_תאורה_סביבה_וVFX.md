# דמויות, AI, תאורה, סביבה ו־VFX

> **מטרת הקובץ:** לרכז Characters, Guards, Wildlife, AI, תאורה, מזג אוויר, סביבה ואפקטים חזותיים.  
> **מתי להשתמש בו:** כאשר מוסיפים דמויות או ישויות, מתכננים התנהגות AI או מעצבים אווירה חזותית.  
> **לא כלול:** Navigation Mesh כהליך Debug, HUD ושמע שאינו סביבתי.  
> **מקורות עיקריים:** `07F_דמויות_AI_תאורה_סביבה_וVFX(1).md`

## תוכן עניינים

- [Day Sequence Device in Fortnite Creative](#day-sequence-device-in-fortnite-creative)
- [Using AI Navigation Modification Devices in Fortnite Creative](#using-ai-navigation-modification-devices-in-fortnite-creative)
- [Using AI Patrol Path Node Devices in Fortnite Creative](#using-ai-patrol-path-node-devices-in-fortnite-creative)
- [Using Character Device Controller Devices in Fortnite Creative](#using-character-device-controller-devices-in-fortnite-creative)
- [Using Character Devices in Fortnite Creative](#using-character-devices-in-fortnite-creative)
- [Using Crowd Volume Devices in Fortnite Creative](#using-crowd-volume-devices-in-fortnite-creative)
- [Using Customizable Light Devices in Fortnite Creative](#using-customizable-light-devices-in-fortnite-creative)
- [Using Disguise Devices in Fortnite](#using-disguise-devices-in-fortnite)
- [Using Guard Spawner Devices in Fortnite Creative](#using-guard-spawner-devices-in-fortnite-creative)
- [Using Post Processing Devices in Fortnite Creative](#using-post-processing-devices-in-fortnite-creative)
- [Using Skydome Devices in Fortnite Creative](#using-skydome-devices-in-fortnite-creative)
- [Using VFX Creator Devices in Fortnite Creative](#using-vfx-creator-devices-in-fortnite-creative)
- [Using VFX Spawner Devices in Fortnite Creative](#using-vfx-spawner-devices-in-fortnite-creative)
- [Using Visual Effect Powerup Devices in Fortnite Creative](#using-visual-effect-powerup-devices-in-fortnite-creative)
- [Using Wildlife Spawner Devices in Fortnite Creative](#using-wildlife-spawner-devices-in-fortnite-creative)

---
## Day Sequence Device in Fortnite Creative

**כותרת מקורית:** Day Sequence Device in Fortnite Creative  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/day-sequence-device-in-fortnite-creative  
**מקור קלט:** `07F_דמויות_AI_תאורה_סביבה_וVFX(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `day-sequence-device-in-fortnite-creative`

**
With the **Day Sequence** device you can control the sky and edit settings for:

-
Sunlight

-
Clouds

-
Fog

-
Sky Color

-
Sun

-
Moon

-
Skylight

The **Day Sequence** device acts much like the Skydome device — you can change a number of device settings to customize how your island will look, or how it will shift through the day and night cycle.

All **Day Sequence** settings can be used in any desired combination.

The Day Sequence device only supports the **Day Night Cycle** time of day manager.

Bold, incremental changes are recommended to quickly establish a middle ground for your natural lighting. Create your project’s base lighting first with as few adjustments as possible, then work on the unique look of your project.

Establishing your base lighting with minimal adjustments means you won’t have to start from scratch with your lighting every time you make adjustments.

For help finding the Day Sequence** device, see [Using Devices](https://dev.epicgames.com/documentation/en-us/fortnite-creative/using-devices-in-fortnite-creative).

If you're using multiple copies of a device on an island, it can be helpful to [rename](https://dev.epicgames.com/documentation/en-us/fortnite-creative/fortnite-creative-glossary#rename-a-device) them. You can choose names that relate to each device's purpose, so it's easier to remember what each one does.

### Contextual Filtering

All major options listed below for the Day Sequence devices use a feature called contextual filtering. This feature hides or displays additional options when an option value is set to **On**. This feature reduces clutter in the Customize panel and makes options easier to manage and navigate.

All options are listed, including those affected by contextual filtering.

### User Options

The goal of establishing a starting point for your base lighting is to use a simple combination of settings that you can repeat in your scenes as they get more complex. The fewer settings you modify, the easier it will be later to adjust them.

In Creative, as in UEFN, there are limits on how far you can adjust the settings for your lighting and skyline.

You can configure this device with the following options:

##### General

The **Day / Night Cycle** controls the way the sun and moon will appear on your island:

-
**Default** is equivalent to choosing a random start time for your day.

-
**Fixed Time** gives you the ability to choose a fixed time of day.

-
**Start at Specified Time** starts your day at the chosen time and continues the day/night cycle.

-
**Random Fixed Time** selects a random time for each loaded session.

-
**Random Start Time** selects a random start time for each loaded session.

When working on exterior lighting, it’s important to choose your time of day first, as this affects the direction and length of your shadows, giving your map a more interesting look.

##### Trigger Volume

Instead of applying the Day Sequence device settings to the entire island, choosing a **Trigger Volume** (by checking the box and entering X, Y and Z values) will limit the lighting settings to that particular spatial location. You will only see the environmental changes when you enter this volume.

##### Sunlight

Sunlight across the island determines how shadows look, whether there are sun flares, and how light bounces off the materials in the world. Sunlight also determines how much interior and exterior lighting is necessary when you place building props.

**אפשרויות ותיאורים:**

##### Enable Sun Component

Overrides the Day / Night Cycle to set the sun to a fixed location.

##### Intensity

Sets the intensity of the light emitted by the Sun component.

##### Color

Changes the color of the sun component.

##### Enable Flare

Enables or disables lens flare when looking at the Sun.

##### Rotation Z

Rotates the sun along the Z axis (blue).

##### Rotation X

Rotates the sun along the X axis (red).

##### Fog

Control the thickness, color and falloff of the fog on your island.

**אפשרויות ותיאורים:**

##### Enable Fog Component

Enables fog.

##### Density

Modifies the fog density, which can be thought of as the fog layer's thickness.

##### Color

Changes the fog color.

##### Height Falloff

Height density factor controls how the density increases as height decreases. Smaller values make the transition larger.

##### Directional Inscattering Color

Sets the inscattering color for the fog. This is the fog's primary color.

##### Max Opacity

This controls the maximum opacity of the fog. A value of 1 means the fog will be completely opaque, while 0 means the fog will be invisible.

##### Secondary Density

The secondary fog layer's global density factor, which you can use to add another fog layer thickness.

##### Secondary Falloff

The height density factor for the secondary fog layer that controls how the density increases as height decreases. Smaller values make the transition larger.

##### Secondary Offset

The height offset relative to the Actor's Z height position in the world.

##### Sunlight Volumetric Scattering

Intensity of the volumetric scattering from the sun component.

##### Skylight

Skylight settings determine how intensely the skylight plays off the materials and props in the world. This affects how dark shadows become and how much light bounces off emissive materials.

**אפשרויות ותיאורים:**

##### Enable Skylight Component

Enables the skylight.

##### Intensity

Changes the intensity of the skylight.

##### Color

Changes the color of the skylight.

##### Sky

The Sky Atmosphere component is a physically-based sky and atmosphere-rendering technique. It's flexible enough to create an Earth-like atmosphere with time-of-day featuring sunrise and sunset, or to create extraterrestrial atmospheres of an exotic nature.

**אפשרויות ותיאורים:**

##### Enable Sky Atmosphere Component

Enables the Sky Atmosphere Component.

##### Sky Gradient Blend

Determines the blend of custom colors for your sky. 1 = all custom colors, 0 = no custom color.

##### Sky Gradient Low Color

The color of the lower part of the sky.

##### Sky Gradient Mid Color

The color of the middle part of the sky.

##### Sky Gradient High Color

The color of the upper part of the sky.

##### Sun Size

Modifies the size of the Sun disk in the sky.

##### Sun Intensity

Modifies the amount of light emanating from the Sun.

##### Sun Color

Modifies the Sun’s color.

##### Custom Sun Color Blend

Determines the blend of custom colors for your Sun component. 1 = all custom colors, 0 = no custom color.

##### Moon Size

Modifies the size of the Moon disk in the sky.

##### Moon Intensity

Modifies the amount of light emanating from the Moon.

##### Moon Color

Modifies the Moon’s color.

##### Moon Halo Size

Changes the size of the Moon’s halo.

##### Moon Halo Intensity

Changes the intensity of the Moon’s halo.

##### Star Brightness

Changes the brightness of stars in the night sky.

##### Clouds

Clouds can create ambience and alter how the lighting in the world looks due to the volume of clouds in the sky. This can result in more shadows all around, deeper shadow colors in existing shadows, and less visible sky.

**אפשרויות ותיאורים:**

##### Light Color

Changes the color for the parts of the clouds hit by sunlight.

##### Shadow Color

Changes the color of the darker parts of the clouds.

##### Lighting Brightness

Changes how light or dark clouds appear.

##### Coverage

Increases or decreases overall cloud coverage.

##### Size

Changes the size of the clouds.

##### Opacity

Changes the thickness of the clouds

##### Speed

Changes the speed at which the clouds pass overhead.

##### Direction X

Changes the direction of the clouds.

##### Direction Y

Changes the direction of the clouds.

### Direct Event Binding

Following are the [direct event binding](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) options for this device.

#### Functions

A [function](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) listens for an event on a device then performs an action.

-
For any function, click the **option**, then **Select Device** to access and select from the **Device** dropdown menu.

-
Once you've selected a device, click **Select Event** to bind the device to an event that will trigger the function for the device.

-
If more than one device or event triggers a function, click the **Add** button to add a line and repeat these steps.

**אפשרויות ותיאורים:**

##### Enable When Receiving From

Enables the device when an event occurs.

##### Disable When Receiving From

Disables the device when an event occurs.

##### Fade In When Receiving From

Gradually fade in the effects of the device.

##### Fade Out When Receiving From

Gradually fade out the effects of the device.

#### Events

This device has no events.

---

## Using AI Navigation Modification Devices in Fortnite Creative

**כותרת מקורית:** Using AI Navigation Modification Devices in Fortnite Creative  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/using-ai-navigation-modification-devices-in-fortnite-creative  
**מקור קלט:** `07F_דמויות_AI_תאורה_סביבה_וVFX(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `using-ai-navigation-modification-devices-in-fortnite-creative`

**
The **AI Navigation Modification** device creates a volume or zone that defines where [AI](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) enemies cannot access.

You can use this device to control which areas AI enemies can enter and which they are excluded from. You can even dynamically change spaces where AI enemies can enter or patrol. This device can also help you route paths around complex geometry that AIs have difficulty navigating.

Some examples of how you might use this device are:

-
You have AI enemies patrolling where there is a hazardous area, and you want the AI to avoid that hazard so they don't take damage from it.

-
You want to give or take away AI enemy access to a particular area in your island based on a specific event or other trigger.

 For help on how to find the AI Navigation Modificatio****n **device, see [Using Devices](https://dev.epicgames.com/documentation/en-us/fortnite-creative/using-devices-in-fortnite-creative).

If you're using multiple copies of a device on an island, it can be helpful to [rename](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) them. You can choose names that relate to each device's purpose, so it's easier to remember what each one does.

### Device Options

This device has some basic functionality, like selecting the height, width and depth of the [volume](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary). Additionally, there are some advanced options, like choosing the shape for the volume and deciding when the device is enabled.

You can configure this device with the following options.

Default values are **bold**.

 Option Value Description
**Barrier Depth**

**1.0**, Pick or enter a number

Determines the depth of the volume, in [tiles](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary).

**Barrier Width**

**1.0**, Pick or enter a number

Determines the width of the volume, in tiles.

**Barrier Height**

**1.0**, Pick or enter a number

Determines the height of the volume, in tiles.

**Navigation Modification Type**

**Block**, Avoid

Determines how the volume modifies AI navigation:

-
**Block**: All navigation data is removed from the volume.

-
**Avoid**: AI can leave the volume, but cannot move into the volume. This results in AI avoiding the space defined by the volume.

Zone Shape

Box, Cylinder

Determines the shape of the volume.

Enabled on Game Start

Enabled, Disabled

Determines whether the device is enabled when the game starts.

### Direct Event Binding System

**Direct event binding** allows devices to communicate directly, which makes your workflow more intuitive, and gives you more freedom to focus on your design ideas.

This device has no events or functions.

---

## Using AI Patrol Path Node Devices in Fortnite Creative

**כותרת מקורית:** Using AI Patrol Path Node Devices in Fortnite Creative  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/using-ai-patrol-path-node-devices-in-fortnite-creative  
**מקור קלט:** `07F_דמויות_AI_תאורה_סביבה_וVFX(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `using-ai-patrol-path-node-devices-in-fortnite-creative`

Use the **AI Patrol Path Node** device to create simple or complex patrolling behavior for guards spawned with the [Guard Spawner device](https://dev.epicgames.com/documentation/fortnite/using-guard-spawner-devices-in-fortnite-creative).

Place the device where you want to start a [patrol path](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary). Using your phone tool, place additional [nodes](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) (points) to mark the patrol path (use the [hotkey](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) control for placing or copying). The nodes will all be connected by a colored line, which will have directional arrows based on the patrol behavior you choose in the device options. You can use the phone tool to remove a node by using the control for cutting or deleting. See the image below for an example.

*The Copy and Cut hotkeys change to Append Node and Move Node when you're working with this device.*

Paths can be straight or curved, and can go up and down stairs or slopes. You can create many different patrol paths, and set other devices to send signals that cause guards to switch from one path to another.

Some devices have a limit on how many times that device can be placed on an island. This is independent of how much [memory](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) the device uses. You can place up to **128 AI Patrol Path Node devices** on your island. For **each device**, you can set **up to 128 individual path nodes**.

 For help on how to find the Advanced Storm Controller Beacon device, see [Using Devices](https://dev.epicgames.com/documentation/en-us/fortnite-creative/using-devices-in-fortnite-creative).

If you're using multiple copies of a device on an island, it can be helpful to [rename](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) them. You can choose names that relate to each device's purpose, so it's easier to remember what each one does.

### Device Options

This device has some basic functionality, like setting a Patrol Path Group. Additionally, there are some advanced options, like setting the next patrol path group and determining patrolling behavior.

You can configure this device with the following options.
**

Default values are **bold**.

 Option Value Description
Patrol Path Group**

**Group None**, Pick or enter a number

Set the Patrol Path Group this device belongs to.

**Next Patrol Path Group**

**Group None**, Pick or enter a number

Determines the patrol path group the AI instigator moves to when the **Go To Next Patrol Path Group When Receiving From** option is used.

**Patrol Path Ordering**

**No Order**, Pick or enter a number

Determines the order of the patrol path in its patrol path group. If set to **No Order**, the device will put the patrol path at the end. If multiple patrol paths have the same order, they will be randomly ordered between themselves.

**Enabled at Start**

**Enabled**, Disabled

Determines if the device is enabled at the start of the game.

**Patrolling Mode**

**Back and Forth**, Looping, Stop at End

Determines how the AI uses the Patrol Path.

Options are:

-
**Back and Forth**: The AI goes from the start node to the end node, and then goes from the end node back to the start node.

-
**Looping**: The AI goes from the start node to the end node, then returns directly to the start node.

-
**Stop at End**: the AI goes from the start node to the end node, and then stays at the end node.

**Show Path in Play Mode (Debug)**

**No**, Yes

Determines whether the patrol path is shown during the game. This option is for debugging and testing your island; it does not work with published islands.

**Show Path In Edit Mode**

**Yes**, No

Determines whether the patrol path is shown in Create mode.

### Direct Event Binding

**Direct event binding** allows devices to communicate directly, making your workflow more intuitive, and giving you more freedom to focus on your design ideas.

Below are the functions and events for this device.

#### Functions

A [**function**](https://dev.epicgames.com/documentation/en-us/fortnite-creative/fortnite-creative-glossary#function) listens for an event on a device then performs an action.

-
For any function, click the **option**, then **Select Device** to access and select from the **Device dropdown menu**.

-
Once you've selected a device, click **Select Event** and select the event that triggers this function.

-
If more than one device or event triggers a function, press the **Add** button to add a line and repeat these steps.

**אפשרויות ותיאורים:**

##### Enable When Receiving From

This function enables the device when an event occurs.

##### Disable When Receiving From

This function disables the device when an event occurs.

##### Go To Next Patrol Group When Receiving From

This function sends the AI instigator to the next patrol group. Works with the **On Node Reached** or **On Next Node Unreachable** events.

##### Go to Next Patrol Path When Receiving From

This function sends the AI instigator to the next patrol path in the patrol group. This option works with the **When Patrol Node Reach** or **When Next Patrol Path Node** in unreachable.

#### Events

Direct event binding uses events as transmitters. An event tells another device to perform a function.

-
For any event option, click the **option**, then **Select Device** to access and select from the **Device dropdown menu**.

-
Once you've selected a device, click **Select Function** to bind the event to a function for that device.

-
If more than one function is triggered by the event, press the **Add** button and repeat.

**אפשרויות ותיאורים:**

##### On Patrol Path Started Send Event To

When an AI starts a patrol path, an event is sent to the selected device, which triggers the selected function.

##### On Patrol Path Stopped Send Event To

When an AI stops using a patrol path, an event is sent to the selected device, which triggers the selected function.

##### On Node Reached Send Event To

When an AI reaches the current patrol path node, an event is sent to the selected device, which triggers the selected function.

##### On Next Node Unreachable Send Event To

When an AI is unable to reach the next patrol path node, an event is sent to the selected device, which triggers the selected function.

### Design Examples

Here are some examples of how you can use the AI Patrol Path Node device.

-
[Door Spotted](https://dev.epicgames.com/documentation/fortnite/using-ai-patrol-path-node-devices-in-fortnite-creative)

-
[Guard Hire](https://dev.epicgames.com/documentation/fortnite/using-ai-patrol-path-node-devices-in-fortnite-creative)

#### Door Spotted

The action of a guard sighting a player can send a signal to other devices. Here is an example of a mechanic that can be implemented into a game that uses this.

You will need the following devices.

-
1 x [Guard Spawner](https://dev.epicgames.com/documentation/fortnite/using-guard-spawner-devices-in-fortnite-creative)

-
3 x **AI Patrol Path Nodes**

-
1 x [Lock](https://dev.epicgames.com/documentation/fortnite/using-lock-devices-in-fortnite-creative)

-
1 x [Player Spawner](https://dev.epicgames.com/documentation/fortnite/using-player-spawn-pad-devices-in-fortnite-creative)

-
1 x [Item Granter](https://dev.epicgames.com/documentation/fortnite/using-item-granter-devices-in-fortnite-creative)

-
Create a simple hallway in an L shape, with a door at one side, and alcoves to hide in.

-
Place an AI Patrol Path Node on one end of the L-shaped structure. Customize it to the following settings.

 Option Value Description
Patrol Path Group

Group 1

The name of the AI patrol path you created.

-
Copy and paste the initial AI Patrol Path Node. Set up two more that traverse around the corner and to the end of the L-shaped hallway.

-
Set a Guard Spawner in a convenient location on the map where you can group global devices. Customize it to the following settings.

**אפשרויות, ערכים ותיאורים:**

##### Number of Guards

- **Value / Values:** 1
- **Description:** Maximum number of guards that can spawn at a time.

##### Total Spawn Limit

- **Value / Values:** 1
- **Description:** Total spawns of guards as they are eliminated.

##### Spawn Radius

- **Value / Values:** 2.5M
- **Description:** Distance from the spawner that a guard can appear.

##### Spawn On Patrol Path

- **Value / Values:** Group 1
- **Description:** The AI Patrol Path that the guards will spawn on and follow.

##### When Alerted To Player Transmit On

- **Value / Values:** Channel 2
- **Description:** When a guard identifies a player, they will send a signal to this channel.

##### When Eliminated Transmit On

- **Value / Values:** Channel 3
- **Description:** When the guard is eliminated, a signal is sent to this channel.

#### -
In front of the open door, set a Lock device and customize it to the following settings.

- **Value / Values:** Option Value Description
Initial Door Position
- **Description:** Open

##### When the match starts, the door will automatically be open.

- **Value / Values:** Open When Receiving From
- **Description:** Channel 3

##### Upon receiving the signal from eliminating the guard, the door will be opened.

- **Value / Values:** Close When Receiving From
- **Description:** Channel 2

##### Upon being sighted by the guard, the door will automatically close and lock.

- **Value / Values:** -
Within a protected alcove that has cover to block a guard's line of sight if the player crouches, place a Player Spawner. Customize it to the following settings.
- **Description:** Option Value Description
When Player Spawned Transmit On

##### Channel 1

- **Value / Values:** When the player spawns, a signal is sent to an Item Granter to award a weapon.
- **Description:** -
Place an Item Granter next to the Guard Spawner. Register an assault rifle to it, then customize it to the following settings.

#### Option Value Description
Equip Granted Item

- **Value / Values:** First Item
- **Description:** The first item registered to the Item Granter is automatically equipped on spawn.

##### Grant Item When Receiving From

- **Value / Values:** Channel 1
- **Description:** When the player initially spawns, they are awarded and equipped with the registered weapon.

##### You now have the basic functionality for having a door close and lock when a player is sighted by a guard, and unlocked when the player eliminates the guard.

- **Value / Values:** As an alternative to having a player defeat the guard, you can have a button that the player can push to unlock the door. Navigating it through stealth will then become mandatory, or a player can return after eliminating the guards and try again.
- **Description:** You could also set the device to cause all guards to go on alert, or spawn hostile Sentry devices in chokepoints, suddenly making the level significantly more dangerous.

#### Guard Hire

Guards, like other AIs such as boars and wolves, can also be recruited by the player to help them in combat.
*
You will need the following devices.

-
4 x [Guard Spawner](https://dev.epicgames.com/documentation/fortnite/using-guard-spawner-devices-in-fortnite-creative)

-
2 x **AI Patrol Path Nodes**

-
1 x [Player Spawner](https://dev.epicgames.com/documentation/fortnite/using-player-spawn-pad-devices-in-fortnite-creative)

-
Create a small T-shaped hallway with a safe spawning alcove at the bottom of the T.

-
Place the Player Spawner in the alcove, using it's default settings.

-
Place a Guard Spawner within the alcove. Customize it to the following settings.

**אפשרויות, ערכים ותיאורים:**

##### Number of Guards

- **Value / Values:** 1
- **Description:** The number of guards spawned by the device at one time.

##### Team

- **Value / Values:** Team 1
- **Description:** Set to the same team as the player's default.

##### Spawn Timer

- **Value / Values:** 1 Second
- **Description:** Guards are spawned after a one second delay.

##### Spawn Through Walls

- **Value / Values:** Off
- **Description:** The guards cannot spawn past walls within their spawn radius.

##### Spawn Radius

- **Value / Values:** 2.5M
- **Description:** The maximum distance a guard can spawn from its spawner.

##### Patrol Option

- **Value / Values:** Disable Patrol
- **Description:** Guards will stand in their initial spawn location instead of patrolling around.

##### Can Be Hired

- **Value / Values:** Yes
- **Description:** By interacting with the guards, you can have them follow you.

#### -
Copy two more of this Spawn Manager and place them all within the alcove.

- **Value / Values:** -
Place an AI Patrol Path Node on one end of the T juncture hallway. Customize it to the following settings.
- **Description:** Option Value Description
Patrol Path Group

##### Group 1

- **Value / Values:** The name of the AI patrol path for Guards to use.
- **Description:** -
Copy and place a second AI Patrol Path Node on the other end of the hallway.

#### -
Place a fourth Guard Spawner anywhere on the level, and customize it to the following settings.

- **Value / Values:** Option Value Description
Guard Type
- **Description:** Ghost

##### The physical model of the guard used.

- **Value / Values:** Number Of Guards
- **Description:** 2

##### Maximum number of guards that can be spawned at once.

- **Value / Values:** Total Spawn Limit
- **Description:** 2

##### Total number of guards that can be spawned.

- **Value / Values:** Team
- **Description:** Team 2

##### The enemy guards are set to a separate team.

- **Value / Values:** Spawn Timer
- **Description:** 1 Second

##### Time interval before spawning guards.

- **Value / Values:** Spawn On Patrol Path Group
- **Description:** Group 1

##### Guards will spawn on the patrol path and follow it instead of spawn near the guard spawner.

- **Value / Values:** You now have the basic functionality to hire guards that will fight enemy AIs — from creatures to other guards — in a player's defense.
- **Description:** Making it impossible for a player to do damage outside of using a melee weapon can make utilizing and sustaining the guards important. New guards could be recruited that despawn the old ones, with better statistics and health, gradually building up a standing army that follows the player. There can be many enemies, from creatures to animals to sentries and other guards that they will react to.

---

## Using Character Device Controller Devices in Fortnite Creative

**כותרת מקורית:** Using Character Device Controller Devices in Fortnite Creative  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/using-character-device-controller-devices-in-fortnite-creative  
**מקור קלט:** `07F_דמויות_AI_תאורה_סביבה_וVFX(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `using-character-device-controller-devices-in-fortnite-creative`

**Character Device Controllers** can change a group of [Character devices](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) to use the same [outfits](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary), have matching poses and animations, and have identical [emotes](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary). Use the same slot settings for multiple [Character devices](https://dev.epicgames.com/documentation/fortnite/using-character-devices-in-fortnite-creative), then associate that slot on the Character Device Controller. Each Character Device Controller can control a different group, so you can create multiple groups of Character devices, with each group looking or acting differently from the other groups.

You can also use multiple Character Device Controllers with one Character device if you want the character to look different or perform different emotes in response to events in the game.

For help finding the Character Device Controller device, see [Using Devices](https://dev.epicgames.com/documentation/en-us/fortnite-creative/using-devices-in-fortnite-creative).

### Device Options

This device has some basic functionality, like setting the Character outfit, the pose, or the emote. There are also advanced options, like setting the Character Slot number associated with this device.

You can configure this device with the following options.

Default values are **bold**.

**אפשרויות, ערכים ותיאורים:**

##### Character

- **Value / Values:** **Creative Mannequin**, Pick a character
- **Description:** When this device is triggered, it sets all associated Character devices to this character. You can choose from over 100 different characters.

##### Idle (Pose)

- **Value / Values:** **Jazz Hands 1**, Pick a pose
- **Description:** When triggered, it sets all associated Character devices to this idle pose.

##### Idle (Animated)

- **Value / Values:** **Cry**, Pick an animation
- **Description:** When triggered, it sets all associated Character devices to to perform this idle animation. This option only works if the associated Character devices have the **Use Animated Idle** option set to **Yes**. See [Character Devices](https://dev.epicgames.com/documentation/fortnite/using-character-devices-in-fortnite-creative) for more info.

##### Emote

- **Value / Values:** **Sit in Chair**, Pick an emote
- **Description:** When this device is triggered, it sets all associated Character devices to perform this emote.

##### Character Slot

- **Value / Values:** **0**, Pick a slot
- **Description:** Determines which Character Slot this device controls. All Character devices that are assigned this slot will be affected by this device. Any Character devices that are assigned to different slots will not be affected.

### Direct Event Binding

Following are the [direct event binding](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) options for this device.

#### Functions

A [function](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) listens for an event on a device then performs an action.

-
For any function, click the **option**, then **Select Device** to access and select from the **Device** dropdown menu.

-
Once you've selected a device, click **Select Event** to bind the device to an event that will trigger the function for the device.

-
If more than one device or event triggers a function, press the **Add** button to add a line and repeat these steps.

**אפשרויות ותיאורים:**

##### Change Character Appearance When Receiving From

Changes the character's appearance when an event occurs.

##### Perform Emote When Receiving From

Characters controlled by this device perform an emote when an event occurs.

##### Change Character Idle (Pose) When Receiving From

Changes the character's idle pose when an event occurs.

##### Change Character Idle (Animation) When Receiving From

Changes the character's idle animation when an event occurs.

##### Reset Characters When Receiving From

Reset all Characters that are assigned to this device's Character Slot when an event occurs.

#### Events

Direct event binding uses events as transmitters. An event tells another device to perform a function.

This device currently has no events.

---

## Using Character Devices in Fortnite Creative

**כותרת מקורית:** Using Character Devices in Fortnite Creative  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/using-character-devices-in-fortnite-creative  
**מקור קלט:** `07F_דמויות_AI_תאורה_סביבה_וVFX(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `using-character-devices-in-fortnite-creative`

A **Character** is a mannequin that you can use to create [NPC](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) characters that can interact with players in a game. You can tie its appearance or behavior to actions by a player or events caused by other devices.

 To find the Character device, see [Using Devices](https://dev.epicgames.com/documentation/fortnite/using-devices-in-fortnite).

### Contextual Filtering

Some devices are affected by a feature called **contextual filtering**. This feature hides or displays options depending on the values selected for certain related options. This reduces clutter in the Customize panel and makes options easier to manage and navigate. To help identify them, values that trigger contextual filtering are in *italic*.

All options are listed, including those affected by contextual filtering; if they are hidden or displayed based on a specific option's value, there will be a note about it in the Description field for that option.

### Device Options

This device has some basic functionality, like selecting a character and pose. There are also some advanced options, like determining the type of interaction.

You can configure this device with the following options.
**

Default values are **bold**. Values that trigger contextual filtering are *italic*.

 Option Value Description
**Character**

**Creative Mannequin**, Pick a character

Determines which character is displayed. You can choose from over 100 different characters.

**Use Animated Idle**

On, **Off**

Determines whether the character pose is animated when idle. If this is set to **On**, the **Idle (Animated)** option displays. If this is set to **Off**, the **Idle (Pose)** option displays.

**Idle (Pose)**

**Stand Tall**, Pick a pose

This option only displays when **Use Animated Idle** is set to **Off**. Determines the static pose the character uses.

**Idle (Animated)**

**Waiting**, Pick a pose

This option only displays when **Use Animated Idle** is set to **On**. Determines the animated pose the character uses.

**Emote**

**Beckon**, Pick an emote

Sets the character to use the selected emote when triggered. It plays once when triggered, without looping.

**Interact Type**

**Do Not Interact**, *Send Event Only*

Determines whether players can interact with the character. If set to **Send Event Only**, two additional options display below.

**Interaction Text**

**Interact**, Enter text in field

Type the text that the player sees into the text field. The default text is **Interact**, but you can use up to 150 characters to customize the message.

**Interact Time**

**Instant**, Pick a time in seconds

Determines how long the player must press the interact control in order to activate the character.

**Visible During Game**

**On**, Off

Determines whether the character can be seen during the game. If you want the character to appear only if certain things happen, choose **Off** and add **Turn On Visibility When Receiving From** under [Functions](https://dev.epicgames.com/documentation/fortnite/using-character-devices-in-fortnite-creative#functions).

**Character Slot**

**0**, Pick a slot

Assign this device to a Character Slot. If you use this device with a Character Device Controller, the controller can manage all Character devices with the same assigned Character Slot.

**Generate Overlap Events**

**On**, Off

Determines whether the character will generate overlap collision events with other devices.

**Random Idle Start**

On, ***Off***

Determines whether the idle should start in a random position. If set to **Off**, additional options will display.

**Initial Idle Animation Position**

**0.0**, Select a number between 0.0 and 100.0

Determines the position the character should start in. This option is only available if **Random Idle Start** is set to **Off**.

**Synchronize Animation**

On, **Off**

Determines if the character animation starts at the same time for all players, even if some are out of range when the animation starts.

**Enable Character Collision**

**On**, Off

Determines whether a character collide with other objects.

**Auto Register with Budget Allocator**

On**, Off

Allows the device to be registered or unregistered with the Animation Budget Allocator.

**Use Live Link**

*On*,** Off**

Determines whether to apply [Live Link](https://dev.epicgames.com/documentation/unreal-engine/live-link-in-unreal-engine) to the character or not.
**

Live Link Animation is only supported in the Unreal Editor for Fortnite.

Live Link Subject**

None, Select a file

Determine which Live Link Subject to get data from if Use Live Link is set to On.

### Direct Event Binding

Following are the [direct event binding](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) options for this device.

#### Functions

A [function](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) listens for an event on a device then performs an action.

-
For any function, click the **option**, then **Select Device** to access and select from the **Device** dropdown menu.

-
Once you've selected a device, click **Select Event** to bind the device to an event that will trigger the function for the device.

-
If more than one device or event triggers a function, click the **Add** button to add a line and repeat these steps.

**אפשרויות ותיאורים:**

##### Turn On Visibility When Receiving From

Shows the character device and allows interaction when an event occurs.

##### Turn Off Visibility When Receiving From

Hides the character device and disables collision when an event occurs.

##### Enable When Receiving From

Enables the device when an event occurs.

##### Play Emote When Receiving From

Plays the emote when an event occurs.

##### Disable When Receiving From

Disables the device when an event occurs.

#### Events

Direct event binding uses events as transmitters. An event tells another device to perform a function.

-
For any event option, click the **option**, then **Select Device** to access and select from the **Device** dropdown menu.

-
Once you've selected a device, click **Select Function** to bind the timer to a function for that device.

-
If more than one function is triggered by the event, click the **Add** button to add a line and repeat these steps.

**אפשרויות ותיאורים:**

##### On Interacted With Send Event To

When this device is interacted with, either by a player or another device, it sends an event to the selected device and triggers the selected function.

---

## Using Crowd Volume Devices in Fortnite Creative

**כותרת מקורית:** Using Crowd Volume Devices in Fortnite Creative  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/using-crowd-volume-devices-in-fortnite-creative  
**מקור קלט:** `07F_דמויות_AI_תאורה_סביבה_וVFX(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `using-crowd-volume-devices-in-fortnite-creative`

The **Crowd Volume** device spawns a group of [NPCs](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) that you can use for crowd scenes, concert audiences, or anywhere else you want a group of NPCs focused on a particular event. Create a race game and put cheering crowds in the stands, or a musical experience using this device to pack the audience.

This device can also improve island performance by generating a crowd without the need for placing individual characters.

 To find the Crowd Volume device, see [Using Devices](https://dev.epicgames.com/documentation/fortnite/using-devices-in-fortnite).

If you're using multiple copies of a device on an island, it can be helpful to [rename](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) them. You can choose names that relate to each device's purpose, so it's easier to remember what each one does.

### Device Options

This device has some basic functionality, like choosing the crowd density, and the size of the volume. Additionally, there are some advanced options, like making the size and facing direction of characters vary randomly.

You can configure this device with the following options.

Default values are **bold**.

**אפשרויות, ערכים ותיאורים:**

##### Character Angle Randomness

- **Value / Values:** **0%**, Pick a percentage
- **Description:** If you want characters in the volume to randomly face different directions, this determines to what degree the character angle deviates from the direction the device is facing.

##### Character Scale Randomness

- **Value / Values:** **0%**, Pick a percentage
- **Description:** If you want the characters in the volume to vary in size, this determines to what degree the size of each character deviates from the normal size.

##### Crowd Density

- **Value / Values:** **100%**, Pick or enter a percentage
- **Description:** Determines how full the volume is with characters.

##### Character Alignment

- **Value / Values:** **100%**, Pick or enter a percentage
- **Description:** Determines how precisely spawned characters are aligned on a grid.

##### Zone Width

- **Value / Values:** **1 Tile**, Pick or enter a number
- **Description:** Determines the width of the zone, in tiles.

##### Zone Depth

- **Value / Values:** **1 Tile**, Pick or enter a number
- **Description:** Determines the depth of the zone, in tiles.

##### Zone Height

- **Value / Values:** **1 Tile**, Pick or enter a number
- **Description:** Determines the height of the zone, in tiles.

##### Enabled During Phase

- **Value / Values:** None, **Always**, Pre-Game Only, Gameplay Only, Create Only
- **Description:** Determines the [phases](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) when the device is enabled. **Pre-Game Only** includes all phases prior to the game starting.

### Direct Event Binding

Following are the [direct event binding](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) options for this device.

#### Functions

A [function](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) listens for an event on a device then performs an action.

-
For any function, click the **option**, then **Select Device** to access and select from the **Device** dropdown menu.

-
Once you've selected a device, click **Select Event** to bind the device to an event that will trigger the function for the device.

-
If more than one device or event triggers a function, click the **Add** button to add a line and repeat these steps.

**אפשרויות ותיאורים:**

##### Enable When Receiving From

This function enables the device when an event occurs. Select the device and event that will enable the device. If more than one device or event can enable the device, you can click the **Add** button for this option, which adds another line.

##### Disable When Receiving From

This function disables the device when an event occurs. Select the device and event that will disable the device. If more than one device or event can disable the device, you can click the **Add** button for this option, which adds another line.

#### Events

This device has no events.

- [ ](https://dev.epicgames.com/community/search)

---

## Using Customizable Light Devices in Fortnite Creative

**כותרת מקורית:** Using Customizable Light Devices in Fortnite Creative  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/using-customizable-light-devices-in-fortnite-creative  
**מקור קלט:** `07F_דמויות_AI_תאורה_סביבה_וVFX(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `using-customizable-light-devices-in-fortnite-creative`

**

The Customizable Light device can be configured in a way that might trigger seizures for people with photosensitive epilepsy.

There are three different kinds of Customizable Lights in Creative:

-
**Customizable Light Device**: This is a light source that can be turned on or off by the player interacting with it, or by signals sent on channels. You can choose a **point light** or a **spotlight**. With this device, there is no associated prop (like a streetlamp or overhead light) that represents the source of the light.

-
**Military Light Gallery**: This gallery is a collection of customizable lights that are integrated with props such as street lights, overhead lamps, and so on.

-
**Customizable Light Gallery**: This gallery contains three customizable lights integrated with props. You can choose a torch, a spotlight, or a row of spotlights. For the row of spotlights, you can only customize one light (the rest of the row duplicates that one light).

The Military Light Gallery and Customizable Light Gallery are both found in the **Galleries** category in the Creative inventory. The Customizable Light** device is in the **Devices** category in the Content browser. This document only documents the Customizable Light device.

To find the **Customizable Light** device, see [Using Devices](https://dev.epicgames.com/documentation/fortnite/using-devices-in-fortnite).

If you're using multiple copies of a device on an island, it can be helpful to [rename](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) them. You can choose names that relate to each device's purpose, so it's easier to remember what each one does.

### Device Options

You can configure this device with the following options.

Default values are **bold**.

**אפשרויות, ערכים ותיאורים:**

##### Enabled During Phase

- **Value / Values:** None, **All**, Pre-Game Only, Gameplay Only, Create Only
- **Description:** Determines in which phases the device is enabled. **Pre-Game Only** includes all phases that occur before the game starts.

##### Initial State

- **Value / Values:** **On**, Off
- **Description:** Determines whether the light is on or off at the start of the game.

##### Light Color

- **Value / Values:** **#FFFFFF**, Pick a color
- **Description:** Determines the color of the light shining from the device. Click the color swatch to open the Color Picker. Select a color, then click the checkmark.

##### Light Intensity

- **Value / Values:** **50\%**, Pick a percentage
- **Description:** Determines the intensity of the light, as a percentage of its maximum intensity.

##### Light Reflection Intensity

- **Value / Values:** **100\%**, Pick a percentage
- **Description:** Determines the intensity of the highlights when the light reflects off shiny surfaces.

##### Light Type

- **Value / Values:** **Point Light**, Spot Light
- **Description:** A **Point Light** shines from the device in all directions. A **Spot Light** shines from the device in a cone shape.

##### Light Size

- **Value / Values:** Tiny, Small, **Medium**, Big, Huge
- **Description:** Determines the size of the light flare, range and amplitude.

##### Rhythm Preset

- **Value / Values:** **Constant**, Flicker, Wave, Short Circuit, Party, Windy, Flash
- **Description:** Determines whether the light plays a Light Rhythm, and if so what type it plays.

##### Rhythm Time

- **Value / Values:** **x4**, Pick a multiplier
- **Description:** Determines the time multiplier for the Rhythm Preset.

##### Cast Shadows

- **Value / Values:** Yes, **No**
- **Description:** Determines whether the light casts shadows. Casting shadows impacts graphics performance.

##### Dimming Amount

- **Value / Values:** **70\%**, Pick a percentage
- **Description:** Determines how much to dim the light when using channel controls.

##### Dimming Time

- **Value / Values:** **1 second**, Pick an amount of time
- **Description:** How much time it takes, in seconds, for the dimming transition to complete.

### Direct Event Binding

Direct event binding allows devices to communicate directly, which makes your workflow more intuitive, and gives you more freedom to focus on your design ideas.

Below are the following direct event binding options for this device.

#### Functions

A [function](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) listens for an event on a device then performs an action.

-
For any function, click the **option**, then **Select Device** to access and select from the **Device dropdown menu**.

-
Once you've selected a device, click **Select Event** and select the event that triggers this function.

-
If more than one device or event triggers a function, press the **Add** button to add a line and repeat these steps.

**אפשרויות ותיאורים:**

##### Enable When Receiving From

This function enables the device when an event occurs.

##### Turn On When Receiving From

This function turns on the light when an event occurs.

##### Reset When Receiving From

This function resets the light when an event occurs.

##### Disable When Receiving From

This function disables the device when an event occurs.

##### Turn Off When Receiving From

This function turns off the light when an event occurs.

##### Dim Light When Receiving From

This function dims the light when an event occurs.

##### Undim Light When Receiving From

This function undims the light when an event occurs.

##### Toggle When Receiving From

This function toggles the light off or on when an event occurs.

#### Events

This device has no events.

### Gameplay Examples Using Customizable Lights

-
[Timed Door](https://dev.epicgames.com/documentation/fortnite/timed-door-in-fortnite-creative)

---

## Using Disguise Devices in Fortnite

**כותרת מקורית:** Using Disguise Devices in Fortnite  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/using-disguise-devices-in-fortnite  
**מקור קלט:** `07F_דמויות_AI_תאורה_סביבה_וVFX(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `using-disguise-devices-in-fortnite`

###### Prerequisite topics

In order to understand and use the content on this page, make sure you are familiar with the following topics:

- [Getting Started with Devices](https://dev.epicgames.com/documentation/fortnite/getting-started-with-devices-in-fortnite)

**
You can use the Disguise** device to apply a disguise to players. Disguises are specific character [outfits](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#outfit) that change a player's appearance. You can use this device to create new types of gameplay:

-
Create stronger team identities.

-
Make more immersive roleplay mechanics.

-
Create social deduction games, where one or more players is secretly pitted against the other players.

-
Create a spy experience, where players must disguise themselves to infiltrate a location or organization.

-
Stage a jailbreak or other escape scenario, where disguises can help the players get away.

For help on how to find the **Disguise** device, see **[Using Devices](https://dev.epicgames.com/documentation/fortnite/using-devices-in-fortnite)**.

### Using the Device

Here is the general workflow for using this device.

-
Decide how players can use the disguises. Choose which disguise the device will apply, and how the disguise behaves depending on a player's actions.

-
Place the Disguise devices and determine how players will acquire the disguise.

-
If your island uses teams or classes, set which team or class is able to use the disguise applied by this device.

-
If your island has combat mechanics, set the options for how the disguise behaves when a disguised player attacks or takes damage.

 Demonstration of how Disguise device works

If you're using multiple copies of a device on an island, it can be useful to rename them. Choosing names that relate to a device's purpose makes it easier to remember what each one does, and easier to find a specific device when using the [Event Browser](https://dev.epicgames.com/documentation/fortnite/event-browser-in-fortnite-creative).

### Device Options
**

 Default values are bold**.

 Options Values Description
**Disguise to Apply**

**Default Combat - Random**, Default Casual - Random, Pick a combat or casual character

Determines what outfit the device applies to the player.

Additional characters are available for brand islands. To learn more, see the [Brand Island Characters ](https://dev.epicgames.com/documentation/fortnite/using-disguise-devices-in-fortnite#brand-island-characters-nbsp)section below.

**Disguise Breaks on Attack**

On Attack, On Damage Anything, **On Damage Opponent**, Off

Determines if the disguise comes off when the disguised player attacks.

-
**On Attack**: The disguise comes off if the disguised player initiates any attack.

-
**On Damage Anything**: The disguise comes off if the player's attack does any damage.

-
**On Damage Opponent**: The disguise comes off only if the player's attack does damage to an opponent.

**Disguise Breaks on Damage**

**On Damaged**, On Damaged By Opponent, On DBNO, On Eliminated, Off

Determines if the disguise comes off when the disguised player takes damage.

-
**On Damaged**: The disguise comes off if the disguised player takes any damage.

-
**On Damaged by Opponent**: The disguise comes off when the disguised player takes damage from a hostile entity.

-
**On DBNO**: The player's disguise only comes off if they are put into a Down But Not Out state.

-
**On Eliminated**: The player's disguise comes off if they take enough damage to be eliminated.

**Apply Disguise on Player Spawn**

-
**Creative**: On, **Off**

-
**UEFN**: True (checked), **False (unchecked)**

**

Determines if a disguise is automatically applied to a player when they spawn. This is subject to the Team to Apply To and Class to Apply To option values, if they are set.

Replace Existing Disguise**

-
**Creative**: **On**, Off

-
**UEFN**: **True (checked)**, False (unchecked)

By default, this will apply a new disguise that replaces any existing disguise the player has on. If this is set to **Off (False)**, and the player already has a disguise on, they keep their existing disguise.

**Start Enabled**

-
Creative: On, Off

-
UEFN: True (checked), False (unchecked)

Determines if the device is enabled when the game starts. If this is set to **Off (False)**, the device must be enabled using event binding or Verse.

**Team to Apply To**

**Any**, Pick or enter a team number

Determines which team the player must belong to for the disguise to be applied.

**Invert Team Filter**

-
Creative: On, **Off**

-
UEFN: True (checked), **False (unchecked)**

If this is set to **On (True)**, all teams have the disguise applied except the one set in the **Team to Apply To** option.

**Class to Apply To**

**Any**, Pick or enter a class number

Determines which class the player must have in order for the disguise to be applied.

**Invert Class Filter**

-
Creative: On, **Off**

-
UEFN: True (checked), **False (unchecked)**

If this is set to **On (True)**, all classes have the disguise applied except the one set in the **Class to Apply To** option.

### Brand Island Characters

For select brand islands, the Disguise device includes additional characters.

 Brand Characters
**Squid Game**

-
Front Man

-
Games Guard (various styles)

-
Game Manager

-
Games Player (various styles and random option)

To learn more about the feature set, see [Working With Squid Game Islands](https://dev.epicgames.com/documentation/fortnite/working-with-squid-game-islands-in-unreal-editor-for-fortnite).

*Star Wars*™

-
Civilian (various styles and random option)

-
Moon Trader (various styles and random option)

-
Rebel Trooper (various styles and random option)

-
Mandalorian (various styles)

-
Stormtrooper

-
Clone Trooper

To learn more about the feature set, see [Working With STAR WARS™ Islands](https://dev.epicgames.com/documentation/fortnite/working-with-star-wars-islands-in-fortnite).

### Functions and Events

 For more information on how events and functions work, see [Getting Started with Devices](https://dev.epicgames.com/documentation/fortnite/getting-started-with-devices-in-fortnite).
**

While you can set both functions and events in Creative (or in a Live Edit session in UEFN), you can only set functions in UEFN, and events are read-only**.

### Functions

**אפשרויות ותיאורים:**

##### Apply Disguise to Instigator When Receiving From

Applies the disguise to the instigating player when an event occurs.

##### Apply Disguise to All When Receiving From

Applies the disguise to all players when an event occurs.

##### Remove Disguise from Instigator When Receiving From

Removes a disguise applied by this device from the instigating player when an event occurs.

##### Remove Disguise from All When Receiving From

Removes a disguise applied by this device from all players when an event occurs.

##### Enable When Receiving From

Enables the device when an event occurs.

##### Disable When Receiving From

Disables the device when an event occurs.

##### Remove Any Disguise From Instigator

Removes any applied disguise from the instigating player when an event occurs.

##### Remove Any Disguise From All

Removes any applied disguises from all players when an event occurs.

### Events
**

Events in UEFN are read-only**. When you set a function on another device that binds to an event on this device, the events are set automatically.

In Creative, you can link events to functions, and functions to events.

**אפשרויות ותיאורים:**

##### On Disguise Applied Send Event To

When a player has a disguise applied from this device, an event occurs, which triggers a function on the bound device.

##### On Disguise Broken Send Event To

If a disguise applied by this device is broken, an event occurs, which triggers a function on the bound device.

##### On Disguise Removed Send Event To

If a disguise applied by this device is removed, an event occurs, which triggers a function on the bound device.

##### On Disguise Applied Any Send Event To

When any disguise is applied to a player, an event occurs, which triggers a function on the bound device.

##### On Disguise Broken Any Send Event To

When any disguise is broken, an event occurs, which triggers a function on the bound device.

##### On Disguise Removed Any Send Event To

If any disguise is removed, an event occurs, which triggers a function on the bound device.

---

## Using Guard Spawner Devices in Fortnite Creative

**כותרת מקורית:** Using Guard Spawner Devices in Fortnite Creative  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/using-guard-spawner-devices-in-fortnite-creative  
**מקור קלט:** `07F_דמויות_AI_תאורה_סביבה_וVFX(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `using-guard-spawner-devices-in-fortnite-creative`

The **Guard Spawner** can [spawn](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) a group of enemies that patrol an area to protect it from players. Like [sentries](https://dev.epicgames.com/documentation/fortnite/using-sentry-devices-in-fortnite-creative), guards have a detection system. This means players can disguise themselves or engage in stealth tactics, which gives players more strategic options for gameplay. Unlike sentries, however, guards will act as a team to attack players, or help other guards on their team.

You can determine whether players can hire guards, and if they can be hired, you can customize additional options related to hiring. You can also enable players to give commands to hired guards using the **Can Be Given Commands** option. Players can use the middle mouse button or press the left arrow on the D-pad to open the Command Wheel.

To find the Dance Mannequin device, see [Finding and Placing Devices](https://dev.epicgames.com/documentation/fortnite/using-devices-in-fortnite).

### Device Options

This device has some basic functionality, like choosing the type and number of guards, and whether guards can spawn through walls. Additionally, there are some advanced options, like how many guards are spawned and the amount of time between spawns.ou can configure this device with the following options.
**

Default values are **bold**. Values that trigger contextual filtering are *italic*.

 Option Value Description
**Guard Type**

**Shadow**, Pick a guard type, Random

Choose what type of guard will spawn. There's a wide selection to choose from.

**Spawn Count**

**4**, Pick a number

This sets the maximum number of guards this device can have active at one time. When the device activates, it will spawn one guard at a time, until it has this number of guards active. An island can only have 30 active guards spawned across all Guard Spawner devices on the island.

**Spawn Through Walls**

Yes, No

Determines whether guards must spawn within line of sight of the spawner, or whether they can spawn behind walls and inside buildings that are within range.

**Enabled at Game Start**

**Enabled**, Disabled

Determines whether the device is automatically enabled at the start of the game.

Item List**

Add Item, Remove Item from Array

The list of items associated with this device. Each array item can set an **Item Definition** and **Item Quantity**.

**Allow Infinite Spawn**

Yes, No

Determines whether the device has a spawn limit.

**Character Cosmetic**

**Don't Override**, Pick a character

Determines what character the device uses.

**Test Spawn Limit**

**1**, pick a number of respawns.

Requires **Allow Infinite Spawn** to be disabled to set this option.

Sets the maximum number of Guards this spawner can produce during its lifetime.

**Guard Team Option**

***Team Index***, Team Neutral, Team Wildlife & Creatures

Determines the team type the guards will be assigned to. If you choose **Team Index**, another option displays below this one.

**Guard Team Index**

**Team 1**, Pick a team

This option only displays if the **Guard Team Option** is set to **Team Index**. Determines which team the guards are assigned to.

**Spawn on Timer**

Yes, No

Determines if guards are spawned on the Spawn Timer countdown, or if they are spawned by events. If this is set to **On**, an additional option displays below this one.

**Spawn Timer**

**3 seconds**, Pick an amount of time

This option only displays if the **Spawn Timer** option is set to **On**. Sets the minimum amount of time between the spawn of one guard and the next. Setting this to **0** means guards spawn as quickly as possible, but this is capped by performance limits.

**Show Spawn Radius**

Yes, No

This option becomes available when **Use Device Spawn Location** is **Disabled**.

Determines if the spawn radius is shown in a preview cylinder when you are editing your island.

**Spawn Radius**

**10M**, Pick a distance

This option becomes available when **Use Device Spawn Location** is **Disabled**.

The maximum distance at which a guard can spawn.

**Use Device Spawn Location**

Yes, No

Whether the Guard should spawn on the device location instead of using the Spawn Radius. This option won't work if the Guard is set to spawn on a Patrol Path Group.

**Use Device Spawn Rotation**

Yes, No

Determines whether a guard's spawn orientation matches the device orientation. If this option is set to **Off**, the guard spawns facing the direction of the Patrol Path it spawns on.

**Play Spawn Visual Effect**

Yes, No

Determines whether a visual effect plays when a guard spawns.

**Invulnerable**

Yes, **No **

Determines if guards spawned are invulnerable or if they are damageable. If this is set to **Off**, two additional options display below this one.

**Starting Health**

**100**, Pick an amount

This option only displays if the **Invulnerable** option is set to **Off**. Determines the starting health value for spawned guards.

**Max Health**

**100**, Pick an amount

This option only displays if the **Invulnerable** option is set to **Off**. Determines the maximum health value for spawned guards.

**Starting Shield**

**No Shield**, Pick an amount

Determines the starting shield value for spawned guards.

**Max Shield**

**No Shield**, Pick an amount

Determines the maximum shield value for spawned guards.

**Show Health Bar**

Yes, No

Determines whether a guard's health is displayed in a health bar above the guard's head.

**Enable Patrol**

Yes, No

This determines whether the guards move around to patrol an area, or whether they stay in one place.

**Max Patrol Distance**

**10M**, Pick a distance

This is the maximum amount of distance a patrolling guard can move from the spawner location. This does not apply if you are using an AI Patrol Path device to set specific Patrol Paths and Patrol Path Groups.

**Spawn On Patrol Path Group**

**Group None**, Pick a group number

Assigns guards to the selected Patrol Path Group.

**Enable Resuming Patrol Path**

Yes, No

Requires **Spawn on Patrol Path Group** to have a value of at least **1** to enable this option.

Determines if the Guards should resume patrolling their path if it was disabled and then enabled. If **Disabled**, the Guards must be assigned a path through a path's **Assign AI To Path** function to continue following the path.

**Change Patrol Path Target**

Never, On Timer, and On Spawn.

Requires **Spawn on Patrol Path Group **to have a value of at least **1** to enable this option.

Determines how often the spawner will select a new random Patrol Path within its Patrol Path Group. If **Never**, the device will always use the first Patrol Path in the Patrol Path Group.

**Change Patrol Path Timer**

**1.0 seconds**, Pick an amount.

Requires **Change Patrol Path** to be set to **On Timer** to enable this option.

Determines the amount of time newly spawned Guards will spend select their patrol path. After it ends, newly spawned Guards will randomly select Patrol Paths. This won't impact Guards that have already spawned.

**Should Randomly Select Paths**

Yes, No

Requires Change Patrol Path to be set to On Spawn or **On Timer** to enable this option.

Determines if the device should randomly select a path to use.

If disabled, the device will select the path (in order of their index if they have been set) that has not had a guard spawned on it. This resets after a guard has spawned on each Patrol Path in the Patrol Path Group.

If multiple paths have the same index, they will be randomly ordered between themselves.

**Can Assign to Disabled Paths**

Yes, No

Requires **Change Patrol Path** to be set to **On Spawn **or **On Timer** to enable this option.

Determines if Guards can be assigned to Patrol Paths that are disabled to use in the future. The Guard will fall back to using the patrol around device behavior until the path is enabled.

If disabled, patrol paths will be ignored unless all paths are disabled.

**Visibility Range**

**40M**, Pick a distance

Sets the maximum distance for a guard's' sight perception. Guards can still become alerted based on sound, regardless of this range.

**Visibility Range Restriction**

**Only When Unaware**, Always

Determines whether the value for the **Visibility Range** option is in effect always, or only when guards are not alerted.

**Team Awareness Propagation**

**Yes**, No

If the guards are assigned to a team, this determines whether a guard's detection of players is spread to the guard's team.

**Drop Inventory On Elimination**

**Yes**, No

Determines whether a guard drops their entire inventory when they are eliminated.

**Accuracy**

**Moderate**, Pick a level

Determines how accurate guards are when they shoot at players.

**Despawn Guards when Disabled**

**Yes**, No

Determines whether spawned guards remain or if they are despawned when the spawner is disabled.

**Can Be Hired**

*Yes*, **No**

Determines whether the spawned guards can be hired by a player. If you choose **Yes**, additional options display below this one.

**Allow Hire Conversation**

**Yes**, No

This option only displays if the **Can Be Hired** option is set to **Yes**. Determines whether players can hire guards using a conversation interaction. If you choose **No**, guards can only be hired or dismissed using events.

**Hired Guard Name**

Enter text

This option only displays if the **Can Be Hired** option is set to **Yes**. Type in a name for a hired guard. This name will be used in the "Hire a Guard" conversation. The text field is limited to 16 characters.

**Maximum Hired Guards**

**Don't Override**, Pick a number

This option only displays if the **Can Be Hired** option is set to **Yes**. Determines the maximum number of guards spawned by this device that a player can hire in the game. **Don't Override** means the maximum is the same as the value set in the Island Settings.

**Auto Hire When Spawned**

**No Auto Hire**, Last Hiring Player, Triggering Player

This option only displays if the **Can Be Hired** option is set to **Yes**. Determines whether the spawned guard is automatically hired. Values for this option are:

-
**No Auto Hire**: Spawned guards are not automatically hired.

-
**Last Hiring Player**: The spawned guard is automatically hired by the last hiring player.

-
**Triggering Player**: The spawned guard is automatically hired by the player that triggered the spawner.

**Restore Health and Shield When Hired**

**No**, Yes

This option only displays if the **Can Be Hired** option is set to **Yes**. Determines whether a damaged guard's health and shield will be restored to default values when the guard is hired.

**Despawn When Dismissed**

**No**, Yes

This option only displays if the **Can Be Hired** option is set to **Yes**. Determines whether the hired guard automatically despawns when the player dismisses the guard.

**Can Be Given Commands**

**No**, Yes

This option only displays if the **Can Be Hired** option is set to **Yes**. Determines if a spawned Guard can be given commands. By default, only the most recently hired Guard can be given commands.

**Use Alertness**

Yes, No

Determines whether the guard displays its alertness level over its head.

### Direct Event Binding

Following are the [direct event binding](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) options for this device.

#### Functions

A [function](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) listens for an event on a device then performs an action.

-
For any function, click the **option**, then **Select Device** to access and select from the **Device** dropdown menu.

-
Once you've selected a device, click **Select Event** to bind the device to an event that will trigger the function for the device.

-
If more than one device or event triggers a function, click the **Add** button to add a line and repeat these steps.

**אפשרויות ותיאורים:**

##### Enable When Receiving From

This function enables the device when an event occurs.

##### Disable When Receiving From

This function disables the device when an event occurs.

##### Spawn When Receiving From

This function spawns a guard when an event occurs.

##### Despawn When Receiving From

This function despawns a guard when an event occurs.

##### Reset Total Spawn Count When Receiving From

This function resets the total spawn count for this device when an event occurs.

##### Hire When Receiving From

This function hires a guard when an event occurs.

##### Dismiss All Hired Guards When Receiving From

This function dismisses any hired guards that spawned from this device when an event occurs.

##### Dismiss Instigator Hired Guards When Receiving From

This function dismisses any guards hired by the instigating player when an event occurs.

##### Set Guard Hireable When Receiving From

All guards spawned by this device are set as hireable when an event occurs.

##### Set Guard Not Hireable When Receiving From

All guards spawned by this device are set as not hireable when an event occurs.

##### Force Attack Target When Receiving From

When an event occurs, this function forces a guard to attack a specific target, bypassing perception checks.

#### Events

Direct event binding uses events as transmitters. An event tells another device to perform a function.

-
For any event option, click the **option**, then **Select Device** to access and select from the **Device** dropdown menu.

-
Once you've selected a device, click **Select Function** to bind the timer to a function for that device.

-
If more than one function is triggered by the event, click the **Add** button to add a line and repeat these steps.

**אפשרויות ותיאורים:**

##### On Spawned Send Event To

When the device spawns a guard, it sends an event to the selected device, which triggers the selected function.

##### On Alerted to Player Send Event To

When a guard is alerted to the player, it sends an event to the selected device, which triggers the selected function.

##### On Alerted to AI Send Event To

When a guard is alerted to an AI entity, it sends an event to the selected device, which triggers the selected function.

##### On Alerted Send Event To

When a guard is alerted, it sends an event to the selected device, which triggers the selected function.

##### On Target Lost Send Event To

When a guard loses sight of its target, it sends an event to the selected device, which triggers the selected function.

##### On Suspicious Send Event To

When a guard becomes suspicious, it sends an event to the selected device, which triggers the selected function.

##### On Unaware Send Event To

When a guard becomes unaware, it sends an event to the selected device, which triggers the selected function.

##### On Eliminated Send Event To

When a guard is eliminated, it sends an event to the selected device, which triggers the selected function.

##### On Eliminating Player Send Event To

When a guard eliminates a player, it sends an event to the selected device, which triggers the selected function.

##### On Eliminating AI Send Event To

When a guard eliminates an AI entity, it sends an event to the selected device, which triggers the selected function.

##### On Eliminating Send Event To

When a guard eliminates an opponent, it sends an event to the selected device, which triggers the selected function.

##### On Damaged Send Event To

When a guard takes damage, it sends an event to the selected device, which triggers the selected function.

##### On Hired Send Event To

When a guard is hired by a player, it sends an event to the selected device, which triggers the selected function.

##### On Dismissed Send Event To

When a player dismisses a guard, it sends an event to the selected device, which triggers the selected function.

---

## Using Post Processing Devices in Fortnite Creative

**כותרת מקורית:** Using Post Processing Devices in Fortnite Creative  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/using-post-processing-devices-in-fortnite-creative  
**מקור קלט:** `07F_דמויות_AI_תאורה_סביבה_וVFX(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `using-post-processing-devices-in-fortnite-creative`

**Post-processing** refers to customizable filters that you can use to create specific visual effects. Most of these filters primarily affect lighting.The **Post Process** device provides a way to apply these different effects on your island.

You may recognize some of the effects from the **camera filters** in **Island Settings** under the [**World**](https://dev.epicgames.com/documentation/fortnite/world-settings-in-fortnite-creative) category, but this device provides even more options.

For a Post Process effect to work correctly, make sure the **Camera Filter** option in the World category is set to **Default (none)**.

Apply these effects to a specific player, throughout an entire island, or set up different effects to happen based on user interactions or activation by other devices. You can also set the effect to remain indefinitely, or to turn off after a specified time or based on [event bindings](https://dev.epicgames.com/documentation/fortnite/using-post-processing-devices-in-fortnite-creative).

You can control transitions between different effects or from no effect to effect and back again by using the **blend** options to set how an effect blends from one state to another.

These effects can be used to simulate or enhance environmental factors or character moods or attitudes.

Using UEFN? Learn more about [post-process effects](https://dev.epicgames.com/documentation/en-us/uefn/intro-to-post-processing-in-unreal-editor-for-fortnite) in our UEFN and Verse documentation.

For help on how to find the **Post Process** device, see [Using Devices](https://dev.epicgames.com/documentation/fortnite/using-devices-in-fortnite).

If you're using multiple copies of a device on an island, it can be useful to [rename](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#rename-a-device) them. Choosing names that relate to a device's purpose makes it easier to remember what each one does, and easier to find a specific device when using the [**Event Browser**](https://dev.epicgames.com/documentation/fortnite/event-browser-in-fortnite-creative).

### Device Options

Configure this device with the following options.

Default values are **bold**.

**אפשרויות, ערכים ותיאורים:**

##### Enabled During Phase

- **Value / Values:** None, **Always**, Pre-Game Only, Gameplay Only, Create Only
- **Description:** Sets the phase in which the device will be enabled.

##### Post Process Effect

- **Value / Values:** **None**, Pick an effect
- **Description:** This is the effect that is applied when the device is enabled. See [Effect Options](https://dev.epicgames.com/documentation/fortnite/using-post-processing-devices-in-fortnite-creative) below for more info on each effect.

##### Effect Duration

- **Value / Values:** **Infinite**, Pick a time in seconds
- **Description:** How long the post process effect will last. **Infinite (0)** continues the effect indefinitely, or you can set a time for when it starts blending out.

##### Priority

- **Value / Values:** **0**, Pick a priority
- **Description:** If you're using more than one effect and they overlap, this determines which effect will display. If two or more effects have the same priority, they will attempt to blend together, but they may not blend the same way for every player.

##### Starting Strength

- **Value / Values:** **1.0**, Pick a value
- **Description:** How strong the effect you use is at the start. The higher the value, the more intense the effect is. The value you set here clamps to **Blend In Strength**.

##### Blend In Strength

- **Value / Values:** **0.0**, Pick a value
- **Description:** How strong the effect is when blended in.

##### Blend In Duration

- **Value / Values:** **0.0**, Pick a time in seconds
- **Description:** How long it takes for a blend to go from 0 strength to full blend.

##### Blend Out Duration

- **Value / Values:** **0.0**, Pick a time in seconds
- **Description:** How long it takes for a blend to go back to 0 strength.

##### Applies to Team

- **Value / Values:** **Any**, Pick a team
- **Description:** Sets which team can activate the device and see the effect.

##### Applies to Class

- **Value / Values:** **Any**, Pick a class
- **Description:** Sets which class can activate the device and see the effect.

### Effect Options

 Effect What It Looks Like
**None**: How things look with no effect applied.
**

**Oak**: Washes out the color and shadows and applies subtle outlines.

**Dark**: Makes things look pretty danged dark. Good for creating a night setting.

**Film Noir**: Gives everything a washed-out black-and-white effect.

**Film Warm**: Warms up the appearance by increasing the yellow.

**Happy Place**: Uses a cheerful palette that makes your island scene look fun!

**Pixelizer**: Pixelizes the image in a way that conjures up old video game consoles from last century.

**Red**: Gives everything a red hue.

**Sepia**: Gives the scene a reddish-brown hue, like an old Wild West photograph.

**Crazy**: This effect makes your players want to emote like no one's watching! The solarization effect reverses colors in unexpected ways.

**Retro**: Outlines images with a glowing line.

**Spooky**: Desaturates the colors just enough to create an edgy feeling.

**Neon Party**: Applies a neon glow to things, but more subtly than the retro effect does.

**Horror Movie**: Washes out color, but less so than the low exposure effect.

**Old Cartoon**: Applies outlines similarly to Comic, but in black and white. It also adds a static effect that simulates old film moving through an analog projector.

**Desolate**: Deepens shadows regardless of time-of-day setting, which creates a feeling of foreboding.

**Halftone**: A bright effect that uses a texture similar to Comic and Neocomic.

**CCTV**: Shows a low-fidelity image in monochrome as though you're watching over a closed-circuit security camera.

**70s Print**: This effect is reminiscent of a Polaroid snapshot that has faded over decades.

**Action Lines**: Dynamic lines radiating outward from the character and action. This effect can convey excitement when a character reacts to something dramatically.

**Comic**: Applies an outline to details.

**Low Exposure**: Washes out much of the color and contrast, the way an underexposed photo would.

**Neocomic**: Intensifies contrast, and adds subtle outlines.

**Nightvision**: Seeing the world through night-vision goggles makes this effect great for stealth games or missions.

**Radial Blur**: Creates a blur effect that radiates from a central point.

**Simple Blur**: Makes everything blurry. What the world looks like when some people take off their glasses.

**VHSfilter**: What things look like when a VHS tape that was played too many times, this is an effect that conjures a vibe from last century, right down to static on the screen and moving bands of color.

**Vignette**: An effect that simulates darkening in a real-world camera lens.Vignetting is mostly noticeable near the edges of the image.

**Heatwave**: A shimmery effect that mimics looking at things in extreme heat such as in a desert area.

**Rain**: Shows raindrops as though on the surface of the camera lens. This is useful when you're creating a rain environment, or when the camera is coming out of water.

**Frost**: An effect like frost on a window pane. It's primarily around the edges.

**80s Cartoon**: Applies outline similarly to Comic, but with brighter and flatter colors.

**Comic Noir**: Applies an outline like Comic or Old Cartoon, but has no static and includes a white border around the entire game screen.

Heavy Linework**: Applies a black and white comic book filter with heavy linework around assets and characters on screen.

### Direct Event Binding

Following are the [direct event binding](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) options for this device.

#### Functions

A [function](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#function) listens for an event on a device then performs an action.

-
For any function, click the **option**, then **Select Device** to access and select from the **Device** dropdown menu.

-
Once you've selected a device, click **Select Event** to bind the device to an event that will trigger the function for the device.

-
If more than one device or event triggers a function, press the **Add** button to add a line and repeat these steps.

**אפשרויות ותיאורים:**

##### Enable for All When Receiving From

Enables the device for all players when an event occurs.

##### Disable for All When Receiving From

Disables the device for all players when an event occurs.

##### Blend In for All When Receiving From

Starts the Blend In from current strength to the Blend In Strength value for all players when an event occurs.

##### Blend Out for All When Receiving From

Starts the Blend Out from current strength to 0 value for all players when an event occurs.

##### Reset for All When Receiving From

Resets to the initial starting strength for all players when an event occurs. This also ends any ongoing blending.

##### Enable for Instigator When Receiving From

Enables the device only for the instigating player when an event occurs.

##### Disable for Instigator When Receiving From

Disables the device only for the instigating player when an event occurs. It also pauses (and hides) any ongoing blending until the device is re-enabled.

##### Blend In for Instigator When Receiving From

Starts blending in when an event occurs, but only for the instigating player.

##### Blend Out for Instigator When Receiving From

Starts blending out when an event occurs, but only for the instigating player.

##### Reset for Instigator When Receiving From

Resets to the initial starting strength when an event occurs, but only for the instigating player.

#### Events

An [event](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#event) tells another device when to perform a function.

-
For any event option, click the **option**, then **Select Device** to access and select from the **Device dropdown menu**.

-
Once you've selected a device, click **Select Function** to bind this event to a function for that device.

-
If more than one function is triggered by the event, click the **Add** button to add a line and repeat these steps.

**אפשרויות ותיאורים:**

##### On Blending In Is Send Event To

Sends an event to a linked device when blending in is complete.

##### On Blending Out Is Send Event To

Sends an event to a linked device when blending out is complete.

---

## Using Skydome Devices in Fortnite Creative

**כותרת מקורית:** Using Skydome Devices in Fortnite Creative  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/using-skydome-devices-in-fortnite-creative  
**מקור קלט:** `07F_דמויות_AI_תאורה_סביבה_וVFX(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `using-skydome-devices-in-fortnite-creative`

The S 14 Time of Day Manager and the Skydome device are being retired in an upcoming release. Create custom lighting with the [Day Sequence device](https://dev.epicgames.com/documentation/fortnite/day-sequence-device-in-fortnite-creative) as well as the [Ambience settings](https://dev.epicgames.com/documentation/fortnite/world-settings-in-fortnite-creative#ambience-settings) available in World Settings.

Opting into the new TODM is **not reversible**, backup or duplicate your island before opting into the new lighting settings.

The **Skydome** device controls how the sky looks, as well as giving you options for changing the sun, clouds, stars or other objects in the sky above your island. You can experiment with the sun and moon, and add other atmospheric elements like stars, fog and clouds. You can change the color of your light source, and blend different colors for your island’s sky to create the perfect atmosphere for your game.

Setting options in the Skydome device will override sky and atmosphere options in the [My Island](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) settings.

Here are some of the things you can do with this device:

-
Create a moonlit night for a spooky game.

-
Change the color of the sky to simulate being on another planet.

-
Change the color of the moon, or the visibility of the stars.

-
Add clouds to the sky, and customize the speed and direction of those clouds.

### Finding and Placing the Device

*Click image to enlarge.*

-
From [Create mode](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#create-mode), press the **Tab** key to open the [Creative inventory](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) screen.

-
Click the **DEVICES** tab. You can scroll to select the device, use the **Search** box to look up the device by name, or check the **Categories** in the panel on the left.

-
Click **PLACE NOW** to [place](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#place) immediately, or put the device in the [QUICK BAR](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#quick-bar) to place later.

-
Press **Tab** to return to your island in Create mode. Use your [phone](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#phone) to position the device, then click to place it. Press **`** to detach the device from your phone tool.

-
Point at the device with your phone. If the **Customize** popup doesn't open immediately, move closer until it does, then press **E** to open the CUSTOMIZE panel.

If you're using multiple copies of a device on an island, it can be helpful to [rename](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#rename-a-device) them. You can choose names that relate to each device's purpose, so it's easier to remember what each one does.

### Device Options

This device has some basic functionality, like choosing the light source and its color. Additionally, there are some advanced options, like [enabling](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#enable) horizon fog and stars.

You can configure this device with the following options.

Default values are **bold**.

#### Basic Options

**אפשרויות, ערכים ותיאורים:**

##### Light Source

- **Value / Values:** None, **Sun**, Moon 1, Moon 2
- **Description:** Defines what the light source is for the Skydome. The position of the light source is defined by the placement direction of the device. When you place the device, use the rotation controls to change the direction of the device's arrows. This will change the position of the light source.

##### Lightsource Custom Color

- **Value / Values:** **#FFFFFF**, Pick a color
- **Description:** Determines the color of the light shining from the device. Click the color swatch to open the Color Picker. Each color swatch has its Hex Code next to the swatch. You can also type a Hex Code into the Search bar to find a specific color. Select a color, then click the checkmark.

##### Lightsource Intensity

- **Value / Values:** **100%**, Pick a percentage
- **Description:** Defines the intensity of the light coming from the light source.

##### Skydome Top Color

- **Value / Values:** **#217894**, Pick a color
- **Description:** The Skydome is colored using a gradient. This option defines the top color in the gradient. Click the color swatch to open the Color Picker. Select a color swatch or enter a Hex Code for the color you want, then click the checkmark.

##### Skydome Middle Color

- **Value / Values:** **#7EA5FF**, Pick a color
- **Description:** The Skydome is colored using a gradient. This option defines the middle color in the gradient. Click the color swatch to open the Color Picker. Select a color swatch or enter a Hex Code for the color you want, then click the checkmark.

##### Skydome Bottom Color

- **Value / Values:** **#217894**, Pick a color
- **Description:** The Skydome is colored using a gradient. This defines the bottom color in the gradient. Click the color swatch to open the Color Picker. Select a color swatch or enter a Hex Code for the color you want, then click the checkmark.

##### Ambient Light

- **Value / Values:** **#FFFFFF**, Pick a color
- **Description:** Determines the color of the ambient light. Click the color swatch to open the Color Picker. Select a color swatch or enter a Hex Code for the color you want, then click the checkmark.

##### Ambient Light Intensity

- **Value / Values:** **20%**, Pick a percentage
- **Description:** Defines the intensity of the ambient light source.

##### Clouds

- **Value / Values:** **Off**, Twisty, Realistic
- **Description:** Determines whether there are clouds in the sky, and if there are clouds this determines what type of clouds appear.

##### Clouds Speed

- **Value / Values:** None, **Very Slow**, Slow, Fast, Very Fast
- **Description:** If there are clouds, this determines how fast the clouds are moving.

##### Clouds Direction

- **Value / Values:** **N**, Pick a compass direction
- **Description:** If there are clouds, this determines the direction the clouds are moving. This is used in conjunction with the **Clouds Speed** option. Values use compass directions, such as **N** for North, **S** for South, and so on.

##### Clouds Color

- **Value / Values:** **#FFFFFF**, Pick a color
- **Description:** Customizes the color of the skydome's clouds.

#### All Options (Additional)

**אפשרויות, ערכים ותיאורים:**

##### Enabled During Phase

- **Value / Values:** None, **All**, Create Only, Game Countdown Only, Gameplay Only
- **Description:** Determines when the Skydome device is enabled.

##### Lightsource Color Mode

- **Value / Values:** **Custom Color**, Match Position
- **Description:** If this is set to the default of **Custom Color**, you can choose the color of the light. If you choose **Match Position**, the device sets a color based on the device's angle of rotation.

##### Stars Visibility

- **Value / Values:** **Off**, Dim, Bright
- **Description:** Determines whether stars are visible in the sky, and if so, how bright they are.

##### Horizon Fog Density

- **Value / Values:** Default, **20%**, Pick a percentage
- **Description:** Determines whether there is atmospheric fog at the horizon, and if so, how far above the horizon it extends.

##### Horizon Fog Color

- **Value / Values:** **#217894**, Pick a color
- **Description:** If you have horizon fog, this sets the color of that fog. If you want a different color, click the color swatch to open the Color Picker. Select a color swatch or enter a Hex Code for the color you want, then click the checkmark

##### Use Volume

- **Value / Values:** Yes, **No**
- **Description:** If you choose **Yes** the device will use the volume as a zone of activation.

##### Volume Width

- **Value / Values:** **1**, Pick a number of tiles
- **Description:** Determines the width of the volume in tiles. This is only used if the **Use Volume** option is set to **Yes**.

##### Volume Depth

- **Value / Values:** **1**, Pick a number of tiles
- **Description:** Determines the depth of the volume in tiles. This is only used if the **Use Volume** option is set to **Yes**.

##### Volume Height

- **Value / Values:** **1**, Pick a number of tiles
- **Description:** Determines the height of the volume in tiles. This is only used if the **Use Volume** option is set to **Yes**.

##### Sky Gradient Colors Influence Ambient Light

- **Value / Values:** **On**, Off
- **Description:** Determines if the backdrop colors influence the ambient light.

##### Post Process

- **Value / Values:** **Night**, Pick a preset effect
- **Description:** Sets a graphic process to enhance the visual look of the skydome using different presets.

### Channels

When one device needs to "talk" to another device, it does so by [transmitting](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) a [signal](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) on a specific [channel](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary). The receiving device needs to be set up to [receive](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#receive) the signal on the same channel.

A channel is identified by a number, and channel numbers are customized for a device under the option that uses the channel. Most devices will also pass the identity of the player who [triggered](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#trigger) the device with the signal.

This device has receivers that perform a variety of functions when receiving a signal over a channel. Also, this device can transmit signals when certain conditions are met.

#### Receivers

Receivers listen for a channel and perform an action when they hear any device (including themselves) send a signal on that channel.

**אפשרויות, ערכים ותיאורים:**

##### Enable When Receiving From

- **Value / Values:** **No Channel**, Pick a channel
- **Description:** Enables the device when it receives a signal on the selected channel.

##### Disable When Receiving From

- **Value / Values:** **No Channel**, Pick a channel
- **Description:** Disables the device when it receives a signal on the selected channel.

---

## Using VFX Creator Devices in Fortnite Creative

**כותרת מקורית:** Using VFX Creator Devices in Fortnite Creative  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/using-vfx-creator-devices-in-fortnite-creative  
**מקור קלט:** `07F_דמויות_AI_תאורה_סביבה_וVFX(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `using-vfx-creator-devices-in-fortnite-creative`

Use the **VFX Creator** to create and customize your own [visual effects](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#vfx),
using a library of [sprites](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#sprite), and with lots of ways to modify them.

This device is more flexible than the [VFX Spawner](https://dev.epicgames.com/documentation/fortnite/using-vfx-spawner-devices-in-fortnite-creative), which gives you a selection of pre-made visual effects to choose from but limits how much you can customize or change those effects.

The VFX Creator creates a [sprite particle effect](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#sprite-particle-effect). You have a large variety of [sprites](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#sprite) to choose from, and a lot of ways to customize how the particle effect works and what it looks like. Using this device, you can create unique effects for your game.

Ways you can use this device include:

-
Highlight an in-game event, such as the beginning or end of a race, or the completion of an objective.

-
Make eliminating a boss even more spectacular and satisfying.

-
Create a particular atmosphere on your island, or emphasize a fantastical aspect of your game.

-
Create environmental effects like rain or leaves.

-
Create interesting trail effects by attaching the VFX to a player.

**Looking for a spark of creative freedom?** See [**Down But Not Out Device Design Example**](https://dev.epicgames.com/documentation/fortnite/down-but-not-out-device-design-example-in-fortnite-creative) to liberate your imagination!

To find the VFX Creator device, go to the **Creative inventory** and select the **Devices** tab. From there, you can search or browse for the device. For more information on finding devices see [Finding and Placing Devices](https://dev.epicgames.com/documentation/fortnite/using-devices-in-fortnite).

If you're using multiple copies of a device on an island, it can be helpful to [rename](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#rename-a-device) them. You can choose names that relate to each device's purpose, so it's easier to remember what each one does.

### Contextual Filtering

Some devices are affected by a feature called **contextual filtering**. This feature hides or displays options depending on the values selected for certain related options. This feature will reduce clutter in the [Customize panel](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#customize-panel) and make options easier to manage and navigate. However, it may not be easy to recognize which options or values trigger contextual filtering. To help you identify them, any values in our device docs that trigger contextual filtering are in *italic*.

All options will be listed, including those affected by contextual filtering; if they are hidden or displayed based on a specific option's value, there will be a note about that in the Description field for that option.

### Device Options

This device has some basic functionality, like choosing the sprite for the effect, and choosing the color and brightness of the effect. Additionally, there are some advanced options, like choosing a secondary color and determining whether the effect loops.

You can configure this device with the following options.

Default values are **bold**. Values that trigger contextual filtering are *italic*.

**אפשרויות, ערכים ותיאורים:**

##### Start Effects When Enabled

- **Value / Values:** **Yes**, No
- **Description:** Determines whether the device executes the effects when it is enabled.

##### Enabled During Phase

- **Value / Values:** None, **All**, Create Only, Game Countdown, Gameplay Only
- **Description:** Determines the phases during which the device is enabled.

##### Sprite Shape

- **Value / Values:** **Soft Circle**, Pick a sprite
- **Description:** Determines which sprite is used for the particle effect. Click the sprite to open the sprite picker. Click to select a sprite.

##### Sprite Size

- **Value / Values:** **1X**, Pick a multiplier
- **Description:** Determines the sprite particle size when the effect starts. This is expressed as a multiple of the sprite's default size, which can vary from sprite to sprite.

##### Sprite Duration

- **Value / Values:** **1S**, Pick an amount of seconds
- **Description:** Determines the lifetime of each sprite particle in the effect.

##### Sprite Rotation Alignment

- **Value / Values:** **Random**, Speed, Planar
- **Description:** Determines how the sprite particles are displayed. **Random** rotates each particle in a random direction. **Speed** rotates each in the direction the particle is moving. With **Planar** each sprite particle faces the device.

##### Use Random Color

- **Value / Values:** ***No***, Yes
- **Description:** Determines the color of the effect. **Yes** uses a random color each time the effect loops. If you select **No**, the **Main Color** option displays and you can select a color.

##### Main Color

- **Value / Values:** **White**, Pick a color
- **Description:** Only displays if **No** is set for **Use Random Color**. This sets the color of the effect. Click the swatch to open the **Color Picker**, then click the picker to select a color.

##### Main Color Brightness

- **Value / Values:** **1**, Pick a level
- **Description:** Determines the brightness of the effect color.

##### Use Secondary Color

- **Value / Values:** **No**, *Yes*
- **Description:** Determines whether a second color will be used along with the main color, to create a color transition in the effect. If you choose **Yes**, the **Random Secondary Color** and **Secondary Color Brightness** options display.

##### Random Secondary Color

- **Value / Values:** ***No***, Yes
- **Description:** This option only displays if you choose **Yes** for the **Use Secondary Color** option. Determines how the secondary color of the effect is chosen. If you choose **Yes**, the device uses a random secondary color for the effect. If you choose **No**, the **Secondary Color** option displays so you can select a color for the effect.

##### Secondary Color

- **Value / Values:** **White**, Pick a color
- **Description:** This option only displays if you choose **No** for the **Random Secondary Color** option. This option sets the secondary color of the effect. Click the swatch to open the color picker. Click to select a color, then click the checkmark to close the color picker.

##### Secondary Color Brightness

- **Value / Values:** **1**, Pick a level
- **Description:** Determines the brightness level of the effect's color.

##### Sprite Speed

- **Value / Values:** **50%**, Pick a percentage
- **Description:** Determines the speed of the sprite particles when the effect loop starts.

##### Effect Gravity

- **Value / Values:** **50%**, Pick a percentage
- **Description:** Determines how fast sprite particles fall, expressed as a percentage of normal gravity.

##### Randomness

- **Value / Values:** **50%**, Pick a percentage
- **Description:** Determines how random the movement and size of the sprites will be. The percentage values are an abstract expression of the amount of randomness used.

##### Keep Size

- **Value / Values:** **Yes**, *No*
- **Description:** Determines whether spawns keep the same size after spawning, or change size over time. If you select **No**, the option **Size Over Time** will display.

##### Size Over Time

- **Value / Values:** **75%**, Pick a percentage
- **Description:** Sets how much the sprites will change in size over time. Less than 100 percent will make them smaller; more than 100 will make them larger.

##### Spawn Mode

- **Value / Values:** **Continuous**, Bursts
- **Description:** Determines whether the sprite particles will generate continually, or whether they will generate in bursts.

##### Effect Generation Amount

- **Value / Values:** **50%**, Pick a percentage
- **Description:** Determines how many sprite particles are generated.

##### Loop

- **Value / Values:** **Forever**, Never, Custom
- **Description:** Determines whether the effect loops.

##### **Forever:** Once the effect spawns, it will continue to spawn in a loop until something stops it.

- **Value / Values:** **Never:** It will play once, then stop.
- **Description:** **Custom:** Select how many times you want it to loop under **Loop Times**.

##### Loop Times

- **Value / Values:** **1**, Pick a number
- **Description:** Set how many times an effect should loop. This option only appears if you select **Custom** for **Loop**.

##### Loop Duration

- **Value / Values:** **1S**, Pick a time in seconds
- **Description:** Determines how long it takes for the effect to play through once. If the effect loops, this is how long the loop lasts.

##### Time Between Loops

- **Value / Values:** **1S**, Instant (0), Pick a time in seconds
- **Description:** If the effect is set to loop, this determines whether the effect begins again immediately, or if the device waits the selected amount of time before starting the effect again.

##### Spawn Zone Shape

- **Value / Values:** **Sphere**, Box, Point
- **Description:** Determines the shape of the space where the sprite particles initially spawn.

##### Spawn Zone Size

- **Value / Values:** **0.5**, Pick a size
- **Description:** Sets the size of the spawn shape in [tiles](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#tile).

##### Stick to Player

- **Value / Values:** **No**, *Yes*
- **Description:** Determines whether the sprite effect spawns and sticks to a player. If you choose **Yes**, the **Spawn On Player Body Part** options display.

##### Spawn On Player Body Part

- **Value / Values:** **Center**, Head, Base, Weapon
- **Description:** Sets where on the player the effects will spawn.

#### Sprites Available

Below is a table showing all the sprites you can use when creating an effect.

 Sprites

Soft Circle

Square

Triangle

Spark

Lens Flare 01

Lens Flare 02

Star

Disc 01

Disc 02

Fire Disc

Shockwave Disc

Dots

Musical Notes

Electric

Leaf

Flower

Snowflake

Droplet

Arrow 01

Arrow 02

Arrow 03

Smoke 01

Smoke 02

Smoke 03

Plus Sign

Heart

Splatter

Bubble

Ash

### Direct Event Binding

Following are the [direct event binding](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#direct-event-binding) options for this device.

#### Functions

A [function](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#function) listens for an event on a device then performs an action.

-
For any function, click the option, then Select Device to access and select from the Device dropdown menu.

-
Once you've selected a device, click Select Event to bind the device to an event that will trigger the function for the device.

-
If more than one device or event triggers a function, press the Add button to add a line and repeat these steps.

**אפשרויות ותיאורים:**

##### Start Effect at Device When Receiving From

Starts the effect generation when receiving a signal from the selected event.

##### Stop Effect at Device When Receiving From

Stops the effect generation when receiving a signal from the selected event.

##### Toggle Effect at Device When Receiving From

Starts or stops the effect generation when receiving a signal from the selected event.

##### Enable When Receiving From

Enables the device when receiving a signal from the selected event.

##### Disable When Receiving From

Enables the device when receiving a signal from the selected event.

##### Toggle Effect Pause at Device When Receiving From

Pauses or resumes the effect keeping it frozen in place when receiving a signal from the selected event.

##### Spawn at Player When Receiving From

Spawns a start the effects at the instigating player's position when receiving a signal from the selected event.

##### Remove Effect from Player When Receiving From

Removes the effect from the moving player to the device position without stopping the effects when receiving a signal from the selected event.

##### Remove Effect from All Players When Receiving From

Removes the effect from the moving instigating player to the device position without stopping the effects when receiving a signal from the selected event.

##### Start Effect at Player When Receiving From

Starts the effect generation when receiving a signal from the selected event.

##### Start Effect for All Players When Receiving From

Starts the effect generation when receiving a signal from the selected event.

##### Stop Effect at Player When Receiving From

Stops the effect generation when receiving a signal from the selected event.

##### Stop Effect for All Players When Receiving From

Stops the effect generation when receiving a signal from the selected event.

##### Toggle Effect Pause at Player When Receiving From

Pauses or resumes the effect keeping it frozen in place when receiving a signal from the selected event.

##### Toggle Effect Pause for All Players When Receiving From

Pauses or resumes the effect keeping it frozen in place when receiving a signal from the selected event.

##### Toggle Effect at Player When Receiving From

Starts or stops the effect generation when receiving a signal from the selected event.

##### Toggle Effect for All Players When Receiving From

Starts or stops the effect generation when receiving a signal from the selected event.

##### Toggle Enabled When Receiving From

Enables or disables the device when receiving a signal from the selected event.

#### Events

Direct event binding uses events as transmitters. An event tells another device to perform a function.

There are no events for this device.

---

## Using VFX Spawner Devices in Fortnite Creative

**כותרת מקורית:** Using VFX Spawner Devices in Fortnite Creative  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/using-vfx-spawner-devices-in-fortnite-creative  
**מקור קלט:** `07F_דמויות_AI_תאורה_סביבה_וVFX(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `using-vfx-spawner-devices-in-fortnite-creative`

With **VFX Spawner** devices, you can place different [visual effects](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#vfx) around your island.

These effects fall into one of two types:

-
**Continuous**: Once activated, the effect will continue to loop until it is deactivated.

-
**Burst**: A quick effect that occurs once, then stops.

Things you can do with the VFX Spawner device include:

-
Use a burst effect, such as a poof of dust or a small explosion, to mask the spawning of a prop.

-
Use any of the musical note effects to visually show the source of music.

-
Simulate weather with effects like rain or snow, or even a tornado!

These effects are also useful for ambience. Integrating an effect with your environment can create subtle, effective moods.

**Looking for more inspiration?** See [**D-Launcher Device Design Examples**](https://dev.epicgames.com/documentation/fortnite/d-launcher-device-design-examples-in-fortnite-creative.INT.udn) to kick off your imagination!

To find the VFX Spawner device, see [Using Devices](https://dev.epicgames.com/documentation/fortnite/using-devices-in-fortnite).

If you're using multiple copies of a device on an island, it can be helpful to [rename](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#rename-a-device) them. Choosing names that relate to a device's purpose makes it easier to remember what each one does, and easier to find a specific device when using the [Event Browser](https://dev.epicgames.com/documentation/fortnite/event-browser-in-fortnite-creative).

### Contextual Filtering

Some devices are affected by a feature called **contextual filtering**. This feature hides or displays options depending on the values selected for certain related options. This reduces clutter in the Customize panel and makes options easier to manage and navigate. To help identify them, values that trigger contextual filtering are in *italic*.

All options are listed, including those affected by contextual filtering; if they are hidden or displayed based on a specific option's value, there will be a note about it in the Description field for that option.

### Device Options

This device has some basic functionality, like setting the type of effect and the speed of the effect's looped animation. Additionally, there are some advanced options, like the phases when the effect is enabled.

Default values are **bold**. Values that trigger contextual filtering are *italic*.

You can configure this device with the following options.

 Option Value Description
**Effect Type**

***Continuous***, *Burst*

Determines whether the effect will play in a continuous loop, or in a short burst, then stop. The next option changes based on what you select here.

**Visual Effect**

**Fireworks**, Pick an effect

This sets the type of visual effect the device produces when the **Effect Type** is set to **Continuous**. See [Continuous Effects](https://dev.epicgames.com/documentation/fortnite/using-vfx-spawner-devices-in-fortnite-creative#continuous-effects) for a list of available effects.

**Burst Visual Effect**

**Explosion Small**, Pick an effect

This sets the type of visual effect the device produces when the **Effect Type** to **Burst**. See [Burst Effects](https://dev.epicgames.com/documentation/fortnite/using-vfx-spawner-devices-in-fortnite-creative#burst-effects) for a list of available effects.

**Sound Effect**

**Default**, None, Pick a sound

Determines what sound plays when the visual effect is spawned. **Default** plays whatever sound is attached to a visual effect (such as **Lightning**), but you can override the default by picking a different option. Some of the sounds are a short burst, while others are continuous. See the **Sound Effects** section for a list of available sounds.

**Enabled on Phase**

None, **Always**, Pre-Game Only, Gameplay Only, Create Only

Determines the phases in which the device is enabled.

**Colorize VFX**

*On*, **Off**

Sets whether the spawned effects use the color selected in the **Custom Color** option. This is useful if you want to assign colors to your effects based on teams. If set to **On**, this makes the next option, **Custom Color**, available

**Custom Color**

**Cerulean**, Pick a color

Choose a custom color for the VFX. Click the color swatch to open the Color Picker. Select a color, then click the checkmark. Note that this option only displays when the **Colorize VFX** option is set to **On**.

**Visible to Team**

**Any**, Pick or enter a team

Determines which team can see the VFX.

**Invert Team Selection**

On, **Off**

If this is set to **On**, all teams can see the VFX except the team selected in the **Visible to Team** option.

**Visible to Class**

No Class, All, **Any**, Pick or enter a class

Determines which classes can see the VFX.

Values for this option are:

-
**No Class**: Only players without an assigned class can see this effect.

-
**All**: All players with an assigned class can see this effect.

-
**Any**: All players, with or without an assigned class, can see the effect.

-
**Pick or enter a class**: Only players on the selected class can see the effect.

**Invert Class Selection**

On, **Off**

If this is set to **On**, all classes can see the VFX except the class selected in the **Visible to Class** option.

**Spawn Rate**

**1.0**, Pick or enter a number

Determines the rate at which the effects are spawned.

**Enable on Reset**

**On**, Off

If this is set to **On**, the disabled device will automatically be enabled when the **Reset When Receiving From** function is triggered.

**Enabled Time**

**Infinite**, Pick an amount

The length of time the visual effect is enabled.

**Clear Particles on Disable**

**On**, Off

If this is set to **On**, spawned effects will be cleared when the device is disabled. If it is set to **Off**, spawned particles will be cleared at the end of their animation.

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

##### Enable When Receiving From

This function enables the device when an event occurs.

##### Disable When Receiving From

This function disables the device when an event occurs.

##### Restart When Receiving From

This function resets the device when an event occurs.

#### Events

Direct event binding uses events as transmitters. An event tells another device to perform a function.

-
For any event option, click the **option**, then **Select Device** to access and select from the **Device dropdown menu**.

-
Once you've selected a device, click **Select Function** to bind the event to a function for that device.

-
If more than one function is triggered by the event, press the **Add** button and repeat.

**אפשרויות ותיאורים:**

##### On Effect Enabled Send Event To

When an effect is enabled, an event occurs.

##### On Effect Disabled Send Event To

When an effect is disabled, an event occurs.

### Continuous Effects

Here is a list of the currently available continuous visual effects.

-
**Fireworks**: Fireworks that go off randomly near the device, with sound effects.

-
**Large Fireworks**: Fireworks that go off randomly but high in the sky, with sound effects.

-
**Leaves**: Leaves that drift through the air, giving a sense of autumn.

-
**Eyes**: A collection of creepy eyes, that might be peering out of the darkness.

-
**Bats**: Bats flying through the air evoke Halloween.

-
**Lightning**: Lightning striking the ground, with sound effects.

-
**Lightning_2**: Lightning bolts going away from the device, with sound effects.

-
**Lightning_3**: Lightning striking the ground with an explosion on impact, including sound effects.

-
**Embers**: Small embers floating up, as though from an open fire.

-
**Fog**: A drifting pattern of fog.

-
**Sparkles**: Sparkly bits of light that move around.

-
**Disco Balls**: An assortment of mirrored balls of varying sizes.

-
**Laser Beams**: Focused, moving beams of light that shoot out of the top of the device.

-
**ConcertRain**: Falling lights that suggest a mix of meteorites and distant strikes of lightning.

-
**SparkRain**: Colorful rainfall that includes sound effects.

-
**Area of Fog**: Ground-level clouds of fog that move continually.

-
**Spooky Ghosts**: Ghostly figures that move in and out of the player's vision in a spooky fashion.

-
**Balloons**: Colorful balloons that float up into the sky until they cheerfully disappear.

-
**Snow**: A gentle sprinkle of snow.

-
**Floating Space Rocks**: Space rocks (meteorites) that float mysteriously in the air.

-
**Bubbles**: Iridescent bubbles that look like they're fresh from a bubble machine.

-
**Falling Sparkles**: Similar to sparkles, but instead of moving around, they're slowing falling to the ground.

-
**Confetti**: Falling bits of paper — perfect for a parade!

-
**Flying Space Rocks**: Space rocks (meteorites) falling from the sky.

-
**Dust Clouds**: Imagine moving across a dune on a dirt bike. These are the clouds your bike might kick up.

-
**Rain**: A steady drizzle of rain.

-
**Small Tornado**: A tornado that spins upward.

-
**Light Fog**: A fog light enough to see through easily.

-
**Sky Lanterns**: Colorful paper lanterns you might see rising over a pond or lake for a festival.

-
**SkyLanterns_A**: Like the previous lanterns, but these are all red.

-
**SkyLanterns_B**: Like the previous lanterns, but all blue.

-
**SkyLanterns_C**: Like the previous lanterns, but all green.

-
**Waterfall Crash**: Roiling water like what appears at the bottom of a high waterfall.

-
**Waterfall Splash**: Splashing water like what you might see at the foot of a smaller waterfall.

-
**Waterfall Mist**: A light mist like you'd find at the edge of a gentle waterfall.

-
**Musical Notes Bubbles**: Musical notes that act like bubbles and pop.

-
**Musical Notes Chrome**: Notes with a metallic sheen.

-
**Musical Notes Goo**: Notes that are dripping a black goo.

-
**Musical Notes Retro**: Notes that look three-dimensional.

-
**Musical Notes Glitch**: Notes that look like the colors are out of register, and that have odd, glitchy behavior.

-
**Musical Notes Wood**: Notes that look like they're carved from wood.

-
**Small Fire**: A small fire effect, like you might use with a torch or brazier.

-
**Trash Can Flies**: A cloud of flies that would typically be seen around a garbage pile or container.

-
**Ambient Dust**: Flecks of material floating in a random way, such as dust particles that hang in the air in an old abandoned building.

### Burst Effects

Here is a list of the currently available burst effects.

-
**Explosion Small**: A small explosion with sound effects.

-
**Explosion Medium**: A slightly larger explosion with sound effects.

-
**Explosion Large**: An even larger explosion with sound effects.

-
**Explosion Electrical**: A large explosion with sound effects that mimics a transformer blowing or a similar electrical explosion.

-
**Dust Poof**: A light poof of dust, enough to partially hide the spawning of a new effect.

-
**Small Splash**: A limited, small splash such as that made by dropping or throwing a small object into water.

### Sound Effects

Here is a list of the currently available sound effects you can use with your visual effect.

-
**Default**: Uses any sound effects that are attached to a visual effect. If none are attached, then the effect is silent.

-
**None**: Turns off any default sound effects.

-
**Alpine**: Suggests wind moving briskly through an snowy forest.

-
**Alpine_Evening**: Similar to Alpine, but with a hollower and more resonant tone.

-
**Alpine_Morning**: Similar to Alpine, but with a softer and higher pitched whistling sound.

-
**Bats**: The sound of bats soaring through the air. Works well with the Bats effect.

-
**Beam**: A continuous rumble and whine that rises and falls in pitch. Could be used with the Laser Beam effect, or used for a rocket ignition.

-
**Beam_Attack**: Similar to the Beam, but this sound is a short burst.

-
**Beam_Impact**: This sound is also a short burst. Either Beam Attack or Beam Impact could be used for a laser weapon hitting a target.

-
**Breeze**: Unlike Alpine, which is a brisk winter or snowy wind, this is gentler and slower, suggesting a warm breeze swaying the treetops.

-
**Fireworks**: A short boom, trailing off into crackling.

-
**Charge**: A large rumbling, leading into higher pitched whizzing.

-
**Charged_Attack**: A larger, more intense rumble followed by crackling instead of whizzing.

-
**Charge_Loop**: A slowly building, rising whine looped to stretch out the rising tone.

-
**Ghost**: A ghost moaning.

-
**Halloween_Laugh**: An eerie laugh.

-
**Halloween_Singing**: A voice singing wordlessly in a minor key, in a large echoing space. This is randomized, slightly different each time it plays.

-
**Halloween_Whispers**: Unintelligible murmuring that may be human or machine, with distant laughter.

-
**Lightning_Strike**: The sound of lightning striking.

-
**Lightning_Strike_02**: A variation of the lightning strike, with slightly different impact sound.

-
**Lightning_Strike_03**: A variation of the lightning strike, with slightly different impact sound from the two other lightning strike effects.

-
**Lightning_Strike_04**: A variation of the lightning strike, with slightly different impact sound from the two other lightning strike effects.

-
**Electricity**: A crackling and buzzing sound, like a Tesla coil.

-
**Electricity_02**: A longer and quieter crackling, buzzing sound. Similar to the sound of laser swords swinging and connecting.

-
**Electricity_03**: Like Electricity 2, but with interrupting staccato zaps or shots.

-
**Electricity_04**: A solid ka-chunk with quiet buzzing in the background, as if you are throwing a large switch or breaker.

-
**Electricity_05**: Similar to Electricity 4, but louder. Could be an explosion or shot as much as it could be a switch thrown.

-
**Electricity_06**: Similar to Electricity, but smoother and with less crackling.

-
**Explosion**: A small detonation, or a gun going off.

-
**Explosion_02**: A large detonation, or a large gun or cannon firing.

-
**Explosion_03**: A quieter large detonation, like a cannon firing from a distance.

-
**Impact**: The sound of an small or medium sized object hitting a floor or wall.

-
**Impact_02**: An impact with some rattling, like a full bag hitting a floor or wall.

-
**Impact_03**: An impact with sounds of breaking or destruction.

-
**Impact_04**: A short muffled thud.

-
**Impact_05**: Another cannon shot, at medium distance.

-
**Impact_06**: A sharper gun shot sound.

-
**Impact_Junk**: The sound of junk (metal and glass) being tossed around and broken, or of something landing on a junk pile.

-
**Impact_Squish**: A thud ending in squelching sounds, like a thrown object landing on something wet.

-
**Electric_Blast**: Like Electricity combined with Explosion 2 or 3. Impact or blasting sound, but accompanied by buzzing and crackling.

-
**Jolt**: A very short zap, like an energy weapon blast.

-
**Whistling_Projectiles**: A sound like a rocket or missile passing by, but with no impact sound at the end.

-
**Ominous_Loop**: An eery, resonant instrumental chord. Dies out, then comes back.

-
**Projectile**: Like Whistling Projectiles, but with a larger number of missles or rockets, at varying distances.

-
**Night_Wind**: A high wind on a moor or a plain, with soft squeals and moans mixed in.

-
**Steamy_Vent**: The sound of liquid boiling, with a whistling sound like steam escaping through a small hole.

-
**Storm**: A loud rumbling mixed with electric buzzing and crackling.

-
**Spooky_Laugh**: High pitched, echoing laughter.

-
**Vent_Launch**: A burst of air, sound of a vent releasing.

-
**Weak_Point**: The creaking sound of metal breaking.

-
**Wind**: Similar to Alpine or Breeze, but with a louder burst like a gust of wind.

-
**Woosh**: A wooshing sound, like something passing by very fast.

-
**Woosh_02**: The sound of an object being swung past you very fast, such as a sword.

-
**Splash**: An impact sound and light splash, as if something had been thrown into a liquid.

-
**Impact_Soft**: A very quiet impact, like a small object landing on a soft surface.

-
**Pickup**: Something being picked up.

-
**Pickup_02**: Like Pickup, but even quieter.

-
**Pickup_03**: Like Pickup, but with quiet rustling like cloth.

-
**Fuse**: A crackling or fizzling sound, like a long fuse on a bomb.

-
**Heal**: A quiet high pitched ringing with a deeper hum underneath it, on a loop.

-
**Health_Field**: A background sound similar to the Heal sound, but with crackling sounds of impacts on top of it.

-
**Healing_Grenade_Underwater**: A plop into water followed by air bubbles moving up to the surface.

-
**Health_Zone**: Similar to Heal, but barely audible and with a more resonant background hum.

-
**Heal_Serene**: Similar to Health Zone, but instead of ringing there is high pitched chimes or voices on top.

-
**Heal_Tranquil**: Very faint ringing, with a higher pitched resonant hum similar to running your finger around the rim of a glass.

-
**Burn**: The sound of a crackling fire.

---

## Using Visual Effect Powerup Devices in Fortnite Creative

**כותרת מקורית:** Using Visual Effect Powerup Devices in Fortnite Creative  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/using-visual-effect-powerup-devices-in-fortnite-creative  
**מקור קלט:** `07F_דמויות_AI_תאורה_סביבה_וVFX(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `using-visual-effect-powerup-devices-in-fortnite-creative`

Use **Visual Effect Powerups** to trigger a visual effect (a glow or an outline) when a player picks something up, or does something noteworthy.

Powerups can be triggered by player interaction, or by binding the effect to another device.

For example, you can set the Visual Effect Powerup to be triggered when a player picks up a Health Powerup, and [grant](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#grant) the player [health](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#health) and a green glow (the effect).

To find the Visual Effect Powerup device, go to the **Creative inventory** and select the **Devices** tab. From there, you can search or browse for the device. For more information on finding devices see [Using Devices](https://dev.epicgames.com/documentation/fortnite/using-devices-in-fortnite).

If you're using multiple copies of a device on an island, it can be helpful to [rename](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#rename-a-device) them. You can choose names that relate to each device’s purpose, so it’s easier to remember what each one does.

### Contextual Filtering

Some devices are affected by a feature called **contextual filtering**. This feature hides or displays options depending on the values selected for certain related options. This reduces clutter in the Customize panel and makes options easier to manage and navigate. To help identify them, values that trigger contextual filtering are in *italic*.

All options are listed, including those affected by contextual filtering; if they are hidden or displayed based on a specific option's value, there will be a note about it in the Description field for that option.

### Device Options

This device has some basic functionality, like choosing the type of visual effect, the color, the duration, and the [respawn](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#respawn) time. Additionally, there are some advanced options, like [class](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#class) and team restrictions, and visibility restrictions.

Default values are **bold**. Values that trigger contextual filtering are *italic*.

You can configure this device with the following options.

 Option Value Description
**Infinite Effect Duration**

**No**, *Yes*

If set to **Yes**, the effect will remain indefinitely. If **No**, you can set the duration of the effect in the next option.

**Effect Duration**

**3 seconds**, Infinite, Pick a duration

The amount of time the applied effect will stay active for.

**Disables Effect on Pickup**

Yes, **No**

If this is set to **Yes** then the effect of this powerup will be canceled when the powerup is collected.

**Pickup Radius**

**On Touch**, Pick a distance

The distance in meters the player needs to be from the powerup to collect it.

**Respawn**

**Yes**, *No*

If set to **Yes**, you can set the respawn time in the next option. If set to **No**, it will never respawn.

**Time to Respawn**

Never, Instant, **15 seconds**, Pick a time

The amount of time after pickup for this item to respawn.

**Spawn on Minigame Start**

**Yes**, No

When the minigame starts, is the powerup immediately spawned? If set to **No**, the powerup will spawn after its respawn time.

**Ambient Audio**

**On**, Off

Plays audio when players are nearby.

**Pickup Audio**

**On**, Off

Plays audio when picking up powerup.

**Selected Class**

**Any**, Pick a class

Specifies which Class can interact with this powerup.

**Selected Team**

**Any**, Pick a team

Specifies which Team can interact with this powerup.

**Apply To**

**Player**, Player’s Team, Player’s Class, Same Class in Player’s Team, All Players

The powerup effect will be applied to the selected receiver.

**Who Can See This Powerup**

None, All, **Only Players Who Can Pick Up**

Only the selected players will be able to see this powerup.

**Visual Effect**

**Glow**, Outline

Apply this VFX to the player that picks up this powerup.

**Color Type**

Team Relationship, Team Color, **White**, Pick a color

Which color is applied.

**Team Color** applies the color of the target’s team.

**Team Relationship** applies red if it’s hostile, green if it’s neutral and blue if it’s friendly.

**Custom Color**

**#00000000**, Select a color

Click the color number to open the Color Picker. Click a color to select.

**Is Effect Visible to Local Player**

**Visible to Local Player**, Not Visible to Local Player

If the effect is not visible on the local player, then the local player will see this effect on other players but not themselves.

**Team Relationship Visibility**

**Everyone**, Only Owning Player’s Team

Whether the effect is visible to everyone, or only the owning player’s team.

### Direct Event Binding

Following are the [direct event binding](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#direct-event-binding) options for this device.

#### Functions

A [function](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#function) listens for an event on a device then performs an action.

-
For any function, click the option, then Select Device to access and select from the Device dropdown menu.

-
Once you've selected a device, click Select Event to bind the device to an event that will trigger the function for the device.

-
If more than one device or event triggers a function, press the Add button to add a line and repeat these steps.

**אפשרויות ותיאורים:**

##### Spawn When Receiving From

Immediately spawns the powerup when an event occurs.

##### Despawn When Receiving From

Immediately despawns the powerup when an event occurs. This powerup will not spawn again until activated by the **Spawn When Receiving From** function.

##### Pickup When Receiving From

Picks up the powerup when an event occurs, and applies the effect through other devices.

##### Clear When Receiving From

Clears any effects for this powerup when an event occurs

#### Events

Direct event binding uses events as transmitters. An event tells another device to perform a function.

-
For any event option, click the **option**, then **Select Device** to access and select from the **Device dropdown menu**.

-
Once you've selected a device, click **Select Function** to bind the timer to a function for that device.

-
If more than one function is triggered by the event, press the **Add** button and repeat.

**אפשרויות ותיאורים:**

##### On Item Picked Up Send Event To

Sends an event to a linked device when a player picks up the powerup.

---

## Using Wildlife Spawner Devices in Fortnite Creative

**כותרת מקורית:** Using Wildlife Spawner Devices in Fortnite Creative  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/using-wildlife-spawner-devices-in-fortnite-creative  
**מקור קלט:** `07F_דמויות_AI_תאורה_סביבה_וVFX(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `using-wildlife-spawner-devices-in-fortnite-creative`

The **Wildlife Spawner** device can be customized to [spawn](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) various animals.

Animals you can spawn using this device include:

-
Sky Jelly

-
Wildwasps

-
Spring Chicken (Prey)

-
Chicken (Prey)

-
Frog

-
Boar (Prey)

-
Wolf (Predator)

-
Raptor (Predator)

-
Air Sprite

-
Water Sprite

-
Dash Sprite

Players can hunt for the prey animals (chickens and boars), which will drop resources (such as meat) when they are eliminated. Some animals spawned by this device can be tamed and ridden by players:

-
Boars

-
Wolves

-
Raptors

To tame an animal, you can just jump on its back when it is near you. Once an animal is tamed, it will follow the player at a distance and can be used as a mount. Some will attack other players and animals that are hostile to the player that tamed them. Players can tame up to three animals at a time. The **Raptor** can also jump while being ridden, and have a very high jump height. This can be used with the environmental design on your island to introduce traversal puzzles, secret areas or loot, and other variations in gameplay and movement.

You can also select a different appearance for some animals, to match the biome of your island. Animals that have biome variants include:

-
Chicken

-
Boar

-
Wolf

-
Sprites

Use the **Biome Variant** option to change the appearance of the animals spawned. Choices are listed in the Device Options section, below.

While there isn't a limit on the number of Wildlife Spawners you can have on an island, there is a limit on the total number of spawned AI enemies on an island. This includes creatures, guards, and wildlife. You can only have 90 AI enemies active at a time, across all devices that spawn AI enemies. If you have a lot of Wildlife Spawners, or if you also have Guard or Creature Spawners on your island, keep track of the number of enemies each is spawning so you stay under the overall limit.

For help on how to find the **Wildlife Spawner** device, see [Using Devices](https://dev.epicgames.com/documentation/fortnite/using-devices-in-fortnite).

If you're using multiple copies of a device on an island, it can be useful to [rename](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) them. Choosing names that relate to a device's purpose makes it easier to remember what each one does, and easier to find a specific device when using the [Event Browser](https://dev.epicgames.com/documentation/fortnite/event-browser-in-fortnite-creative).

### Contextual Filtering

Some devices are affected by a feature called contextual filtering. This feature hides or displays options depending on the values selected for certain related options. This feature will reduce clutter in the Customize panel and make options easier to manage and navigate. However, it may not be easy to recognize which options or values trigger contextual filtering.

To help you identify them, in our device docs we use *italic* for any values that trigger contextual filtering. All options will be listed, including those affected by contextual filtering; if they are hidden or displayed based on a specific option's value, there will be a note about that in the **Description** field for that option.

### Device Options

This device has some basic functionality, like choosing the type of animal, choosing the biome variant, and how many animals spawn. There are also advanced options, like setting the total number of animals spawned, and how much health each animal has.

You can configure this device with the following options.
**

Default values are **bold**. Values that trigger contextual filtering are *italic*.

 Option Value Description
**Type**

Sky Jelly, Wildwasps, Spring Chicken, *Chicken*, Frog, *Boar*, ***Wolf***, Raptor, *Air Sprite*, *Water Sprite*, *Dash Sprite*, Random, Random Prey, Random Predator

Determines the type of animal that is spawned. The shape of the device changes to match the type of animal that spawns. If you choose **Chicken**, **Boar**, Sprit****e**, or **Wolf** the **Biome Variant** option is displayed below this one.

**Biome Variant**

**Classic**, Medieval, Snow

This option only displays if you have chosen **Chicken**, **Boar**, or **Wolf** in the **Type** option. Determines which variant color is used for animals spawned from this device.

**Spawn Count**

**4**, Pick a number

Determines the maximum number of animals that can be active at once. When activated, the spawner produces one animal at a time, up to the maximum number selected. Islands can have a maximum of 30 wildlife spawned and active at a time, across all Wildlife Spawner devices.

**Allow Infinite Spawn**

**Yes**, *No*

Determines if this device should restrict the maximum number of wildlife spawned in its lifetime.

**Total Spawn Limit**

**10**, Pick or enter a number

This option only displays if the **Allow Infinite Spawn** option is set to **No**. Sets the maximum number of wildlife this spawner can produce during its lifetime.

**Spawn on Timer**

***On***, Off

Determines if wildlife should be spawned on a timer, or only when receiving events.

**Spawn Timer**

**3 seconds**, Pick a number

This option only displays if the **Spawn on Timer** option is set to **On**. Determines the minimum amount of time between wildlife spawns.

**Spawn Through Walls**

**On**, Off

Determines whether animals must spawn within the [line of sight](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) of the device, or if they can spawn behind walls that obstruct the line of sight.

**Spawn Radius**

**10.0M**, Pick or enter an amount

The maximum distance from the device that the Wildlife can spawn.

**Activate from Any Distance**

**Yes**, *No*

Determines if this device requires that a player be within a specified distance in order to spawn wildlife.

**Activation Distance**

**5M**, Pick a distance

This option only displays if the **Activate from Any Distance** is set to **No**. Determines the distance from the spawner that a player must be within for wildlife to begin spawnning.

**Tamed Follow Distance**

**Default**, Pick a distance

Determines the distance from the taming player that wildlife will try to remain within while tamed.

**Wander Range**

**Default**, Pick a distance

Determines the distance from the device that a wildlife can range peacefully. A wildlife may be pulled out of this range when fleeing, engaging in combat, or pursuing a goal. Wildlife pulled far enough outside of the **Wander Range** will not return.

**Enabled On Game Start**

**Enabled**, Disabled

Determines whether the device is enabled when the game starts.

**Force Spawn**

**Never**, On Timer Only, On Spawn Event Only, Always

Determines if this device should spawn new wildlife when it is at its **Number of Wildlife** cap. When a new wildlife is spawned this way, the oldest wildlife from this device will be eliminated.

**Custom Damage**

**Default**, Pick an amount

Sets the amount of damage the Wildlife from this device can do to others.

**Custom Damage to Player**

**Default**, Pick an amount

Sets the amount of damage the wildlife from this device can do to players. If this option is set to anything other than **Default**, this will override the value set in the **Damage** option.

**Custom Damage to Environment**

**Default**, Pick an amount

Sets the amount of damage wildlife from this device can do to the environment.

**Custom Movement Speed Multiplier**

Very Slow, Slow, **Default**, Fast, Very Fast

Sets the multiplier applied to the movement speed of spawned animals.

**Invincible**

Yes, ***No***

Determines if wildlife spawned from this device can take damage.

**Starting Health**

**Default**, Pick an amount

This option only displays if the **Invincible** option is set to **No**. Sets the maximum health value for spawned animals.

**Taming**

**Enabled**, Disabled

Determines whether animals spawned by this device can be tamed by players.

**Maximum Tamed Wildlife**

**Default**, 1, 2, 3

Determines the limit of wildlife from this device that a player can tame in game. Default means applying the same option set in the island settings. The device's tame limit won't be larger than the island setting limit.

**Can Drop Loot**

**Yes**, No

Determines whether spawned animals drop resources when they are eliminated.

**Riding**

*Enabled*, **Disabled**

Determines whether tamed wildlife spawned from this device can be ridden. If you choose **Enabled**, several other options display below this one in the Customize panel.

**Allow Riding on Different Teams**

**On**, Off

Determines if the Wildlife spawned by this device can only be ridden by the players on the same team or not.

**Starting Energy**

**100\%(Default)**, Pick a percentage

This option only displays if the **Riding** option is set to **Enabled**. Determines the starting energy value for the rideable wildlife spawned from this device.

**Maximum Energy**

**100\%(Default)**, Pick a percentage

This option only displays if the **Riding** option is set to **Enabled**. Determines the maximum energy value for the rideable wildlife spawned from this device.

**Energy Restore Amount**

**None**, Pick a percentage

This option only displays if the **Riding** option is set to **Enabled**. Determines the amount of energy restored when the associated functions are triggered.

**Energy Consume Amount**

**None**, Pick a percentage

This option only displays if the **Riding** option is set to **Enabled**. Determines the amount of energy consumed when a player rides wildlife spawned by this device.

**Prevent Player Dismounting**

**Off**, On

Determines if players are able to use the interact control to dismount. If you set this to **On**, player cannot dismount using the interact control and cannot dismount by jumping off the mount. They can still be dismounted by functions.

**Wildlife Team Type**

Team Index, **Team Wildlife & Creatures**, Team Neutral

Determines which team Wildlife are assigned to.

**Wildlife Team Index**

**Team 1**, Pick or enter a team

If the **Wildlife Team Type** is set to **Team Index**, this option sets the Team Index Wildlife are assigned.

**Spawn on Patrol Path**

0, Select a path number

Spawns wildlife on the selected Patrol Path Group.

Selecting a Patrol Path Group number other than 0 causes new options to become available, such as: Enable Resuming Patrol Path, and Change Patrol Path Target.

**Enable Resuming Patrol Path**

**On**, Off

Determines if the wildlife should resume patrolling their path if it was disabled and then enabled.

If set to **Off**, the wildlife must be assigned a path through a path's "Assign AI To Path" function to continue path following.

**Change Patrol Path Target**

**Never**, *On Spaw*n, *On Timer*

Determines how often the spawner will select a new random Patrol Path within its Patrol Path Group.

If set to NEVER, the device will always use the first Patrol Path in the Patrol Path Group.

Using any value other than Never causes further options to become available.

**Change Patrol Path Timer**

1.0, Select a time

This option becomes available when the

Change Patrol Path Timer is selected.

Determines the amount of time newly spawned Wildlife will be selecting the Patrol Path.

After it ends, newly spawned Wildlife will randomly select Patrol Path. This won't impact Wildlife that have already spawned.

**Should Randomly Select Path**

**On**, Off

This option becomes available when

Change Patrol Path Target is selected.

Determines if the device should randomly select a path to use. If set to Off, the device will select the path in order of their indexes if they have been set, or on the path that has not had Wildlife spawned on it, which resets after a Wildlife has spawned on each Patrol Path in the Patrol Group.
**

If multiple paths have the same index they will be randomly ordered between themselves.

Sprite Activations**

0, Select activations amount

This option becomes available when the Type option is set to one of the Sprite types.

### Direct Event Binding

Following are the [direct event binding](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) options for this device.

#### Functions

A [function](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) listens for an event on a device then performs an action.

-
For any function option, click the **option**, then **Select Device** to access and select from the **Device dropdown menu**.

-
Once you've selected a device, click **Select Event** to bind the timer to an event that will trigger the function for the device.

-
If more than one device should be affected by a function, press the **Add** button and repeat.

**אפשרויות ותיאורים:**

##### Enable When Receiving From

This function enables the device when an event occurs.

##### Disable When Receiving From

This function disables the device when an event occurs.

##### Spawn When Receiving From

This function spawns an animal when an event occurs.

##### Despawn When Receiving From

This function despawns an animal when an event occurs.

##### Destroy Spawner When Receiving From

This function destroys the spawner when an event occurs.

##### Tame When Receiving From

This function tames a spawned animal when an event occurs.

##### Untame All When Receiving From

This function untames all spawned animals when an event occurs.

##### Untame from Instigator When Receiving From

This function untames all animals tamed by the instigator when an event occurs.

##### Reset Total Spawn Count When Receiving From

This function resets the total spawn amount when an event occurs.

##### Eliminate Tamed from Instigator When Receiving From

This function eliminates the instigator's tamed animals when an event occurs.

##### Ride When Receiving From

This function teleports the nearest ridable wildlife to the instigator and mounts the instigator on it.

##### Dismount All When Receiving From

This function dismounts all players from all wildlife spawned by this device.

##### Dismount Instigator When Receiving From

This function dismounts the instigator from all wildlife spawned by this device.

##### Restore Energy for All When Receiving From

This function restores the amount of energy defined in the **Energy Restore Amount** option to all riding players.

##### Restore Energy for Instigator When Receiving From

This function restores the amount of energy defined in the **Energy Restore Amount** option to the instigating player.

##### Consume Energy for All When Receiving From

This function consumes the amount of energy defined in the **Energy Consume Amount** option from all players.

##### Consume Energy for Instigator When Receiving From

This function consumes the amount of energy defined in the **Energy Consume Amount** option from the instigator.

#### Events

An [event](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) tells another device when to perform a function.

-
For any event option, click the **option**, then **Select Device** to access and select from the **Device dropdown menu**.

-
Once you've selected a device, click **Select Function** to bind the timer to a function for that device.

-
If more than one device is affected by the function, press the **Add** button and repeat.

**אפשרויות ותיאורים:**

##### On Spawned Send Event To

When this device spawns wildlife, an event occurs, triggering the selected function.

##### On Eliminated Send Event To

When wildlife spawned by this device are eliminated, an event occurs, triggering the selected function.

##### On Tamed Send Event To

When wildlife spawned by this device are tamed, an event occurs, triggering the selected function.

##### On Untamed Send Event To

When wildlife spawned by this device are untamed, an event occurs, triggering the selected function.

##### On Force Spawned Send Event To

When wildlife is force spawned from this device, an event occurs, triggering the selected function. This causes the oldest wildlife spawned to be eliminated.

##### On Eliminated by A Neutral Player Send Event To

When untamed wildlife spawned from this device are eliminated by a neutral player, an event occurs, triggering the selected function.

##### On Eliminated by An Enemy Player Send Event To

When tamed wildlife spawned from this device are eliminated by an enemy player, an event occurs, triggering the selected function.

##### On Eliminated by Predator Send Event To

When wildlife spawned by this device are eliminated by a Predator, an event occurs, triggering the selected function.

##### On Damaged Send Event To

When wildlife spawned from this device are damaged, an event occurs, triggering the selected function.

##### On Something Is Eaten Send Event To

When wildlife spawned from this device eat a food item, an event occurs, triggering the selected function.

##### On Ridden Send Event To

When wildlife spawned from this device are ridden, an event occurs, triggering the selected function.

##### On Dismounted Send Event To

When wildlife spawned from this device are dismounted, an event occurs, triggering the selected function.

##### On Eliminating Send Event To

When wildlife spawned from this device are eliminated, an event occurs, triggering the selected function.

##### On Picked Up Send Event To

When wildlife spawned from this device are picked up by a player, an event occurs, triggering the selected function. This works with Chickens and Spring Chickens.

##### On Placed Send Event To

When wildlife spawned from this device are placed by a player after being picked up, an event occurs, triggering the selected function. This works with Chickens and Spring Chickens.

##### On Thrown Send Event To

When wildlife spawned from this device are thrown by a player after being picked up, an event occurs, triggering the selected function. This works with Chickens and Spring Chickens.
