# שחקנים, קבוצות, Classes, מצלמות וסבבים

> **מטרת הקובץ:** לרכז את ניהול השחקנים, Teams, Classes, Spawn, מצלמות, Controls ו־Round Settings Device.  
> **מתי להשתמש בו:** כאשר מגדירים תפקידים, קבוצות, נקודות הופעה, שליטה במצלמה או התנהגות בין סבבים.  
> **לא כלול:** Round Settings ברמת האי, HUD כללי ומטרות או ניקוד.  
> **מקורות עיקריים:** `04_עיצוב_משחק_שלבים_והכוונת_שחקנים(1).md`, `07C_שחקנים_קבוצות_תפקידים_ומצלמות(1).md`

## תוכן עניינים

- [Designing with Cameras and Controls in Fortnite Creative](#designing-with-cameras-and-controls-in-fortnite-creative)
- [Using Class Designer Devices in Fortnite Creative](#using-class-designer-devices-in-fortnite-creative)
- [Using Class Selector Devices in Fortnite Creative](#using-class-selector-devices-in-fortnite-creative)
- [Using Class Selector UI Devices in Fortnite Creative](#using-class-selector-ui-devices-in-fortnite-creative)
- [Using Down But Not Out Devices in Fortnite Creative](#using-down-but-not-out-devices-in-fortnite-creative)
- [Using First Person Camera Devices in Fortnite Creative](#using-first-person-camera-devices-in-fortnite-creative)
- [Using Fixed Angle Camera Devices in Fortnite Creative](#using-fixed-angle-camera-devices-in-fortnite-creative)
- [Using Fixed Point Camera Devices in Fortnite Creative](#using-fixed-point-camera-devices-in-fortnite-creative)
- [Using Orbit Camera Devices in Fortnite Creative](#using-orbit-camera-devices-in-fortnite-creative)
- [Using Player Checkpoint Devices in Fortnite Creative](#using-player-checkpoint-devices-in-fortnite-creative)
- [Using Player Marker Devices in Fortnite Creative](#using-player-marker-devices-in-fortnite-creative)
- [Using Player Movement Devices](#using-player-movement-devices)
- [Using Player Reference Devices in Fortnite Creative](#using-player-reference-devices-in-fortnite-creative)
- [Using Player Spawn Pad Devices in Fortnite Creative](#using-player-spawn-pad-devices-in-fortnite-creative)
- [Using Round Settings Devices in Fortnite Creative](#using-round-settings-devices-in-fortnite-creative)
- [Using Side Scroller Controls Devices in Fortnite Creative](#using-side-scroller-controls-devices-in-fortnite-creative)
- [Using Team Settings and Inventory Devices In Fortnite Creative](#using-team-settings-and-inventory-devices-in-fortnite-creative)
- [Using Third Person Controls Devices in Fortnite Creative](#using-third-person-controls-devices-in-fortnite-creative)

---
## Designing with Cameras and Controls in Fortnite Creative

**כותרת מקורית:** Designing with Cameras and Controls in Fortnite Creative  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/designing-with-cameras-and-controls-in-fortnite-creative  
**מקור קלט:** `04_עיצוב_משחק_שלבים_והכוונת_שחקנים(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `designing-with-cameras-and-controls-in-fortnite-creative`

*

*Learn to use this **Beta** feature, but use caution when shipping with it.

The player's perspective can change everything about a game: a dynamic camera can intensify the sense of action, making intense moments more exhilarating, while a fixed viewpoint can create suspense and terror. Switching between cameras can intensify emotions, or create a deeper connection between the player and the in-game character. Carefully selecting different camera perspectives can significantly shape the player's engagement, emotional investment, and overall enjoyment of their gaming experience.

On this page, you will learn about how each type of camera can be used, and how to adjust the controls for the kind of gameplay you’re looking to make.

For more information on each of the devices covered here, see:

-
[Fixed Point Camera device](https://dev.epicgames.com/documentation/fortnite/using-fixed-point-camera-devices-in-fortnite-creative)

-
[Fixed Angle Camera device](https://dev.epicgames.com/documentation/fortnite/using-fixed-angle-camera-devices-in-fortnite-creative)

-
[Third Person Controls device](https://dev.epicgames.com/documentation/fortnite/using-third-person-controls-devices-in-fortnite-creative)

-
[First Person Mode Controls device](https://dev.epicgames.com/documentation/fortnite/using-first-person-camera-devices-in-fortnite-creative)

Please note that, when switching cameras, the **Third Person Controls** device must be used to retain control over the player character. This will be covered in more detail in the [Adapting Controls](https://dev.epicgames.com/documentation/fortnite/designing-with-cameras-and-controls-in-fortnite-creative) section.

### Fixed Point Cameras

Fixed point cameras maintain a predetermined location and angle throughout gameplay or in specific areas. These cameras adjust dynamically to player actions.

Fixed point cameras are useful in a variety of situations, some of which are explored below.

#### Using a Static Camera for Mini Games

Static cameras remain completely still, capturing a specific view of the game environment. They often provide a consistent perspective and can be used to create compelling mini games.

In the following example, the Fixed Camera device is used for a party game. Players must remain on the platform for as long as possible while trying to get the other players off the platform and avoid cannonballs.

Notice how the camera slightly follows the player as they move around the floating platform.

The fixed camera in this example uses the following modified settings:

 Option Value Description
**Field of View**

50.0

The degrees of the vertical axis that the camera can view.

**Look at Offset Distance**

1.2

Moves the camera a bit forward, offsetting the view [target](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#target).

**Look at Offset Horizontal**

0.24

Moves the camera left or right, offsetting the view target.

**Look at Offset Vertical**

0.24

Moves the camera up or down, offsetting the view target.

**Yaw Accelerations**

0.24

Determines how fast the camera accelerates left or right towards the target, 0 being instant.

**Pitch Acceleration**

0.24

Determines how fast the camera accelerates up or down towards the target, 0 being instant.

In order for players to be able to aim their weapons and have their characters change direction, a **Player Controller **device is placed in the level with the default settings.

#### Using Multiple Fixed Cameras for Added Suspense

Use multiple fixed cameras positioned strategically throughout the level in any game where you want to build tension. In this example, as the player progresses the game switches between these camera perspectives to reveal different aspects of the environment. This naturally builds suspense because players don't know what may be hiding behind the next corner!

As a player enters a **Mutator Zone** device, the fixed camera linked to this zone is added to the player.

If you're working in UEFN, it can be helpful to use the **World** setting with the transform gizmo when you’re placing cameras. This ensures they stay level to the ground.

As the player moves from one mutator zone to another, the cameras get added and removed to match the player’s location. Since the basement is a closed space with only one exit, a **Trigger** device on the floor is used instead of a mutator zone.

The Fixed Camera devices in this example use the following modified settings:

 Option Value Description
**Add to Players on Start**

False

Players are added to cameras through their interaction with devices.

**Transition In Time**

0.0

To create a more dramatic effect, transitions between cameras are instantaneous.

**Transition Out Time**

0.0

To create a more dramatic effect, transitions between cameras are instantaneous.

The Mutator Zone has the **Enable VFX** setting disabled to maintain immersion.

The Trigger device uses the following modified settings:

 Option Value Description
**Visible In Game**

False

Players should not know they are walking on a trigger.

**Trigger VFX**

False

Players should not know they are walking on a trigger.

**Trigger SFX**

False

Players should not know they are walking on a trigger.

**Direct Event Binding**

The cameras are linked to devices in the following way:

 Device Function Device Event
**Fixed Point Camera**

Add to Player

Mutator Zone

On Player Entering Zone

**Fixed Point Camera**

Remove from Player

Mutator Zone

On Player Exiting Zone

**Fixed Point Camera**

Add to Player

Trigger

On Triggered

#### Advantages of Fixed Point Cameras

Fixed point cameras offer a wide variety of advantages:

-
**Cinematic Presentation**: Create cinematic moments by presenting scenes from carefully chosen angles, which enhances storytelling and immersion.

-
**Controlled Viewpoints**: Designers can control what the player sees, ensuring that key elements or surprises are revealed at specific times.

-
**Artistic Direction**: Fixed cameras can showcase the game's art style, architecture, or specific details in the environment.

-
**Gameplay Challenges**: Challenge players by restricting their view, adding difficulty, or creating puzzles that rely on obscured information.

#### Limitations of Fixed Point Cameras

If you're not careful, fixed point cameras can negatively impact player experience. Keep these points in mind when making your game.

-
**Limited Player Control**: Players might feel restricted or disoriented if they can't control the camera freely, affecting their overall experience.

-
**Potential for Frustration**: In certain situations, fixed cameras might hinder gameplay, leading to frustration when they obscure important information or impede progress.

As island creators and game designers, you must balance the benefits and drawbacks of fixed point cameras to ensure they enhance the gaming experience without causing unnecessary hindrances to the player.

### Fixed Angle Cameras

Fixed angle cameras move with the player, remaining in a locked angle and giving them a consistent perspective. They can offer various viewpoints, such as top-down, side-scrolling, or isometric angles, giving players a consistent visual reference as they navigate through the game. They're commonly used in many classic games.

#### Using a Fixed Angle Camera for a Zombie Survival Game

This example uses a Fixed Angle Camera device to emulate the feeling of a classic top-down shooter. Here, players must eliminate hordes of zombies in order to level up and obtain better weapons.

You can see that there are [transitions](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#camera-transition) between two fixed angle cameras. The first is enabled when the player must purchase weapons, and transitions to the second camera when the player leaves the shop to fight the hordes of zombies.

The first **Fixed Angle Camera** device in this example uses the following modified settings:

 Option Value Description
**Add to Players on Start**

False

This camera is not added to players at the start of the game.

**Transition in Priority**

10

Camera transition is determined by the highest priority, comparing the Out Priority of the current camera to the In Priority of the destination camera.

**Transition in Type**

Linear

Behavior of the camera when activating.

**Transition in Time**

0

This is an immediate transition.

**Transition Out Type**

Linear

Determines the style of transition.

**Transition Out Time**

0

This is an immediate transition.

The second **Fixed Angle Camera** device in this example uses the following modified settings:

 Option Value Description
**Transition in Type**

Linear

Behavior of the camera when activating.

**Transition in Time**

0

This is an immediate transition.

**Transition Out Priority**

2

Camera transition is determined by the highest priority, comparing the Out Priority of the current camera to the In Priority of the destination camera.

**Transition Out Type**

Linear

Determines the style of transition.

**Transition Out Time**

0

This is an immediate transition.

**Collision Type**

Transparency

Makes objects that obscure the target invisible when line of sight is broken.

The **Third Person Controls** device in this example uses the following modified settings:

**אפשרויות, ערכים ותיאורים:**

##### Interact Distance

- **Value / Values:** 50
- **Description:** Distance from player required to perform an interaction.

##### Rotation Rate

- **Value / Values:** 600
- **Description:** The player’s turning rate, in degrees per second.

##### Shooting Locomotion Movement Speed

- **Value / Values:** 400
- **Description:** Movement speed while shooting, in meters per second.

##### Shooting Locomotion Rotation Rate

- **Value / Values:** 600
- **Description:** The player’s turning rate while shooting, in degrees per second.

##### Aiming Locomotion Movement Speed

- **Value / Values:** 400
- **Description:** Movement speed while aiming, in meters per second.

##### Aiming Rotation Rate

- **Value / Values:** 600
- **Description:** The player’s turning rate while aiming, in degrees per second.

##### Scale Weight by Angle

- **Value / Values:** 0.7
- **Description:** This setting affects the prioritization of targets. As targets get closer to you, aiming at it becomes prioritized.

##### Ranged Targeting Angle

- **Value / Values:** 180
- **Description:** Depending on where the player is facing, the range in degrees where targets are considered valid.

##### Aim Targeting Angle

- **Value / Values:** 180
- **Description:** Depending on where the player is facing, the range in degrees where targets are considered valid.

#### Advantages of Fixed-Angle Cameras

-
**Artistic Presentation**: Allows for meticulously crafted views, showcasing the game's visual elements and artistic design from specific angles.

-
**Controlled Narrative**: Designers can guide players' attention to key story elements or scenic views by positioning the camera strategically.

-
**Consistency**: Offers a stable perspective, providing players with a familiar and reliable viewpoint as they progress through the game.

-
**Optimized Design**: Simplifies level design and game mechanics because developers can anticipate what the player can see from a fixed angle, aiding themn in creating focused experiences.

#### Limitations of Fixed-Angle Cameras

-
**Limited Exploration**: Players might feel constrained or miss out on certain details as they cannot freely adjust the camera to explore the environment.

-
**Obstructed Views**: Fixed angles can sometimes hide crucial information or obstruct the player's view, leading to frustration or confusion.

Staying true to your vision should be the priority, so try not to sacrifice gameplay at the cost of using a better-looking camera!

### Orbit Cameras

Using an [orbit camera](https://dev.epicgames.com/documentation/fortnite/using-orbit-camera-devices-in-fortnite-creative) is like being the director of your own action movie. You can rotate it around a central point or your character, and view the environment from different perspectives. This type of camera is commonly used in open-world games and 3D platformers to give players a greater sense control over their view of the virtual world and enhance immersion.

Check out the [Orbit Camera Device Design Example](https://dev.epicgames.com/documentation/fortnite/orbit-camera-device-design-example-in-fortnite-creative) page to learn about a fun way to use the orbit camera in your projects!

### First Person Mode Cameras

Use the Gameplay Mode: First Person Mode device to put players in a first-person perspective.

You can use this device to create unique First Person Shooters that fully immerse players into your gameplay experience.

#### Limitations of First Person Mode Cameras

Below are the limitation of using the First Person Mode device.

-
Most ranged weapons, except Akimbo and Ballistic Shield are available, but not all available weapons have custom reload animations.

-
Some player actions are not available in first-person view. Players performing some actions (such as swimming, gliding and skydiving) will automatically switch to the default Third Person Camera. Additionally, there are some other player actions that might cause the player's hands or weapon to be hidden.

-
Shadows are missing when using the first-person view, and in certain situations there might be some clipping or other rendering issues.

-
Melee weapons and vehicles are not supported in the current version of the device.

### Priority System

For the Camera devices, **Priority** determines which device takes priority when multiple devices are active.

When placing a device, the default priority is **0**, which is the lowest priority assignment. Any device with a higher Priority number (1 and above) will override devices with a lower priority.

#### Visualizing Priorities

In this example, three Fixed Angle cameras are connected to ON/OFF switches. The first camera is set to **Priority 0**, and the two cameras to the right are both set to **Priority 1**.

The player always sees the highest priority active camera. When cameras are the same priority, the camera that is most recently added is what the player sees.

Reactivating the Priority 0 camera will not work until both Priority 1 cameras have been turned off. A lower priority camera can never override a high priority camera.

#### How to Use Priorities

The priority system can really simplify your workflow when used correctly!

Instead of working out complicated trigger logic, you can automatically add higher priority cameras to players as they enter a building, then remove them when they go back outside.

Try coming up with your own scenarios!

### Adapting Controls

Simply putting down a camera device in your level will result in your player character always facing the same direction as the camera. The Third Person Control device attempts to capture player intent, allowing your character to face a target or your movement direction.

Depending on the type of game you’re looking to make, you may need to calibrate the targeting logic to achieve the desired player experience.

On the left side, the device's settings are left on default. Zombies are not targeted until they are very close and the player needs to make adjustments often to get them into the weapon’s sights.

On the right side, the automatic targeting was significantly increased, so much so that the player only needs to press the Fire button to eliminate every zombie that appears on the screen!

Here are the modified settings for the example on the right:

-
Rotation Rate: 800

-
Rotate Toward Target: True

-
Shooting Locomotion Rotation Rate: 800

-
Aiming Rotation Rate: 800

-
Scale Weight by Angle: 1.0

-
Ranged Targeting Angle: 180

-
Aim Targeting Angle: 180

The best way to determine what feels right for your island is to playtest often, alone and with other players.

### Boundaries and Deadzones

The [deadzone](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#deadzone) refers to an established area within which the player character can move around without affecting the camera. When the player moves to an edge of the deadzone, the camera will move to follow the target.

In the example below, notice how the camera is static as the player runs inside the deadzone, and starts to move again when the player exits the deadzone.

Deadzones help you manage what players can see or do in certain areas.

You can use deadzones for artistic purposes as well! By limiting the camera's movement within predefined zones, create picturesque views or cinematic compositions, and spruce up the game's visual storytelling.

**Boundaries** are pre-defined points beyond which the camera will not move.

Notice in the example below how the camera follows the player within the volume, but stops once the player exits the volume. This movement is defined by the camera’s boundaries.

For sidescroller games, boundaries are often placed at the edges of the screen. When the player reaches these zones, the camera doesn't move further until the player advances. Once a player moves beyond a certain point, the camera's boundary might restrict them from returning, focusing on the forward movement through the level design.

### Using UEFN to Level Up Your Design

While camera and controls devices are fully available to use in Fortnite Creative, you can take your design work to the next level using Unreal Editor for Fortnite (UEFN).

To learn about using cameras in UEFN, see:

-
[Gameplay Camera and Control Devices](https://dev.epicgames.com/documentation/en-us/uefn/gameplay-camera-and-control-devices-in-unreal-editor-for-fortnite)

-
[Making a Title Sequence](https://dev.epicgames.com/documentation/en-us/uefn/making-a-title-sequence-in-unreal-editor-for-fortnite) gameplay example

---

## Using Class Designer Devices in Fortnite Creative

**כותרת מקורית:** Using Class Designer Devices in Fortnite Creative  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/using-class-designer-devices-in-fortnite-creative  
**מקור קלט:** `07C_שחקנים_קבוצות_תפקידים_ומצלמות(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `using-class-designer-devices-in-fortnite-creative`

**
The **Class Designer** device is used in conjunction with the [Class Selector](https://dev.epicgames.com/documentation/fortnite/using-class-selector-devices-in-fortnite-creative) device to make it easy to create [class-based gameplay](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary).

The Class Designer gives you a way to define a custom [class](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) with an initial set of [attributes](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) and an inventory [loadout](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary).

Each device is used to design one custom class. To define the inventory loadout for this class, drop [items](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) onto the device to [register](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) them for that class.

The Class Identifier is used by:

-
The **[Class Selector](https://dev.epicgames.com/documentation/fortnite/class-selector)** device

-
The Team Settings & Inventory device

-
**Island** Settings**

There is a hierarchy of setting overrides, described as follows:

-
Island Settings are the baseline.

-
Team Settings & Inventory overrides Island Settings if there is a specific value set in the device.

-
Class Designer overrides both Team Settings & Inventory and Island Settings, if there is a specific value set in the device that differs from the Island Settings or Team Settings & Inventory values.

See the pages under Island Settings for more info.

For information on finding the Class Designer device, see [Using Devices](https://dev.epicgames.com/documentation/fortnite/using-devices-in-fortnite).

If you're using multiple copies of a device on an island, it can be helpful to [rename](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) them. You can choose names that relate to each device's purpose, so it's easier to remember what each one does.

### Device Options

A player cannot interact with this device in [Play mode](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) even if it is visible.
This device has some basic functionality, like setting the maximum health and shields for the class, and whether items are granted to the player when they respawn. Additionally, there are some advanced options, such as turning on player movement features like Sprinting and Sliding.

#### Contextual Filtering

Some devices are affected by a feature called **contextual filtering**. This feature hides or displays options depending on the values selected for certain related options. This reduces clutter in the Customize panel and makes options easier to manage and navigate. To help identify them, values that trigger contextual filtering are in *italic*.

All options are listed, including those affected by contextual filtering; if they are hidden or displayed based on a specific option's value, there will be a note about it in the Description field for that option.
**

Default values are **bold**. Values that trigger contextual filtering are *italic*.

You can configure this device with the following options.

**אפשרויות, ערכים ותיאורים:**

##### Class Identifier

- **Value / Values:** **Class Not Selected**, Pick a number
- **Description:** This is used by the Class Selector to identify which Class the player will switch to. If multiple Class Designers use the same identifier, the one that was placed first will be used.

##### Class Name

- **Value / Values:** Enter text
- **Description:** Enter a name for your custom class. The text field is limited to 24 characters.

##### Class Description

- **Value / Values:** Enter text
- **Description:** Enter a description of up to 512 characters.

##### Grant Items On Respawn

- **Value / Values:** Yes, **No**
- **Description:** Determines whether the device grants the listed items to players when they [respawn](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary).

##### Equip Granted Item

- **Value / Values:** **Don't Equip**, Pick an item
- **Description:** If the device grants items to the player, this determines whether the item listed in order should be equipped or not. Specifying an item order higher than the number of items in the list results in the last item being granted.

##### Visible During Game

- **Value / Values:** Yes, **No**
- **Description:** Determines whether the device is visible during the game.

##### Initial Weapon Ammo

- **Value / Values:** **Don't Override**, select a number from 1 to 999
- **Description:** Sets the amount of ammunition loaded in the weapon when granted, limited by the weapon's magazine size.

##### Spare Weapon Ammo

- **Value / Values:** **Default**, select a number from 1 to 999
- **Description:** Sets how much spare ammunition is added to the player's inventory when a weapon is granted. **Default** provides ammo based on the ammo type used by the weapon.

##### Start With Pickaxe

- **Value / Values:** **Don't Override**, No, Yes
- **Description:** Determines whether players start the game with a pickaxe.

##### Invincibility

- **Value / Values:** **Don’t Override**, On, Off
- **Description:** Determines if players should spawn with invincibility.

##### Max Health

- **Value / Values:** **Don't Override**, Pick an amount
- **Description:** Determines the maximum health players can attain. This takes precedence over a Team Settings & Inventory device.

##### Allow Health Recharge

- **Value / Values:** **Off**, On
- **Description:** When set to **On**, players can regenerate health over time.

##### Health Recharge Delay

- **Value / Values:** **6.5 Seconds**, Pick a time
- **Description:** Determines how long after taking damage before a player's health starts to recharge.

##### Health Recharge Amount

- **Value / Values:** **1**,Pick a number
- **Description:** Sets how much health per second is recharged after **Health Recharge Delay** completes.

##### Starting Shield Percentage

- **Value / Values:** **Don't Override**, No Shields, 50% Shields, 100% Shields
- **Description:** Determines how many shields the player has when they spawn, as a percentage of their **Max Shields**. This takes precedence over a **Team Settings & Inventory** device.

##### Max Shields

- **Value / Values:** **Don't Override**, No Shields, Pick an amount
- **Description:** Determines the maximum shield capacity this class can attain. This takes precedence over a Team Settings & Inventory device.

##### Allow Shield Recharge

- **Value / Values:** **Off**, On
- **Description:** When set to **On**, allows player shields to recharge over time.

##### Shield Recharge Delay

- **Value / Values:** **6.5 Seconds**, Pick a time
- **Description:** Determines how long after taking damage before a player's shield starts to recharge.

##### Shield Recharge Amount

- **Value / Values:** **1**,Pick a number
- **Description:** Sets how much health per second is recharged after **Shield Recharge Delay** completes.

##### Allow Overshield

- **Value / Values:** **Don't Override**, Off, On
- **Description:** Determines whether the Overshield feature is available.

##### Overshield Max

- **Value / Values:** **Don't Override**, Pick an amount
- **Description:** *This only displays if you have set the **Overshield: More Options** option to **Show**.* Determines the maximum amount of Overshield a player can have. If you set an amount here, it will override any amount set in the My Island > Settings tab.

##### Overshield Recharge Delay

- **Value / Values:** **Don't Override**, Pick an amount of seconds
- **Description:** *This only displays if you have set the **Overshield: More Options** option to **Show***. The Overshield starts to recharge after this amount of time if the player takes no damage during the delay. If you set the delay here, it will override the delay set in Island Settings.

##### Overshield Recharge Rate

- **Value / Values:** **Don't Override**, Pick an amount
- **Description:** *This only displays if you have set the **Overshield: More Options** option to **Show***. Determines how much the Overshield recharges each second, after the recharge delay has ended. If you set the recharge amount here, it will override the recharge amount in Island Settings.

##### Overshield Recharge Period

- **Value / Values:** 1.0**, Select an amount
- **Description:** Determines the tick period for recharging the Overshield.

##### Movement Multiplier

- **Value / Values:** **Don't Override**, Pick a multiplier
- **Description:** Determines how fast the player moves as a multiplication of the base move speed. This takes precedence over a Team Settings & Inventory device.

##### Allow Sprinting

- **Value / Values:** **Don't Override**, Off, On
- **Description:** Determines whether the Sprinting feature is available.

##### Sprinting Energy Cost Per Second

- **Value / Values:** **Don't Override**, Pick an amount
- **Description:** This only displays if you have set the **Sprinting: More Options** option to **Show**. Determines how fast sprinting Energy is drained each second while a player is sprinting. If you set the energy cost here, it will override the energy cost set in the My Island > Settings tab.

##### Sprinting Jump Multiplier

- **Value / Values:** **Don't Override**, Pick or enter a multiplier
- **Description:** This only displays if you have set the **Sprinting: More Options** option to **Show**. Determines how much higher or farther players jump when sprinting, as a multiple of normal jump height or length. Use the arrows to select a multiplier. If you set the jump multiplier here, it will override the jump multiplier set in the My Island > Settings tab.

##### Sprinting Speed Multiplier

- **Value / Values:** **Don't Override**, Pick a multiplier
- **Description:** This only displays if you have set the **Sprinting: More Options** option to **Show**. Determines how fast a player moves when Sprinting, as a multiple of their speed when not Sprinting. If you set the sprint speed here, it will override the sprint speed set in the My Island > Settings tab.

##### Energy Max

- **Value / Values:** **Don't Override**, Pick an amount
- **Description:** Determines how much Energy is available to the player. This affects Sprinting, as well as other abilities that use Energy.

##### Energy Recharge Amount

- **Value / Values:** **Don't Override**, Pick an amount
- **Description:** When Energy begins to recharge, this determines the amount of Energy recharged each second.

##### Energy Recharge Delay

- **Value / Values:** **Don't Override**, Pick a time
- **Description:** After a player stops using Energy, this sets the length of delay before the player's Energy begins to recharge.

##### Allow Sliding

- **Value / Values:** **Don't Override**, Off, On
- **Description:** Determines whether the Sliding feature is available.

##### Allow Slide Kick

- **Value / Values:** **Don't Override**, Off, On
- **Description:** Determines whether sliding players can use the Slide Kick to impact and knock away players on an opposing team.

##### Allow Shoulder Bashing

- **Value / Values:** **Don't Override**, Off, On
- **Description:** Determines whether the Shoulder Bashing feature is available.

##### Instant Reload

- **Value / Values:** **Don't Override**, On, Off
- **Description:** Determines whether weapons are reloaded instantaneously, or reloaded based on the time defined in each weapon. This takes precedence over a Team Settings & Inventory device.

##### Infinite Reserve Ammo

- **Value / Values:** **Don't Override**, On, Off
- **Description:** Determines whether players have infinite reserve ammo or not. This takes precedence over a Team Settings & Inventory device.

##### Infinite Items

- **Value / Values:** **Don't Override**, On, Off
- **Description:** Determines whether players have infinite items (grenades, health items, traps, etc.) during the game.

##### Infinite Building Materials

- **Value / Values:** **Don't Override**, On, Off
- **Description:** Determines whether players have infinite building materials. This takes precedence over a Team Settings & Inventory device.

##### Eliminated Player's Items

- **Value / Values:** **Don't Override**, Drop, Keep, Delete
- **Description:** Determines what happens to the player's items when the player is eliminated. This takes precedence over a Team Settings & Inventory device. Options are:

#### -
**Drop**: The player's items are dropped on the ground, and other players can pick them up.

- **Value / Values:** -
**Keep**: The player's items are retained.
- **Description:** -
**Delete**: The player's items are removed from the game.

##### Eliminated Player's Resources

- **Value / Values:** **Don't Override**, Drop, Keep, Delete
- **Description:** Determines what happens to the player's resources (wood, metal, stone, gold) when they are eliminated. This takes precedence over a Team Settings & Inventory device. Options are:

#### -
**Drop**: The player's items are dropped on the ground. Other players can pick them up.

- **Value / Values:** -
**Keep**: The player's items are retained.
- **Description:** -
**Delete**: The player's items are removed from the game.

##### Eliminated Player's Game Resources

- **Value / Values:** **Don't Override**, Drop, Keep, Delete
- **Description:** Determines what happens to the player's resources (wood, metal, stone, gold) when they are eliminated. This takes precedence over a Team Settings & Inventory device. Options are:

#### -
**Drop**: The player's items are dropped on the ground. Other players can pick them up.

- **Value / Values:** -
**Keep**: The player's items are retained.
- **Description:** -
**Delete**: The player's items are removed from the game.

##### Fall Damage

- **Value / Values:** **Don't Override**, On, Off
- **Description:** Determines whether players are affected by fall damage. This takes precedence over a Team Settings & Inventory device.

##### Gravity

- **Value / Values:** **Don't Override**, Very Low, Low, Normal, High, Very High
- **Description:** Determines the amount of gravity that affects players during the game.

##### Jump Fatigue

- **Value / Values:** **Don't Override**, On, Off
- **Description:** Determines whether continuous jumping applies a penalty to jump height. This takes precedence over a Team Settings & Inventory device.

##### Allow Mantling

- **Value / Values:** **Don't Override**, On, Off
- **Description:** Determines whether the Mantling feature is available.

##### Mantling Minimum Height

- **Value / Values:** **Don't Override**, Very Low, Low, Normal, High
- **Description:** This only displays if you have set the **Show More Options: Mantling** option to **Show**. Determines the lowest height at which a player can use mantling on a ledge. You might want to adjust this value if gravity or other factors affect mantling.

##### Mantling Minimum Height In Water

- **Value / Values:** **Don't Override**, Very Low, Low, Normal, High
- **Description:** This only displays if you have set the **Show More Options: Mantling** option to **Show**. Determines the lowest height at which a player can mantle from the water. You might want to adjust this value if gravity or other factors affect mantling.

##### Allow Hurdling

- **Value / Values:** **Don't Override**, On, Off
- **Description:** Determines if hurdling is available to players. If you choose **On**, players will hurdle over obstacles automatically if they are sprinting toward the obstacle.

##### Player Flight

- **Value / Values:** **Don't Override**, On, Off
- **Description:** Determine whether players can fly. This takes precedence over a Team Settings & Inventory device.

##### Always Show Name Plates

- **Value / Values:** **Don't Override**, Always Show to Team, Always Show to All, Always Hide, No
- **Description:** Determines whether players names and locations can be seen by other players.

##### Limit Name Plate Max Distance

- **Value / Values:** **Dont' Override**, Select a distance
- **Description:** If set to a number, name plates will disappear if that player is further away than that distance from the camera.

##### Name Plate Line of Sight

- **Value / Values:** **Don't Override**, Always Show, Hide Behind Objects
- **Description:** If set, the name plates will hide whenever a player is obstructed by an obstacle.

##### Focus Angle

- **Value / Values:** **Don't Override**, Pick an angle
- **Description:** When a player is focusing, this determines the maximum angle another player can be from the focusing player's look direction in order to be a valid focus target.

##### Focus Time

- **Value / Values:** **Don't Override**, Pick a number
- **Description:** Determines the amount of time a player must focus on another player to see that player's name plate.

##### Show Voice Indicator

- **Value / Values:** **Don't Override**, Don't Override Show Name Plates, Always Show to Team, Always Show to Hostiles, Always Show to All, Disable
- **Description:** Determines whether the voice indicator can be seen on a player's name plate. Can be used to control the voice indicator and name plate separately.

##### Show Player Health Indicator

- **Value / Values:** **Don't Override**, Team Only, Enemies, Anyone, Never
- **Description:** Determines who can see the health indicator over the player's head. This takes precedence over a Team Settings & Inventory device. Options are:

#### -
**Team Only**: Only team members can see the player's health indicator.

- **Value / Values:** -
**Enemies**: Only enemies can see the player's health indicator.
- **Description:** -
**Anyone**: All players can see the player's health indicator.

#### -
**Never**: No one can see the player's health indicator.

- **Value / Values:** **Display Health for All Players**
- **Description:** **Don't Override**, Yes, No

##### Determines if this player can see the health bar display on the HUD for all players.

- **Value / Values:** This is actually a separate UI element from **Show Player Health Indicator**, and is often used for [boss fight](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) scenarios.
- **Description:** **Glider Redeploy**

##### **Don't Override**, On, Off

- **Value / Values:** Determines whether the player can freely deploy gliders without using an item. This takes precedence over a Team Settings & Inventory device.
- **Description:** **Down But Not Out**

##### **Don't Override**, Default, Classic, Improved, Off

- **Value / Values:** Determines the type of Down But Not Out state this class allows. This takes precedence over a Team Settings & Inventory device. Options are:
- **Description:** -
**Don't Override**: The settings for Down But Not Out are not affected by this device.

#### -
**Default**: The Down But Not Out state is set automatically based on team size.

- **Value / Values:** -
**Classic**: Enables the Down But Not State for this class.
- **Description:** -
**Improved**: Enables the Down But Not State for this class, and adds more interactions during the state like opening doors and dropping inventory items.

#### -
**Off**: Down But Not Out is disabled for this class.

- **Value / Values:** **Drop Reboot Card on Elimination**
- **Description:** **Don't Override**, If Can Be Rebooted, No

##### Determines if players drop a Reboot Card when eliminated. Reboot cards are only dropped if a remaining teammate is eligible to use a Reboot Van.

- **Value / Values:** **Allow Building**
- **Description:** **Don't Override**, None, All, Traps Only, No Traps

##### Determines whether players can build and place traps. This takes precedence over a Team Settings & Inventory device. Options are:

- **Value / Values:** -
**None**: The player can neither build nor place traps.
- **Description:** -
**All**: The player can build or place traps, if they have the required resources.

#### -
**Traps Only**: The player cannot build, but can place traps.

- **Value / Values:** -
**No Traps**: The player can build, but not place traps.
- **Description:** **Respawn Time**

##### **Don't Override**, Pick or enter an amount of seconds

- **Value / Values:** Determines how long the player must wait after being eliminated before they are respawned. Use the arrows to select a number. This takes precedence over a Team Settings & Inventory device.
- **Description:** **Spawn Limit**

##### **Don't Override**, Infinite, Pick a number

- **Value / Values:** Determine the number of times the player can spawn into the game (also known as Number of Lives). This includes the initial spawn. So setting it to 1 means the player will not be able to respawn when eliminated. This takes precedence over a Team Settings & Inventory device.
- **Description:** **Spawn Location**

##### **Don't Override**, Spawn Pads, Sky, Current Location, Do Not Spawn

- **Value / Values:** Determines where the player will spawn when the game starts. This takes precedence over a Team Settings & Inventory device. Options are:
- **Description:** -
**Spawn Pads**: Where the Player Spawner device is placed.

#### -
**Sky**: Up in the air where the player will parachute down.

- **Value / Values:** -
**Current Location**: Where they are currently located.
- **Description:** -
**Do Not Spawn**: Player will not be spawned unless triggered by event binding.

##### Health Granted on Elimination

- **Value / Values:** **Don't Override**, Pick an amount
- **Description:** How much health the player gets when they eliminate another player. When the amount awarded will cause their current health to exceed their max health, the excess amount will be awarded as shields. This takes precedence over a Team Settings & Inventory device.

##### Wood Granted on Elimination

- **Value / Values:** **Don't Override**, Pick an amount
- **Description:** How much wood the player gets when they eliminate another player. This takes precedence over a Team Settings & Inventory device.

##### Stone Granted on Elimination

- **Value / Values:** **Don't Override**, Pick an amount
- **Description:** How much stone the player gets when they eliminate another player. This takes precedence over a Team Settings & Inventory device.

##### Metal Granted on Elimination

- **Value / Values:** **Don't Override**, Pick an amount
- **Description:** How much metal the player gets when they eliminate another player. This takes precedence over a Team Settings & Inventory device.

##### Gold Granted on Elimination

- **Value / Values:** **Don't Override**, Pick an amount
- **Description:** How much gold the player gets when they eliminate another player. This takes precedence over a Team Settings & Inventory device.

##### Maximum Building Resources

- **Value / Values:** **Don't Override**, Pick an amount
- **Description:** Sets the maximum amount of resources a player can carry. This takes precedence over a Team Settings & Inventory device.

##### Allow Item Drop

- **Value / Values:** **Don't Override**, Yes, No
- **Description:** Determines whether players can drop items from their inventory during the game. This takes precedence over a Team Settings & Inventory device.

##### Allow Item Pick Up

- **Value / Values:** **Don't Override**, Yes, No
- **Description:** Determines whether players can pick up items during the game. This takes precedence over a Team Settings & Inventory device.

##### Harvest Multiplier

- **Value / Values:** **Don't Override**, Pick a multiplier
- **Description:** Determines the rate at which players can harvest resources. This takes precedence over a Team Settings & Inventory device.

##### Override Spawn Immunity Time

- **Value / Values:** **Don’t Override**, Yes, No
- **Description:** Determines if the invulnerability time granted to a player on respawn should be overridden.

##### Visible In UI

- **Value / Values:** **On**, Off
- **Description:** If there is a Class Selector UI device active, this option determines whether this class is shown in the Class Selector UI list of available classes.

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

##### Show in UI When Receiving From

Enables this class in the Class Selector UI when an event occurs.

##### Hide in UI When Receiving From

Disables this class in the Class Selector UI when an event occurs.

#### Events

There are no events for this device.

### Gameplay Examples

-
[Class Setup In A Hole](https://dev.epicgames.com/documentation/fortnite/class-setup-in-an-arena-gameplay-example-in-fortnite-creative)

-
[Top Scorer In Class](https://dev.epicgames.com/documentation/fortnite/top-scorer-in-class-in-fortnite-creative)

-
[Dungeon Crawler](https://dev.epicgames.com/documentation/fortnite/dungeon-crawler-gameplay-example-in-fortnite-creative)

---

## Using Class Selector Devices in Fortnite Creative

**כותרת מקורית:** Using Class Selector Devices in Fortnite Creative  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/using-class-selector-devices-in-fortnite-creative  
**מקור קלט:** `07C_שחקנים_קבוצות_תפקידים_ומצלמות(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `using-class-selector-devices-in-fortnite-creative`

The **Class Selector** device is used in conjunction with the [Class Designer](https://dev.epicgames.com/documentation/fortnite/using-class-designer-devices-in-fortnite-creative) device for creating [class-based gameplay](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary). Once you've set up your custom [classes](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) with the Class Designer, you can use the Class Selector to set how they'll be used [in-game](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary).

You need one Class Selector for each custom class you use. When in [Play mode](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary), a player can select or switch to a specific class by walking over the device's colored activation zone.

You can also use the Class Selector to set up team selection independently from class selection, but be aware that team switching will force the player to [respawn](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary).

To find the Class Selector device, see [Using Devices](https://dev.epicgames.com/documentation/en-us/fortnite-creative/using-devices-in-fortnite-creative).

If you're using multiple copies of a device on an island, it can be helpful to [rename](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) them. You can choose names that relate to each device's purpose, so it's easier to remember what each one does.

### Contextual Filtering

Some devices are affected by a feature called contextual filtering. This feature hides or displays options depending on the values selected for certain related options. This feature will reduce clutter in the Customize panel and make options easier to manage and navigate.

However, it may not be easy to recognize which options or values trigger contextual filtering. To help you identify them, in our device docs we use *italic* for any values that trigger contextual filtering. All options will be listed, including those affected by contextual filtering; if they are hidden or displayed based on a specific option's value, there will be a note about that in the **Description** field for that option.

### Device Options

Before you start to customize a Class Selector, make sure you've placed and customized your Class Designer devices, each with it's own **Class Identifier**. You will use this identifier with the **Class to Switch to** option in the Class Selector.

Keep in mind the following:

-
You have to specify a **class number** for this to work.

-
That number must be defined in a Class Designer device.

-
If the number is not defined in a Class Designer, the player will be assigned default attributes with no weapons. The device **will not** fall back to the Default Class Identifier assigned in a Team Settings & Inventory device, or in [Island Settings > Mode](https://dev.epicgames.com/documentation/fortnite/mode-settings-in-fortnite-creative).

Default values are **bold**. Values that trigger contextual filtering are *italic*.

You can configure this device with the following options.

**אפשרויות, ערכים ותיאורים:**

##### Class to Switch To

- **Value / Values:** **Don't Override**, No Class, Pick a class number
- **Description:** Indicates which class the player will switch to, as defined by the **Class Identifier** in the **Class Designer**. If you choose **No Class**, the player will not switch their class. This is mostly used for team switching.

##### Send Game Start Class Changes at Warmup

- **Value / Values:** **Off**, On
- **Description:** Determines whether the device sends any **Class Changed** events that are triggered at the start of the game during warmup instead of when the countdown is finished.

##### Team To Switch To

- **Value / Values:** **Don't Override**, Random, Pick or enter a team number
- **Description:** With **Do Not Switch**, no team switching happens when a player changes their class. If you choose **Random**, the player switches to a random team that is not their current team.

##### Send Game Start Team Changes at Warmup

- **Value / Values:** **Off**, On
- **Description:** Determines whether the device sends any **Team Changed** events that are triggered at the start of the game during warmup instead of when the countdown is finished.

##### Activating Team

- **Value / Values:** **Any**, Pick or enter a team number
- **Description:** Only players in a specific team can use this device. If you choose **Any**, all teams can use this device.

##### Time to Switch

- **Value / Values:** **Instant**, Pick or enter a time
- **Description:** The time it takes for the player to switch their class after they walk over the activation zone. This is irrelevant to Team Switching since the player is forced to respawn when they switch teams.

##### Respawn Player On Switch

- **Value / Values:** On, **Off**
- **Description:** Determines whether a player will respawn when switching classes.

##### Restore Health and Shields on Switch

- **Value / Values:** **On**, Off
- **Description:** Determines whether the player's health and shields are restored to their starting amount when they switch classes.

##### Clear Items On Switch

- **Value / Values:** **Never**, Team, Class, Always
- **Description:** Determines whether items are removed from the player's inventory when they switch classes. [INCLUDE:#clearitems]

##### Size of Volume

- **Value / Values:** **1 Meter**, Pick a size
- **Description:** The size of the activation volume in meters.

##### Volume Visible In Game

- **Value / Values:** **On**, Off
- **Description:** Determines whether the activation volume is visible during the game. This does not affect the collision properties of the device.

##### Visible During Game

- **Value / Values:** **On**, Off
- **Description:** Determines whether the device is visible to the player. This also affects [collision](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) when the player interacts with the device. When **On**, the device has collision. When **Off**, the device has no collision.

##### Accent Color Type

- **Value / Values:** ***Direct Color***, Team Color, Team Relationship
- **Description:** Determines whether the device uses a custom color, or the team or team relationship color. If you set this to **Direct Color**, the **Accent Color** option displays below this one.

##### Accent Color

- **Value / Values:** **Aqua**, Pick a color swatch
- **Description:** Determines the color used by the device. Click the swatch to open the Color Picker. Select a color, then click the checkmark to close the Color Picker.

##### Enabled During Phase

- **Value / Values:** None, Always, Pre-Game Only, **Gameplay Only**
- **Description:** Sets the [game phase](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) in which the device is enabled. If you choose **Pre-Game Only**, the device is only enabled before the game begins. (Pre-game includes [lobby](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) and countdowns.) If you choose **Gameplay Only**, the device is only enabled during the game.

##### Activation Audio

- **Value / Values:** **On**, Off
- **Description:** This option only displays if the **Accent Color Type** option is set to **Direct Color**. Determines whether the Class Selector plays audio effects when activated.

##### Zone Audio

- **Value / Values:** **On**, Off
- **Description:** **Determines whether the Class Selector should play audio effects when players enter the zone.**

##### Display VFX Effect On Activation

- **Value / Values:** **On**, Off
- **Description:** Controls whether a [VFX](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) effect is created when a player changes class or team.

##### Throttle Class Changes

- **Value / Values:** On, **Off**
- **Description:** If this is set to **On**, when a player changes class the device will delay any subsequent class changes for 3 seconds in order to avoid potential performance impacts.

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

This function disables the class selector when an event occurs.

##### Change Player to Class When Receiving From

This function changes the player to the specified class when an event occurs.

##### Change Player to Team When Receiving From

This function changes player to the specified Team when an event occurs.

##### Change Player to Team and Class When Receiving From

This function changes the player to the specified team when an event occurss, even if player is within the team switch cooldown period.

##### Change Selector Team When Receiving From

When an event occurs, this function changes the **Team to Switch To** value to the team of the instigating player.

#### Events

Sends an event to a linked device when a player interacts with the button.
Direct event binding uses events as transmitters. An event tells another device to perform a function.

-
For any event option, click the **option**, then **Select Device** to access and select from the **Device** dropdown menu.

-
Once you've selected a device, click **Select Function** to bind the timer to a function for that device.

-
If more than one function is triggered by the event, click the **Add** button to add a line and repeat these steps.

**אפשרויות ותיאורים:**

##### On Class Switched Send Event To

When a player switches classes, an event is sent to the selected device, which triggers the selected function.

##### On Team Switched Send Event To

When a player switches teams, an event is sent to the selected device, which triggers the selected function.

### Gameplay Examples

-
[Class Setup In An Arena](https://dev.epicgames.com/documentation/fortnite/class-setup-in-an-arena-gameplay-example-in-fortnite-creative)

-
[Top Scorer In Class](https://dev.epicgames.com/documentation/fortnite/top-scorer-in-class-in-fortnite-creative)

-
[Dungeon Crawler](https://dev.epicgames.com/documentation/fortnite/dungeon-crawler-gameplay-example-in-fortnite-creative)

---

## Using Class Selector UI Devices in Fortnite Creative

**כותרת מקורית:** Using Class Selector UI Devices in Fortnite Creative  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/using-class-selector-ui-devices-in-fortnite-creative  
**מקור קלט:** `07C_שחקנים_קבוצות_תפקידים_ומצלמות(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `using-class-selector-ui-devices-in-fortnite-creative`

The **Class Selector UI** device can create both a **popup dialog** and a new **tab on the game Map screen** to display a list of [classes](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) players can choose from.

To find the **Class Selector UI** device, see **Using Devices**](using-devices-in-fortnite-creative).

You can use this class selection [UI](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) in many ways:

-
Have players choose a class when they spawn at the beginning of the game that they keep for the entire game.

-
Allow players to choose their class when the game starts, then let them change their class when they respawn.

-
Decide whether a class change happens with the popup dialog or on the Map screen tab, or both if they both are available.

Below are illustrations of the **Class Selector UI popup dialog**, and the **Class Selector UI tab** on the Map screen.

[
](https://dev.epicgames.com/community/api/documentation/image/939b4741-4345-4b1d-9187-3fe39a7eaf14?resizing_type=fit) Class Selector UI Popup Dialog

[
](https://dev.epicgames.com/community/api/documentation/image/bfe7184e-08c2-43d1-8068-73085721aeac?resizing_type=fit) Class Selector UI Map Screen

The list of classes can also provide more details about a class for the player, such as what weapon [loadout](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) or [resources](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) are [granted](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) to that class.

This device requires that you use the **Class Designer** device. The Class Designer, along with the **Team Settings & Inventory** device, can sometimes override [Island Settings](https://dev.epicgames.com/documentation/fortnite/understanding-island-settings-in-fortnite-creative). This could produce unexpected results if you are not aware of how the game prioritizes these settings. The hierarchy of setting or device option overrides is as follows:

-
[Island Settings > Mode](https://dev.epicgames.com/documentation/fortnite/mode-settings-in-fortnite-creative) are the baseline for an island.

-
Options in the Team Settings & Inventory device override Island Settings if there is a specific value set in the device.

-
The [Class Designer](https://dev.epicgames.com/documentation/fortnite/class-designer) device overrides both Team Settings & Inventory and Island Settings if there is a specific value set in the device that differs from the Island Settings or Team Settings & Inventory values.

-
Some options in the Class Selector UI device override Class Designer options.

You can only place one instance of this device on an island.

### Using the Class Selector UI

To use this device effectively, you need to use it with Class Designer devices (one Class Designer for each class you want to provide for players). First, place the Class Selector UI device, then place your Class Designer devices. Set up your Class Designers for each class you want to provide to players:

-
Add a class name and description (these are Class Designer options used by the Class Selector UI device).

-
Add a different class identifier for each class.

-
Add whatever items, weapons and resources you want to grant each class.

-
Make sure that each Class Designer has the **Visible in UI** option set to **Yes**.

There are also options in the Class Designer that you can use to enable or disable the class selection UI. For more information on the Class Designer device, see [Class Designer Devices](https://dev.epicgames.com/documentation/fortnite/using-class-designer-devices-in-fortnite-creative) in the Creative documentation.

### Contextual Filtering

Some devices are affected by a feature called **contextual filtering**. This feature hides or displays options depending on the values selected for certain related options. This feature will reduce clutter in the Customize panel and make options easier to manage and navigate. However, it may not be easy to recognize which options or values trigger contextual filtering.

To help you identify them, in our device reference documents we use *italic* for any values that trigger contextual filtering. All options will be listed, including those affected by contextual filtering; if they are hidden or displayed based on a specific option's value, there will be a note about that in the Description field for that option.

### Device Options

This device has some basic functionality, like enabling or disabling the device, and determining whether the Popup or Map screen UI displays. Additionally, there are some advanced options, like saving a player’s shield and health data.

Default values are **bold**. Values that trigger contextual filtering are *italic*.

You can configure this device with the following options.

 Option Value Description
**Enabled**

**On**, Off

Turns all functionality on or off, including whether the Pop-up UI appears and whether the UI appears in the Player Menu.

**Label**

*Custom Label*, **Classes**, Loadouts, Heroes, Adventurers, Warriors, Characters, Shopkeepers, Fisherfolk, Townsfolk, Monsters, Aliens, Soldiers, Zombies, Wizards, Survivors, Perks

A localized name used in the UI to describe what the classes are. This is used as the name of the new tab displayed in the Map screen and is used in the in-game UI. If you choose **Custom Label**, you can enter your own non-localized label; choosing **Custom Label** also displays two additional options.

**Custom Singular Label**

**Class**, Enter text

This option is only displayed if you choose **Custom Label** for the **Label** option. The singular form of your custom label that appears in the UI (for example, "Class" instead of "Classes"). The text field is limited to 24 characters. The customized label is not localized to other languages.

**Custom Plural Label**

**Classes**, Enter text

This option is only displayed if you choose **Custom Label** for the **Label** option. The plural form of your custom label that appears in the UI (for example, "Classes" instead of "Class"). The text field is limited to 24 characters. The customized label is not localized to other languages.

**Show Popup UI**

Manually Only, **Player Spawn**

Determines when the class selector popup dialog is automatically shown.

**Player Can Disable Popup UI**

**On**, Off

If this is set to **On**, players can click a button in the UI to disable the Popup class dialog from displaying when the player respawns. If the **Show in Map Key Menu** option is set to **Visible**, the player can still change their class from the Map screen.

**Popup Auto Select Timer**

**30 seconds**, Pick a time

By default, a 30-second timer is displayed when the class selector popup dialog opens. You can select or type in a different number of seconds for this timer. When the timer reaches zero, a class is automatically set for the player and the popup dialog closes. If this option is set to **0 seconds**, the timer is hidden.

**Show in Map Key Menu**

**Visible**, Hidden

Determines whether the new class selector tab appears in the Map screen.

**Change on Next Respawn**

Neither, **Map Key Menu**, Popup UI, Both

This setting determines whether the class change a player selects is made immediately, or if the change is made the next time the player respawns. Values for this option are:

-
**Neither**: Changes to class are made immediately.

-
**Map Key Menu**: If the player changes class using the tab in the Map Key Menu, the change is made when they next respawn.

-
**Popup UI**: If the player changes class using the popup dialog, the change is made when they next respawn.

-
**Both**: When the player changes class using either UI, the change is made when they next respawn.

**Show Close Button**

**Off**, On

Determines whether the **Close** button is displayed in the class selector popup dialog or the class selector UI in the Map screen.

**Always Grant Items on Respawn**

**On**, Off

Determines whether the device grants items to players automatically on respawn. This overrides item-related options in the Class Designer device.

**Show HUD Message Post Popup UI**

**Always**, Skip First Time, Never

This setting determines when the HUD message will show which class was selected. This is useful for timing events at the start of a match or round, in case there is overlap with other player messaging.

### Direct Event Binding

Following are the [direct event binding](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) options for this device.

#### Functions

A [function](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) listens for an event on a device then performs an action.

-
For any function, click the **option**, then **Select Device** to access and select from the **Device dropdown menu**.

-
Once you've selected a device, click **Select Event** to bind the device to an event that will trigger the function for the device.

-
If more than one device or event triggers a function, click the **Add** button to add a line and repeat these steps.

**אפשרויות ותיאורים:**

##### Disable When Received From

Disables UI pop-up messages when an event occurs.

##### Enable When Receiving From

Enables UI pop up messages when an event occurs.

##### Show Popup UI When Receiving From

Shows popup UI messages when an event occurs.

#### Events

Sends an event to a linked device when a player interacts with the button.
Direct event binding uses events as transmitters. An event tells another device to perform a function.

-
For any event option, click the **option**, then **Select Device** to access and select from the **Device dropdown menu**.

-
Once you've selected a device, click **Select Function** to bind the event to a function for that device.

-
If more than one function is triggered by the event, click the **Add** button to add a line and repeat these steps.

 Option Description
**On Class Selected Send Event To**

Sends an event to a linked device when a player selects a class.

**On Class Updated Send Event To**

Sends an event to a linked device when a player's class is changed using the Class Selector UI.

**On Popup UI Closed Send Event To**

Sends an event to a linked device when the popup UI closes.

**On Popup UI Opened Send Event To**

Sends an event to a linked device when the popup UI opens.

- [ ](https://dev.epicgames.com/community/search)

---

## Using Down But Not Out Devices in Fortnite Creative

**כותרת מקורית:** Using Down But Not Out Devices in Fortnite Creative  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/using-down-but-not-out-devices-in-fortnite-creative  
**מקור קלט:** `07C_שחקנים_קבוצות_תפקידים_ומצלמות(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `using-down-but-not-out-devices-in-fortnite-creative`

**
**Down But Not Out (DBNO)** is a player state where the player does not have full health, but is not yet out of the game. You can use the **Down But Not Out** device to customize the DBNO state to support your game design.

The DBNO state can include the following gameplay elements:

-
A state between **healthy** and **removed from game**.

-
A method for **reviving downed players**.

-
An ability for players to **grab, carry or throw downed players**.

-
A way for a downed player to be [shaken down](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary), with a variety of results.

To find the Down But Not Out** device, see [Using Devices](https://dev.epicgames.com/documentation/fortnite/using-devices-in-fortnite).

Want some ideas? See the [Down But Not Out Device Design Example](https://dev.epicgames.com/documentation/fortnite/down-but-not-out-device-design-examples-in-fortnite-creative) and [Item Remover Device Design Example](https://dev.epicgames.com/documentation/fortnite/item-remover-device-design-example-in-fortnite-creative) to jumpstart your imagination!

If you're using multiple copies of a device on an island, it can be helpful to [rename](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) them. You can choose names that relate to each device's purpose, so it's easier to remember what each one does.

### Contextual Filtering

Some devices are affected by a feature called **contextual filtering**. This feature hides or displays options depending on the values selected for certain related options. This reduces clutter in the Customize panel and makes options easier to manage and navigate. To help identify them, values that trigger contextual filtering are in *italic*.

All options are listed, including those affected by contextual filtering; if they are hidden or displayed based on a specific option's value, there will be a note about it in the Description field for that option.

### Device Options

This device has some basic functionality, like enabling or disabling the DBNO state, and the rate at which a player's [Tenacity](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) goes down. Additionally, there are some advanced options, like selecting which team or class is affected, and whether players can be shaken down during DBNO.

Default values are **bold**. Values that trigger contextual filtering are *italic*.

You can configure this device with the following options.

 Option Value Description
**Enabled During Phase**

**All**, None, Pre-Game Only, Gameplay Only

[Enables](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) the device during a specific phase. The [pre-game phase](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) includes all phases before the game starts.

**DBNO Enabled**

**Do Not Override**, Yes, No

Determines whether players can be put into the DBNO state.

Even if you enable DBNO in this device option, DBNO does not work unless you have your island set up to have teams.

**Tenacity Type**

**Default**, Max Health, *Custom*

Tenacity is the amount of health resource a player has when downed. **Default** uses the classic value of 100. **Max Health** uses the player's maximum health configuration. If you select **Custom**, you can set a tenacity value in the next option, **Tenacity Amount**.

**Tenacity Amount**

**100**, Pick a number

Sets the value used for a player's tenacity. This option only shows if you select **Custom** for **Tenacity Type**.

**Use Default Tenacity Depletion Rate**

**Yes**, *No*

Use the game default depletion rate or set up a custom one. The **Default** amount of Tenacity lost each second is 2. If you set it to **No**, the **Custom Tenacity Depletion Rate** will show.

**Custom Tenacity Depletion Rate**

**5**, Pick a number

The amount of tenacity lost per second. This is a option is only availble when the **Use Default Tenacity Depletion Rate** is set to **No**.

**Use Default Health After Revive**

**Yes**, *No*

Use the game default health after revive or set up a custom one. If you select **No**, you can set the **Health After Revive** percentage below.

**Health After Revive**

**100/%**, Pick a percentage

This sets the amount of maximum health a player gets after they're revived. Amounts are a percentage of a player's total health.

**Allow Revives**

***Yes***, No

When set to **Yes**, you can set the **Time to Revive** and **Revive Progress Decay** below. Otherwise, those options are hidden.

**Time to Revive**

**10 Seconds**, Instant (0 seconds), Pick a time

Sets the amount of time it takes to revive a teammate in a DBNO state.

**Revive Progress Decay**

**Battle Royale**, Instant Reset, *Custom Decay*

When a player is down but not out, there is a limit to how long the player can remain in this state before either being revived by another player or being fully eliminated. This limit is called **decay**. This setting controls that decay.

-
**Battle Royale:** Uses the Battle Royale decay rate.

-
**Instant Reset:** Instantly resets the decay to zero.

-
**Custom Decay:** Allows you to set a custom multiplier on the decay rate. When set to Custom Decay, the next option, **Decay Rate Multiplier**, is available.

**Decay Rate Multiplier**

**1.0X**, Pick a number

Choose a multiplier based on a constant value that is not related to Battle Royale. This option only shows if **Revive Progress Decay** is set to **Custom Decay**.

**Shakedowns**

***On***, Off

Determines whether downed players can be [shaken down](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary). If set to **On**, the **Alert Team When Downed** option becomes available.

**Show Player Location on Shakedown**

**Yes**, No

Sets whether shaking down reveals the location of the downed player’s teammates. This option is only available when **Shakedowns** is set to **On**.

**Alert Team When Downed**

**On**, Off

If set to **On**, the teammate-is-down sound alert activates. If set to **Off**, no sound plays when a teammate is down.

**Last Man Standing Mode**

**No**, Yes

If set to **Yes**, the game will not end when the last player on a team is downed; the game ends only when all players are completely eliminated.

If you have Last Man Standing Mode set to **Yes**, but no teams are set up on your island, a single player could go into DBNO status with no way to get out.

**Selected Class**

**Any**, All, No Class, Pick a class

Determines which [class](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) or classes the DBNO rules apply to.

-
**Any**: DBNO rules apply to all players, even those without an assigned class.

-
**All**: DBNO rules apply to all players with an assigned class.

-
**No Class**: DBNO rules apply to players without a class assigned.

**Invert Class Selection**

**All But Selected**, Only Selected

The class of the triggering player is inverted:

-
**All But Selected:** The chosen class is the only "safe" class, they won't be affected by the device.

-
**Only Selected:** The chosen class, including "No Class", is the only one affected by this device.

**Selected Team**

**Any**, None, Pick a team

Determines which team or teams the DBNO rules apply to.

**Invert Team Selection**

**All But Selected**, Only Selected

The team of the triggering player is inverted:

-
**All But Selected:** The chosen team is the only "safe" team, they won't be affected by the device.

-
**Only Selected:** The chosen team, including "No Team", is the only one affected by this device.

**Allow Carry**

**Yes**, No

If this option is set to **Yes**, enemy players are able to carry or throw downed players. Allies are always able to carry a downed player, whether this is set to Yes or No.

**Downed Invincibility Time**

**Don't Override**, Pick a time

How long a player is invincible when downed.

### Direct Event Binding

Following are the [direct event binding](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) options for this device.

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

Enables the device when an event occurs.

##### Disable When Receiving From

Disables the device when an event occurs.

##### Down Player When Receiving From

The [instigating](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) player is placed into the downed state when an event occurs.

##### Revive Player When Receiving From

Revives the activating player when an event occurs.

#### Events

Direct event binding uses events as transmitters. An event tells another device to perform a function.

-
For any event option, click the **option**, then **Select Device** to access and select from the **Device dropdown menu**.

-
Once you've selected a device, click **Select Function** to bind the event to a function for that device.

-
If more than one function is triggered by the event, press the **Add** button and repeat.

**אפשרויות ותיאורים:**

##### On Player Downed Send Event To

When a player is downed, an event is sent to the selected device.

##### On Player is Picked Up Send Event To

When a player is picked up, an event is sent to the selected device.

##### On Player Thrown Send Event To

When a player is thrown, an event is sent to the selected device.

##### On Player Dropped Send Event To

When a player is dropped, an event is sent to the selected device.

##### On Player Revived Send Event To

When a player is revived, an event is sent to the selected device.

##### On Shakedown Send Event To

When a player shakes down a downed player, an event is sent to the selected device.

##### On Shaken Down Send Event To

When a player is shaken down by another player, an event is sent to the selected device.

---

## Using First Person Camera Devices in Fortnite Creative

**כותרת מקורית:** Using First Person Camera Devices in Fortnite Creative  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/using-first-person-camera-devices-in-fortnite-creative  
**מקור קלט:** `07C_שחקנים_קבוצות_תפקידים_ומצלמות(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `using-first-person-camera-devices-in-fortnite-creative`

The **First Person Camera** device is a camera and controls device you can use to put players into a first-person perspective, so you can create First Person Shooters and other first-person perspective games.

If you're using multiple copies of a device on an island, it can be useful to [rename](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) them. Choosing names that relate to a device's purpose makes it easier to remember what each one does, and easier to find a specific device when using the [Event Browser](https://dev.epicgames.com/documentation/fortnite/event-browser-in-fortnite-creative).

### Finding the Device in Creative

There are multiple ways to search and browse through the **Devices** category to find the First Person Camera.

*   Use the **search bar** to search for a specific device by name. Enter "first person" or "camera" to narrow your search.

*   Explore devices by using **tags**. In the right panel, check the box for any specific keywords you want to use. If you select multiple tags, devices that have any of the selected tags are shown. If you want to get more specific, click **Intersect** above the tag list. This will show only devices that have all the tags you selected.

*   Click the **Sort** button, above the displayed device tiles, to sort the results alphabetically. Clicking this button cycles through the different sorting patterns: Default, A-Z, and Z-A.

### Finding the Device in UEFN

If you want to use this device in UEFN, this section shows you how to find it.

There are several ways you can find the **First Person Camera** device in UEFN.

*   You can click **Content Drawer** at the bottom left of the editor. When the drawer pops up, look in the side navigation panel and you'll see a folder tree. Click **Fortnite > Devices > !Beta**. The device is in this folder. Drag it into your viewport to add it to your scene.

[![Image 1: Open the Content Drawer](https://dev.epicgames.com/community/api/documentation/image/931f5739-a029-4b45-990d-41e0eae91bf4)](https://dev.epicgames.com/community/api/documentation/image/931f5739-a029-4b45-990d-41e0eae91bf4?resizing_type=fit)
*   You can open a **Content Browser** window and dock it below your viewport. Then use the side navigation panel and click **Fortnite > Devices > !Beta**.

[![Image 2: Open a Content Browser](https://dev.epicgames.com/community/api/documentation/image/74b3e56d-e6b5-48ee-8068-5756b823b8c4)](https://dev.epicgames.com/community/api/documentation/image/74b3e56d-e6b5-48ee-8068-5756b823b8c4?resizing_type=fit)
*   In the Content Browser, you can use the **Search** bar to find your device by typing in part of the device's name (such as "first person").

### Camera Terms and Definitions

When developers use a game engine to build a game, they use cameras for lots of different purposes. There are some specialized terms used for these in-game cameras that you might be unfamiliar with. Many of these terms are used in the device options for this and other camera devices. The table below lists these terms and their definitions.

| Term | Definition |
| --- | --- |
| **Field of View** | The term **field of view** refers to what the camera can actually "see". The field of view is represented as an angle, and is measured in degrees. Angles have two sides, joined at a point called the vertex. With cameras, the vertex is the lens (virtual in this case) of the camera. The arms of the angle spread up and down (the vertical axis) from that vertex. The higher the number of degrees, the wider the angle, and the more the camera can see. |
| **Pitch, Yaw** | **Pitch** and **yaw** are terms originating in aviation. They refer to the different types of rotation a plane can perform when moving. These terms were adopted into 3D design and game development, to more precisely define a virtual 3D environment and how things are positioned in that virtual space. Pitch and yaw are measured relative to the object's original position. **Pitch** refers to up and down movement of an object, and **yaw** refers to horizontal left or right movement of an object. The _axis of rotation_ is different from the direction of movement. For example, if a plane _pitches_, the nose of the plane moves up or down; but the plane is _rotating_ on the _Y axis_(which is the left-right or east-west horizontal axis). See the terms X-axis,Y-axis, and Z-axis in this table. |
| **Angle Pitch** | This is a measurement of how much the camera points up or down while framing its target. |
| **Angle Yaw** | This is a measurement of how much the camera turns left or right while framing its target. |
| **Camera Offset** | Normally the camera view centers on its target. The **camera****offset** is how far from the center the camera view is. The camera can have an offset amount on the X-, Y-, or Z-axis and it can have an offset on more than one axis at a time. |
| **X-axis** | In a 3D space (real or virtual), the X-axis represents horizontal forward/backward (or north/south) movement. |
| **Y-axis** | In a 3D space (real or virtual), the Y-axis represents horizontal left/right (or east/west) movement. |
| **Z-axis** | In a 3D space (real or virtual), the Z-axis represents vertical up/down movement. |
| **Transition In Type** | * Ease In: The camera transition will start slowly and speed up as it continues. * Ease Out: The camera transition will slow down as it ends. * Ease In-Out: The camera transition will start slowly, speed up, then slow again as it ends. * Linear: The camera transition moves smoothly from one camera to another at the same speed. * Fade: The image gradually becomes visible when fading in, or gradually becomes blank when fading out. When Fade is selected an additional fade option become available;_Fade in Hold Time_. |
| **Transition Out Type** | * **Ease In**: The camera transition will start slowly and speed up as it continues. * **Ease Out**: The camera transition will slow down as it ends. * **Ease In-Out**: The camera transition will start slowly, speed up, then slow again as it ends. * **Linear**: The camera transition moves smoothly from one camera to another at the same speed. * **Fade**: The image gradually becomes visible when fading in, or gradually becomes blank when fading out. When Fade is selected an additional fade option become available; _Fade Out Hold Time_. |
| **Priority System** | If multiple cameras are assigned to a player, priority determines which camera is active at any point in time. Priority can be set in the device options. If two cameras are tied for the highest priority, the most recently added camera will become active. |
| **Boom Collision** | In film, a boom jib is an apparatus that holds the camera. Boom operators can move and orient the camera with levers and wheels to get the shot they desire. The Boom Collision properties for fixed angle cameras allow you to determine the behavior of that camera when an object in the scene gets between the camera and its target. |
| **Deadzone** | The deadzone refers to an established area within which the target can move around without affecting the camera. When the target moves to an edge of the deadzone, the camera will move to follow the target. |

### Contextual Filtering

Some devices are affected by a feature called **contextual filtering**. This feature hides or displays options depending on the values selected for certain related options. This reduces clutter in the Customize panel and makes options easier to manage and navigate. To help identify them, values that trigger contextual filtering are in _italic_.

All options are listed, including those affected by contextual filtering; if they are hidden or displayed based on a specific option's value, there will be a note about it in the Description field for that option.

### Device Options

Default values are **bold**. Values that trigger contextual filtering are _italic_.

You can configure this device with the following options.

| Option | Value | Description |
| --- | --- | --- |
| Creative Preview | Start | Click Start to preview the controls. Click Stop to leave the preview and go back to editing your island. |
| **Priority** | **0**, Pick or enter a number | Determines where this camera falls in the priority system. When multiple cameras are added to a player, the camera with the highest priority is considered the active camera. Use higher numbers to indicate higher priority. If two cameras are tied for the highest priority, the most recently added will become active. |
| **Enabled During Phase** | None, **Always**, Pre-Game Only, Gameplay Only | Determines which game phase the device is enabled. |
| **Remove on Elimination** | On, **Off** | Automatically removes the camera from the player upon elimination. |
| **Add to Players on Start** | **On**, Off | Determines whether this camera is automatically added to all players when the game starts. |
| **Preview Device Color** | **#74ABFFFF**, Pick a color | Click the swatch to open the color picker. Scroll to browse through color swatches, or enter a Hex code in the Search bar to find a specific color. Click the swatch to select it, then click the checkmark to close the Color Picker. [![Image 3: Color Picker](https://dev.epicgames.com/community/api/documentation/image/6f94700d-4737-4744-9d6e-3d27a939f858)](https://dev.epicgames.com/community/api/documentation/image/6f94700d-4737-4744-9d6e-3d27a939f858?resizing_type=fit) |
| **Use as Elimination Camera** | **No**, Yes, Elimination Only | Values from this camera will be used to drive the elimination camera. It will utilize the Field of View, Rotation, and Location Offset, or Location of the Camera. It will also use the Transition In Time to move the elimination camera from where the camera was upon elimination to its new location and rotation. |
| **Interaction Distance** | **Close**, Standard, Far | Scale of the distance a player must be from interactable objects to trigger the interaction prompt. |
| **Focus Target Override** | **None**, Select a Target | This option only becomes available when the **Look at Target** option is set to **On**. Override object becomes the camera focus target. Does nothing if set to None. |
| **Field of View** | **80 Degrees**, Select an angle | Determines the degrees on the vertical (Y) axis the camera can view |
| **Targeting Reticle** | Display All, Reticle Only, Ammo Count Only, Display None | If set to On, the camera will support screen shake events in game. |
| **Affects Team** | **Any**, Pick or enter a team | Determines which team is affected by this device. **Note**: the camera does react dynamically to changes in team during the game. If your game involves or allows players to change teams, you may have to figure out how to manually re-add cameras to those players. |
| **Affects Class** | No Class, **Any**, Pick or enter a class | Determines which classes are affected by this device. **No Class** means only players with no assigned class are affected. **Any** means all players, including those with no assigned class, are affected. |
| **Invert Team** | On, **Off** | If this is set to **On**, all teams are affected by this device except the team selected in the **Affects Team** option. |
| **Invert Class** | On, **Off** | If this is set to **On**, all classes are affected by this device except the class selected in the **Affects Class** option. |
| **Transition In Priority** | **0**, Pick or enter a number | This is the priority used when this camera is the destination for a transition. |
| **Transition In Time** | **0.2**, Pick or enter an amount | This is how long the transition lasts when this camera is the destination. |
| **Transition In Type** | Linear, Ease-In, Ease-Out, **Ease-In-Out _, Fade_** | This determines what type of transition this camera uses when it is the destination camera. When this option is set to Fade the Fade In Hold Time option becomes available. |
| **Transition Out Priority** | **0**, Pick or enter a number | This is the priority used when this camera transitions to another. |
| **Transition Out Time** | **0.2**, Pick or enter an amount | This is how long the transition lasts when this camera is the origin camera for a transition. |
| **Transition Out Type** | Linear, Ease-In, Ease-Out, **Ease-In-Out, _Fade_** | This determines what type of transition this camera uses when it is the origin camera for a transition. When this option is set to Fade the Fade Out Hold Time option becomes available. |
| **Look at Focus Target on Activate** | _On_, **Off** | This option only becomes available when the Look at Target option is set to On. If set to **On**, look at the focus target override when this camera is activated. |
| **Fade In Hold Time** | **0.0 s**, Select the seconds | This option becomes available when Transition In Type is set to **Fade**. Determines the total time in seconds for the fade-in effect when using fade-type transitions. |
| **Fade Out Hold Time** | **0.0s**, Select the seconds | This option becomes available when Transition Out Type is set to Fade. Determines the total time in seconds for the fade-in effect when using fade-type transitions. |

### Direct Event Binding

Following are the [direct event binding](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) options for this device.

#### Functions

A [function](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) listens for an event on a device then performs an action.

1.   For any function, click the **option**, then **Select Device** to access and select from the **Device** dropdown menu.

2.   Once you've selected a device, click **Select Event** to bind the device to an event that will trigger the function.

3.   If more than one device or event triggers a function, click the **Add** button to add a line and repeat these steps.

| Option | Description |
| --- | --- |
| **Enable When Receiving From** | Enables the camera when an event occurs. |
| **Disable When Receiving From** | Disables the camera when an event occurs. |
| **Add to Player When Receiving From** | Adds this camera to the instigating player when an event occurs. |
| **Remove from Player When Receiving From** | Removes this camera from the instigating player when an event occurs. |
| **Add to All When Receiving From** | Adds this camera to all players when an event occurs. |
| **Remove from All When Receiving From** | Removes this camera from all players when an event occurs. |
| **Focus on Target When Receiving From** | Sets the target of the camera to the focus target instead of the player, for all players. |
| **Focus on Player When Receiving From** | Sets the target of the camera to the player, for all players. |

#### Events

This device has no events.

---

## Using Fixed Angle Camera Devices in Fortnite Creative

**כותרת מקורית:** Using Fixed Angle Camera Devices in Fortnite Creative  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/using-fixed-angle-camera-devices-in-fortnite-creative  
**מקור קלט:** `07C_שחקנים_קבוצות_תפקידים_ומצלמות(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `using-fixed-angle-camera-devices-in-fortnite-creative`

You can use the **Fixed Angle Camera** device to override the default Fortnite camera, giving you a freedom to create entirely new types of gameplay and new [game genres](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary).

When you place the Fixed Angle Camera, it will frame a **look-at [target](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary)** and move to follow that target when the target moves. You can customize how the camera moves and behaves using the device options.

You will need to use a [Third Person Controls](https://dev.epicgames.com/documentation/fortnite/using-third-person-controls-devices-in-fortnite-creative) device with this camera. To learn more about how to use the camera and controls devices together, see [Designing with Cameras and Controls](https://dev.epicgames.com/documentation/fortnite/designing-with-cameras-and-controls-in-fortnite-creative).

To learn about using cameras in UEFN, see:

-
[Gameplay Camera and Control Devices](https://dev.epicgames.com/documentation/en-us/uefn/gameplay-camera-and-control-devices-in-unreal-editor-for-fortnite)

-
[Making a Title Sequence](https://dev.epicgames.com/documentation/en-us/uefn/making-a-title-sequence-in-unreal-editor-for-fortnite) for a gameplay example

To find the Fixed Angle Camera device, press the **M** key and then click the **Content** tab to open the Creative inventory. Select the **Devices** category. From there, you can search or browse for the device. For more information on finding devices see [Using Devices](https://dev.epicgames.com/documentation/fortnite/using-devices-in-fortnite).

### Camera Terms and Definitions

When developers use a game engine to build a game, they use cameras for lots of different purposes. There are some specialized terms used for these in-game cameras that you might be unfamiliar with. Many of these terms are used in the device options for this and other camera devices. The table below lists some of these terms and their definitions.

 Term Definition
**Field of View**

The term **field of view** (or **FOV** for short) refers to what the camera can actually "see". The field of view is represented as an angle, and is measured in degrees. Angles have two sides, joined at a point called the **vertex**. With cameras, the vertex is the lens (virtual in this case) of the camera. The arms of the angle spread up and down (the vertical axis) from that vertex. The higher the number of degrees, the wider the angle, and the more the camera can see.

**Pitch, Yaw**

**Pitch** and **yaw** are terms originating in aviation. They refer to the different types of rotation a plane can perform when moving. These terms were adopted into 3D design and game development to more precisely define a virtual 3D environment and how things are positioned in that virtual space. Pitch and yaw are measured relative to the object's original position. **Pitch** refers to up and down movement of an object, and **yaw** refers to horizontal left or right movement of an object. **Note**: the **axis of rotation** is different from the direction of movement. For example, if a plane **pitches**, the nose of the plane moves up or down; but the plane is **rotating** on the Y-axis (which is the left-right or east-west horizontal axis). See the terms **X-axis**, **Y-axis**, and **Z-axis** in this table.

**Angle Pitch**

This is a measurement of how much the camera points up or down while framing its target.

**Angle Yaw**

This is a measurement of how much the camera turns left or right while framing its target.

**Camera Offset**

Normally the camera view centers on its target. The **camera offset** is how far from the center the camera view is. The camera can have an offset amount on the X-, Y-, or Z-axis and it can have an offset on more than one axis at a time.

**X-axis**

In a 3D space (real or virtual), the X-axis represents horizontal forward/backward (or north/south) movement.

**Y-axis**

In a 3D space (real or virtual), the Y-axis represents horizontal left/right (or east/west) movement.

**Z-axis**

In a 3D space (real or virtual), the Z-axis represents vertical up/down movement.

**Camera Transition**

When you have multiple cameras active, a **transition** is when you move from one camera view to another. In Fortnite, camera devices have an **In Priority** and an **Out Priority**. The camera transition is determined by the highest priority, comparing the Out Priority of the current camera with the In Priority of the destination camera.

**Transition Types**

**Ease In**: the camera transition will start slowly and speed up as it continues. **Ease Out**: the camera transition will slow down as it ends. **Ease In-Out**: the camera transition will start slowly, speed up, then slow again as it ends. **Linear**: the camera transition moves smoothly from one camera to another at the same speed. **Fade**: The camera will fade in from black and fade out to black.

**Priority System**

If multiple cameras are assigned to a player, priority determines which camera is active at any point in time. Priority can be set in the device options. If two cameras are tied for the highest priority, the most recently added camera will become active.

**Boom Collision**

In film, a boom jib is an apparatus that holds the camera. Boom operators can move and orient the camera with levers and wheels to get the shot they desire. The Boom Collision properties for fixed angle cameras allow you to determine the behavior of that camera when an object in the scene gets between the camera and its target.

**Deadzone**

The **deadzone** refers to an established area within which the target can move around without affecting the camera. When the target moves to an edge of the deadzone, the camera will move to follow the target.

**Look-at Location**

Where the camera is looking at any time. With the orbit camera, it might be something other than the player.

**Soft Deadzone**

The area inside of the deadzone where the camera starts to accelerate to follow the player. This area blends the look-at location between remaining stationary and following the target.

### Contextual Filtering

Some devices are affected by a feature called **contextual filtering**. This feature hides or displays options depending on the values selected for certain related options. This feature will reduce clutter in the Customize panel and make options easier to manage and navigate.

However, it may not be easy to recognize which options or values trigger contextual filtering. To help you identify them, in our device docs we use *italic* for any values that trigger contextual filtering. All options will be listed, including those affected by contextual filtering; if they are hidden or displayed based on a specific option's value, there will be a note about that in the Description field for that option.

### Device Options

Configure this device with the following options.
**

Default values are **bold**. Values that trigger contextual filtering are *italic*.

 Option Value Description
**Priority**

**0**, Pick or enter a number

Determines where this camera falls in the priority system. When multiple cameras are added to a player, the camera with the highest priority is considered the active camera.

**Enabled During Phase**

None, **Always**, Gameplay Only

Determines which phases the camera is active in. If you choose **None**, the camera can only be enabled manually using events.

**Remove on Elimination**

On, **Off**

Determines whether this camera is removed from a player when they are eliminated.

**Add to Players on Start**

**On**, Off

Determines whether this camera is automatically added to all players when the game starts.

Use as Elimination Camera**

**No**, Yes, Elimination Only

Values from this camera are used to drive the elimination camera.

It uses the **Field of View**, **Rotation**, and **Location Offset** or **Location** of the camera.

It also uses the **Transition In Time** to move the camera from where the camera was upon elimination to its new location and rotation.

**Field of View**

**80**, Pick or enter a number of degrees from 20-120

This option only displays if the **Projection Mode** option is set to **Perspective**. The term **field of view** refers to what the camera can actually see.

This setting determines the angle on the vertical axis, in degrees, that represents the Field of View for this camera.

A higher number makes a wider angle, which results in a larger field of view.

**Camera Shake**

On, **Off**

If this is set to **On**, the camera will support screen shake events in the game.

**Focus Target Override**

**None**, Pick a target

Override object for the camera focus target. Does nothing if set to None.

**Look At Focus Target On Activate**

On, **Off**

If this is set to **On**, then when the camera activates it looks at the focus target override.

**Projection Mode**

**Perspective**, *Orthographic*

Determines whether the camera is using Perspective or Orthographic projection.

If you choose **Orthographic**, an additional option displays.

**Projection Width**

**1000 PPI**, Pick or enter a width

This option only displays if the **Projection Mode** option is set to **Orthographic**.

 Determines how wide a view the camera projects in orthographic mode.

**Distance**

**1200 cm**, Pick or enter a number

This option only displays if the **Projection Mode** option is set to **Perspective**.

 Determines the distance between the camera and the player.

**Affects Team**

**Any**, Pick or enter a team

Determines which team is affected by this device.
**

The camera does react dynamically to changes in team during the game. If your game involves or allows players to change teams, you may have to figure out how to manually re-add cameras to those players.

**Affects Class**

No Class, **Any**, Pick or enter a class

Determines which classes are affected by this device.

-
No Class means only players with no assigned class are affected.

-
Any means all players, including those with no assigned class, are affected.

**Invert Team**

On, **Off**

If this is set to **On**, all teams are affected by this device except the team selected in the **Affects Team** option.

**Invert Class**

On, **Off**

If this is set to **On**, all classes are affected by this device except the class selected in the **Affects Class** option.

**Transition In Priority**

**0**, Pick or enter a number

This is the priority used when this camera is the destination for a transition.

**Transition In Time**

**0.2**, Pick or enter an amount

This is how long the transition lasts when this camera is the destination.

**Transition In Type**

Linear, Ease-In, Ease-Out, **Ease-In-Out**, Fade

This determines what type of transition this camera uses when it is the destination camera.

**Transition Out Priority**

**0**, Pick or enter a number

This is the priority used when this camera transitions to another.

**Transition Out Time**

**0.2**, Pick or enter an amount

This is how long the transition lasts when this camera is the origin camera for a transition.

**Transition Out Type**

Linear, Ease-In, Ease-Out, **Ease-In-Out**, Fade

This determines what type of transition this camera uses when it is the origin camera for a transition.

**Angle Pitch**

**-65 degrees**, Pick or enter a number of degrees

From the camera's position, this determines how much the camera rotates up or down around the player.

**Angle Yaw**

**0 degrees**, Pick or enter a positive or negative number

From the camera's position, this determines how much the camera rotates left or right around the player.

**Angle Roll**

**0 degrees**, Pick or enter a positive or negative number

From the camera's position, this determines how much the camera rotates in place, tilting left or right.

**Offset X**

**0 cm**, Pick or enter a positive or negative number

This setting can move the view forward or back, relative to the camera's position.

A positive number moves the view forward, a negative number moves the view backward.

**Offset Y**

**0 cm**, Pick or enter a positive or negative number

Normally the camera view centers on its target.

This setting can move the view left or right, relative to the camera's position.

A positive number moves the view to the left, a negative number moves the view to the right.

**Offset Z**

**0 cm**, Pick or enter a positive or negative number

Normally the camera view centers on its target.

This setting can move the view up or down, relative to the camera's position.

A positive number moves the view down, a negative number moves the view up.

**Horizontal Speed**

**10 cm/s**, Pick or enter a number

Determines the speed at which the camera moves in the X axis (forward/back) and Y axis (left/right) in order to frame the target.

**Vertical Speed**

**10 cm/s**, Pick or enter a number

Determines the speed at which the camera moves in the Z axis (up/down) in order to frame the target.

**Preview Device Color**

**#74ABFFFF**, Pick a color

Click the swatch to open the color picker.

Scroll to browse through color swatches, or enter a Hex code in the Search bar to find a specific color.

Click the swatch to select it, then click the checkmark to close the Color Picker.

**Preview Mannequin**

**On**, Off

If this is set to **On**, a holographic preview of a mannequin will display, showing a player's relationship to the camera.

This can help you visualize what the player will see with this camera assigned so you can tune the settings for the camera more precisely.

**Show Dead Zone in Preview**

On, **Off**

If this is set to **On**, a preview of the Deadzone will be visible when previewing this camera.

**Transition In Priority**

**0**, Pick or enter a number

This is the priority used when this camera is the destination for a transition.

**Transition In Time**

**0.2 seconds**, Pick or enter an amount

This is how long the transition lasts when this camera is the destination.

Fade In Hole Time**

 0.0 s, Pick an amount

This option only becomes available when **Transition In Type** is set to **Fade**.

Determines the total time in seconds for the fade-in effect when using fade-type transitions.

**Transition In Type**

Linear, Ease-In, Ease-Out, **Ease-In-Out**, *Fade*

This determines what type of transition this camera uses when it is the destination camera.

**Transition Out Priority**

**0**, Pick or enter a number

This is the priority used when this camera transitions to another.

**Transition Out Time**

**0.2 seconds**, Pick or enter an amount

This is how long the transition lasts when this camera is the origin camera for a transition.

**Fade Out Hold Time**

**0.0 s**, Pick an amount

This option only becomes available when **Transition Out Type** is set to **Fade**.

Determines the total time in seconds for the fade-in effect when using fade-type transitions.

**Transition Out Type**

Linear, Ease-In, Ease-Out, **Ease-In-Out**, *Fade*

This determines what type of transition this camera uses when it is the origin camera for a transition.

**Boom Collision**

*On*, **Off**

By default, boom collision is off. This means objects in the world that are between the camera and its target will hide the target.

If you set this to **On**, additional options display that you can use to set different behaviors that occur when something is between the camera and its target.

**Collision Type**

Instant, ***Predictive***, *Transparency*

This option only displays if the **Boom Collision** option is set to **On**.

This option determines what the camera does if objects in the world obscure the target.

 If this option is set to **Predictive**, two additional options are displayed below this one.

If this option is set to **Transparency**, three additional options are displayed below this one.

**Collision In Time**

**0.5**, Pick or enter an amount

This option only displays if the **Collision Type** option is set to **Predictive**.

Determines how fast the camera pulls in when using Predictive Collision.

**Collision Out Time**

**0.5**, Pick or enter an amount

This option only displays if the **Collision Type** option is set to **Instant** or **Predictive**.

Determines how fast the camera pulls out when using Predictive Collision.

**Transparency Collision Radius**

**5.0 cm**, Pick or enter an amount

The radius from the camera's path to its target. This is used to identify which objects to make transparent.

**Transparency Amount**

**0.4**, Pick an amount

This option only displays if the **Collision Type** option is set to **Transparency**.

Determines how opaque objects are when they break the line of sight of your character. **0** means they are totally transparent; **1** means they are totally opaque.

**Transparency Cutout Radius**

**100cm**, Pick or enter an amount

This option only displays if the **Collision Type** option is set to **Transparency**.

Determines an area of full transparency around the camera target when a boom collision has occurred.

**Deadzone**

*On*, **Off**

If you choose **On**, this establishes an area within which the target can move without affecting the camera.

When the target reaches the edge of the deadzone, the camera will move to follow the target. If you choose **On**, additional options display.

**Deadzone Type**

Sphere, ***Cylinder***, *Rectangle*

This option only displays if the **Deadzone** option is set to **On**.

This determines the shape of the deadzone.

**Deadzone Height**

**0 cm**, Pick or enter an amount

This option displays if the **Deadzone Type** option is set to **Cylinder** or **Rectangle**.

 Determines the height of the deadzone.

**Deadzone Width**

**100 cm**, Pick or enter an amount

This option only displays if the **Deadzone Type** option is set to **Rectangle**.

Determines the width of the deadzone.

**Deadzone Depth**

**100 cm**, Pick or enter an amount

This option only displays if the **Deadzone Type** option is set to **Rectangle.**

**Deadzone Diameter**

**100 cm**, Pick or enter an amount

This option displays if the **Deadzone Type** option is set to **Sphere** or **Cylinder**.

**Deadzone Soft Percent**

**100\%**, Pick or enter a percentage

Determines an area within the deadzone where the camera blends between remaining stationary and following the player.

**Deadzone Jump Size**

**Off**, Pick or enter a size

If you specify a size, it determines the area within which a player can jump up and down without the camera following them.

**Boundary**

*On*, **Off**

If this is set to **On**, you can use the seven additional options that display below this one, to define specific boundaries for where the camera can move on the X-, Y- and Z-axes.

**Boundary Preview**

**On**, Off

This option only displays if the **Boundary** option is set to **On**.

If this option is set to **On**, a holographic preview of the set boundaries will display while you are editing your island.

**Boundary X Min**

**0 cm**, Pick or enter a positive or negative number

This option only displays if the **Boundary** option is set to **On**.

This determines how far backward the camera can move on the X axis.

**Boundary X Max**

**0 cm**, Pick or enter a positive number

This option only displays if the **Boundary** option is set to **On**.

This determines how far forward the camera can move on the X axis.

**Boundary Y Min**

**Off**, Pick or enter a positive or negative number

This option only displays if the **Boundary** option is set to **On**.

This determines how far to the right the camera can move on the Y axis.

**Boundary Y Max**

**Off**, Pick or enter a positive number

This option only displays if the **Boundary** option is set to **On**.

This determines how far to the left the camera can move on the Y axis.

**Boundary Z Min**

**Off**, Pick or enter a positive or negative number

This option only displays if the **Boundary** option is set to **On**.

This determines how far upward the camera can move on the Z axis.

**Boundary Z Max**

**Off**, Pick or enter a positive number

This option only displays if the **Boundary** option is set to **On**.

This determines how far downward the camera can move on the Z axis.

**POI Framing**

*On*, **Off**

Provides away to use point of interest framing to keep players in range on screen.

When this option is set to On, additional POI Framing options become availabel.

**POI Framing Type**

**Zoom to Fit**, *LookAtOffset*

Determines which method Point of Interest Framing uses.

Zoom to Fit pulls the camera back to keep all targets in range on screen.

Offset slides the camera to keep all targets in range on screen.

When this option is set to LookAtOffset, additional offset options become available.

**POI Framing Actor Tracking Acrivation Angle**

**40.00**, Select an amount

The Field of View extent defines when other targets should be included in actor tracking calculations.

It is advised to set the amount to roughly half the Field of View of your camera.

**POI Framing Actor Tracking Falloff Distance**

**1,500.0 CM**, Select an amount

The distance extent that defines when other targets should be removed from actor tracking calculations.

**POI Framing Movement Sharpness**

**1.0**, Select an amount

Sets how tightly the camera's move and zoom actions perform while POI Framing is enabled.

Higher values equal tighter tracking.

**POI Framing Own Player Weight**

**1.0**, Select an amount

Determines how much preference the camera gives toward the owning player when framing the shot.

This option becomes available when the LookAtOffset options is selected.

**POI Framing Other Player Weight**

0.25, Select an amount

Determines how much preference the camera gives toward the non owning player when framing the shot.

This option becomes available when the LookAtOffset options is selected.

**POI Framing Target Frame Time**

**1.0**, Select an amount

Determines how much time it takes to reposition the camera upon changing targets.

**POI Framing Target Decay Time**

**1.0**, Select an amount

Determines how much time it takes to reposition the camera upon having no targets beyond the controlling player.

**POI Framing Zoom to Fit Max Offset**

**1200.0 CM**, Select an amount

Determines how much the Zoom To Fit option affects the zoom out capabilities of the furthest back camera.

### Direct Event Binding

Following are the [direct event binding](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) options for this device.

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

Enables the camera when an event occurs.

##### Disable When Receiving From

Disables the camera when an event occurs.

##### Add to Player When Receiving From

Adds this camera to the instigating player when an event occurs.

##### Add to All When Receiving From

Adds this camera to all players when an event occurs.

##### Remove from Player When Receiving From

Removes this camera from the instigating player when an event occurs.

##### Remove from All When Receiving From

Removes this camera from all players when an event occurs.

##### Focus On Target When Receiving From

When an event occurs, this function sets the camera to focus on a target instead of focusing on the player.

##### Focus On Player When Receiving From

When an event occurs, this function sets the camera to focus on the player. This applies to all players.

#### Events

This device has no events.

### Use Fixed Angle Camera In Verse

You can use the code below to control a Fixed Angle Camera device in [Verse](https://dev.epicgames.com/documentation/en-us/uefn/learn-programming-with-verse-in-unreal-editor-for-fortnite). This code shows how to use events and functions in the Fixed Angle Camera device API. Modify it to fit the needs of your experience.

using { /Fortnite.com/Devices }
using { /Verse.org/Simulation }
using { /UnrealEngine.com/Temporary/Diagnostics }

## A Verse-authored creative device that can be placed in a level
gameplay_camera_fixed_angle_device_verse_example := class(creative_device):
 # Reference to the Gameplay Camera Fixed Angle Device in the level.
 # In the Details panel for this Verse device,
 # set this property to your Gameplay Camera Fixed Angle Device.
 @editable

Expand code Copy full snippet(23 lines long)

To use this code in your UEFN experience, follow these steps.

-
Drag a Fixed Angle Camera device onto your island.

-
Create a new Verse device named **gameplay_camera_fixed_angle_device_verse_example**. See [Create Your Own Device Using Verse](https://dev.epicgames.com/documentation/en-us/uefn/create-your-own-device-in-verse#creatinganewdevicewithverse) for steps.

-
In Visual Studio Code, open **gameplay_camera_fixed_angle_device_verse_example.verse** in Visual Studio Code and paste the code above.

-
Compile your code and drag your Verse-authored device onto your island. See [Adding Your Verse Device to Your Level](https://dev.epicgames.com/documentation/en-us/uefn/create-your-own-device-in-verse#addingyourversedevicetoyourlevel) for steps.

-
Add a reference for the Fixed Angle Camera device on your island to your Verse device. See [Adding a Verse Reference to a Creative Device in Your Level](https://dev.epicgames.com/documentation/en-us/uefn/customize-verse-device-properties-in-verse#addingaversereferencetoacreativedeviceinyourlevel) for steps.

Disable the **Add to Players on Start** property of the Camera device so that only Verse will add the camera to the player.

-
Save your project and click **Launch Session** to playtest.

#### Fixed Angle Camera API

See the [gameplay_camera_fixed_angle_device API Reference](https://dev.epicgames.com/documentation/en-us/uefn/verse-api/fortnitedotcom/devices/gameplay_camera_fixed_angle_device) for more information on using the Fixed Angle Camera device in Verse.

---

## Using Fixed Point Camera Devices in Fortnite Creative

**כותרת מקורית:** Using Fixed Point Camera Devices in Fortnite Creative  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/using-fixed-point-camera-devices-in-fortnite-creative  
**מקור קלט:** `07C_שחקנים_קבוצות_תפקידים_ומצלמות(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `using-fixed-point-camera-devices-in-fortnite-creative`

The **Fixed Point Camera** device can be used to override the default Fortnite camera, giving you the freedom to create entirely new types of gameplay and new [game genres](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary). Place the Fixed Point Camera in a specific location where you want the player's view to focus on a specific object, character, or area. You can use the device options to specify if the camera stays still, or if it can rotate up and down or turn left and right, in order to keep a target in-frame.

You will need to use a [Third Person Controls](https://dev.epicgames.com/documentation/fortnite/using-third-person-controls-devices-in-fortnite-creative) device with this camera. To learn more about how to use the camera and controls devices together, see [Designing with Cameras and Controls](https://dev.epicgames.com/documentation/fortnite/designing-with-cameras-and-controls-in-fortnite-creative).

To learn about using cameras in UEFN, see:

-
[Gameplay Camera and Control Devices](https://dev.epicgames.com/documentation/en-us/uefn/gameplay-camera-and-control-devices-in-unreal-editor-for-fortnite)

-
[Making a Title Sequence](https://dev.epicgames.com/documentation/en-us/uefn/making-a-title-sequence-in-unreal-editor-for-fortnite) for a gameplay example

To find the Fixed Point Camera device, press the **M** key and then click the **Content** tab to open the **Creative inventory**. Select the **Devices** category. From there you can search or browse for the device. For more information on finding devices see [Using Devices](https://dev.epicgames.com/documentation/fortnite/using-devices-in-fortnite).

### Camera Terms and Definitions

When developers use a game engine to build a game, they use cameras for lots of different purposes. There are some specialized terms used for these in-game cameras that you might be unfamiliar with. Many of these terms are used in the device options for this and other camera devices. The table below lists these terms and their definitions.

 Term Definition
**Field of View**

The term **field of view** (or **FOV** for short) refers to what the camera can actually "see". The field of view is represented as an angle, and is measured in degrees. Angles have two sides, joined at a point called the **vertex**. With cameras, the vertex is the lens (virtual in this case) of the camera. The arms of the angle spread up and down (the vertical axis) from that vertex. The higher the number of degrees, the wider the angle, and the more the camera can see.

**Pitch, Yaw**

**Pitch** and **yaw** are terms originating in aviation. They refer to the different types of rotation a plane can perform when moving. These terms were adopted into 3D design and game development to more precisely define a virtual 3D environment and how things are positioned in that virtual space. Pitch and yaw are measured relative to the object's original position. **Pitch** refers to up and down movement of an object, and **yaw** refers to horizontal left or right movement of an object. **Note**: the **axis of rotation** is different from the direction of movement. For example, if a plane **pitches**, the nose of the plane moves up or down; but the plane is **rotating** on the Y-axis (which is the left-right or east-west horizontal axis). See the terms **X-axis**, **Y-axis**, and **Z-axis** in this table.

**Angle Pitch**

This is a measurement of how much the camera points up or down while framing its target.

**Angle Yaw**

This is a measurement of how much the camera turns left or right while framing its target.

**Camera Offset**

Normally the camera view centers on its target. The **camera offset** is how far from the center the camera view is. The camera can have an offset amount on the X-, Y-, or Z-axis and it can have an offset on more than one axis at a time.

**X-axis**

In a 3D space (real or virtual), the X-axis represents horizontal forward/backward (or north/south) movement.

**Y-axis**

In a 3D space (real or virtual), the Y-axis represents horizontal left/right (or east/west) movement.

**Z-axis**

In a 3D space (real or virtual), the Z-axis represents vertical up/down movement.

**Camera Transition**

When you have multiple cameras active, a **transition** is when you move from one camera view to another. In Fortnite, camera devices have an **In Priority** and an **Out Priority**. The camera transition is determined by the highest priority, comparing the Out Priority of the current camera with the In Priority of the destination camera.

**Transition Types**

**Ease In**: the camera transition will start slowly and speed up as it continues. **Ease Out**: the camera transition will slow down as it ends. **Ease In-Out**: the camera transition will start slowly, speed up, then slow again as it ends. **Linear**: the camera transition moves smoothly from one camera to another at the same speed. **Fade**: the camera will fade in from black and fade out to black.

**Priority System**

If multiple cameras are assigned to a player, priority determines which camera is active at any point in time. Priority can be set in the device options. If two cameras are tied for the highest priority, the most recently added camera will become active.

**Boom Collision**

In film, a boom jib is an apparatus that holds the camera. Boom operators can move and orient the camera with levers and wheels to get the shot they desire. The Boom Collision properties for fixed angle cameras allow you to determine the behavior of that camera when an object in the scene gets between the camera and its target.

**Deadzone**

The **deadzone** refers to an established area within which the target can move around without affecting the camera. When the target moves to an edge of the deadzone, the camera will move to follow the target.

### Contextual Filtering

Some devices are affected by a feature called **contextual filtering**. This feature hides or displays options depending on the values selected for certain related options. This feature will reduce clutter in the Customize panel and make options easier to manage and navigate.

However, it may not be easy to recognize which options or values trigger contextual filtering. To help you identify them, in our device docs we use *italic* for any values that trigger contextual filtering. All options will be listed, including those affected by contextual filtering; if they are hidden or displayed based on a specific option’s value, there will be a note about that in the Description field for that option.

### Device Options

Configure this device with the following options.
**

Default values are **bold**. Values that trigger contextual filtering are *italic*.

 Option Value Description
**Priority**

**0**, Pick or enter a number

Determines where this camera falls in the priority system. When multiple cameras are added to a player, the camera with the highest priority is considered the active camera.

**Enabled During Phase**

None, **Always**, Gameplay Only

Determines which phases the camera is active in. If you choose **None**, the camera can only be enabled manually using events.

**Remove on Elimination**

On, **Off**

Determines whether this camera is removed from a player when they are eliminated.

**Add to Players on Start**

**On**, Off

Determines whether this camera is automatically added to all players when the game starts.

Use as Elimination Camera**

**No**, Yes, Elimination Only

Values from this camera are used to drive the elimination camera. It uses the Field of View, Rotation, and Location Offset or Location of the camera.

It also uses the Transition in time to move the elimination camera from where the camera was upon elimination to its new location and rotation.

**Field of View**

**80**, Pick or enter a number of degrees from 20-120

This option only displays if the **Projection Mode** option is set to **Perspective**.

The term **field of view** refers to what the camera can actually see. This setting determines the angle on the vertical axis, in degrees, that represents the Field of View for this camera.

A higher number makes a wider angle, which results in a larger field of view.

**Camera Shake**

On, **Off**

If this is set to **On**, the camera will support screen shake events in the game.

**Focus Target Override**

**None**, Select a target

This option only becomes available when **Look at Target** is set to **On**.

Override object for the camera's focus target. Does nothing if set to None.

**Look at Focus Target on Active**

On, **Off**

If set to **On**, look at the focus target override when this camera is activated.

**Projection Mode**

**Perspective**, *Orthographic*

Determines whether the camera is using Perspective or Orthographic projection.

If you choose **Orthographic**, an additional option displays.

**Projection Width**

**1024 PPI**, Pick or enter a width

This option only displays if the **Projection Mode** option is set to **Orthographic**.

Determines how wide a view the camera projects in orthographic mode.

**Affects Team**

**Any**, Pick or enter a team

Determines which team is affected by this device.
**

The camera does react dynamically to changes in team during the game. If your game involves or allows players to change teams, you may have to figure out how to manually re-add cameras to those players.

**Affects Class**

No Class, **Any**, Pick or enter a class

Determines which classes are affected by this device.

-
No Class means only players with no assigned class are affected.

-
Any means all players, including those with no assigned class, are affected.

**Invert Team**

On, **Off**

If this is set to **On**, all teams are affected by this device except the team selected in the **Affects Team** option.

**Invert Class**

On, **Off**

If this is set to **On**, all classes are affected by this device except the class selected in the **Affects Class** option.

**Preview Device Color**

**#74ABFFFF**, Pick a color

Click the swatch to open the color picker.

Scroll to browse through color swatches, or enter a Hex code in the Search bar to find a specific color.

 Click the swatch to select it, then click the checkmark to close the Color Picker.

**Transition In Priority**

**0**, Pick or enter a number

This is the priority used when this camera is the destination for a transition.

**Transition In Time**

**0.2 Sec**, Pick or enter an amount

This is how long the transition lasts when this camera is the destination.

Fade In Hold Time**

0.0 s, Pick or enter an amount

This option becomes available when **Transition In Type** is set to **Fade**.

Determines the total tome in seconds for the fade-out effect, when using fade-type transitions.

**Transition In Type**

Linear, Ease-In, Ease-Out, **Ease-In-Out**, *Fade*

This determines what type of transition this camera uses when it is the destination camera.

**Transition Out Priority**

**0**, Pick or enter a number

This is the priority used when this camera transitions to another.

**Transition Out Time**

**0.2 Sec**, Pick or enter an amount

This is how long the transition lasts when this camera is the origin camera for a transition.

**Fade Out Hold Time**

**0.0 s**, Pick or enter an amount

This option becomes available when **Transition Out Type** is set to **Fade**.

Determines the total tome in seconds for the fade-in effect, when using fade-type transitions.

**Transition Out Type**

Linear, Ease-In, Ease-Out, **Ease-In-Out**, *Fade*

This determines what type of transition this camera uses when it is the origin camera for a transition.

**Look At Focus Target On Activate**

On, **Off**

If this is set to **On**, then when the camera activates it looks at the focus target override.

**Look at Target**

**No**, *Yes*

Determines whether the camera adjusts its Pitch or Yaw to frame the camera target.

**Look at Offset Distance**

**0**, Pick a distance

This option only displays if the **Look at Target** option is set to **On**.

Positions the camera view forward or backward (X axis) from the Look-at Target, instead of centered.

**Look at Offset Horizontal**

**0**, Pick a distance

This option only displays if the **Look at Target** option is set to **On**.

Positions the camera view left or right (Y axis) from the Look-at Target, instead of centered.

**Look at Offset Vertical**

**75 cm**, Pick a distance

This option only displays if the **Look at Target** option is set to **On**.

Positions the camera view upward or downward (Z axis) from the Look-at Target, instead of centered.

**Yaw Acceleration**

**6 degrees/second**, Pick or enter a number

This option only displays if the **Look at Target** option is set to **On**.

Determines the speed at which the camera moves leftward or rightward in order to frame the target. If this is set to **0**, the speed is instant.

**Yaw Max Speed**

**0 degrees/second**, Pick or enter a number

This option only displays if the **Look at Target** option is set to **On**.

Determines the maximum speed at which the camera moves left/right to frame the target. If you set this to **0**, there is no limit to the speed.

**Pitch Acceleration**

**6 degrees/second**, Pick or enter a number

This option only displays if the **Look at Target** option is set to **On**.

Determines the speed at which the camera moves upward/downward in order to frame the target. If this is set to **0**, the speed is instant.

**Pitch Max Speed**

**0 degrees/second**, Pick or enter a number

This option only displays if the **Look at Target** option is set to **On**.

Determines the maximum speed at which the camera moves up/down to frame the target. If you set this to **0**, there is no limit to the speed.

**Clamp**

**Off**, *On*

This option only displays if the **Look at Target** option is set to **On**.

If this is set to **On**, you can set limits for how far the camera can pitch and yaw. Four options related to Clamping display below this one.

**Clamp Pitch Min**

**-30 degrees**, Pick or enter a number

This option only displays if the **Clamp** option is set to **On**.

This determines the maximum distance the camera can rotate downward toward the target.

**Clamp Pitch Max**

**60 degrees**, Pick or enter a number

This option only displays if the **Clamp** option is set to **On**.

This determines the maximum distance the camera can rotate upward toward the target.

**Clamp Yaw Min**

**-45 degrees**, Pick or enter a number

This option only displays if the **Clamp** option is set to **On**.

This determines the maximum distance the camera can rotate leftward toward the target.

**Clamp Yaw Max**

**45 degrees**, Pick or enter a number

This option only displays if the **Clamp** option is set to **On**.

This determines the maximum distance the camera can rotate rightward toward the target.

**Deadzone**

*On*, **Off**

If you choose **On**, this establishes an area within which the target can move without affecting the camera.

When the target reaches the edge of the deadzone, the camera will move to follow the target. When set to **On**, four additional options displays below this one.

**Deadzone Yaw**

**10 degrees**, Pick or enter a number

This option only displays if the **Deadzone** option is set to **On**.

 The amount of space to the left and right within which the target can move before the camera needs to move left or right to follow the target.

**Deadzone Pitch**

**3 degrees**, Pick or enter a number

This option only displays if the **Deadzone** option is set to **On**.

 The amount of space up and down within which the target can move before the camera needs to move up or down to follow the target.

**Deadzone Yaw Offset**

**0 degrees**, Pick or enter a number

This option only displays if the **Deadzone** option is set to **On**.

 The amount of space to offset the deadzone left (use a negative number) or right (use a positive number).

**Deadzone Pitch Offset**

**0 degrees**, Pick or enter a number

This option only displays if the **Deadzone** option is set to **On**.

 The amount of space to offset the deadzone down (use a negative number) or up (use a positive number).

### Direct Event Binding

Following are the [direct event binding](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) options for this device.

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

Enables the camera when an event occurs.

##### Disable When Receiving From

Disables the camera when an event occurs.

##### Add to Player When Receiving From

Adds this camera to the instigating player when an event occurs.

##### Remove from Player When Receiving From

Removes this camera from the instigating player when an event occurs.

##### Add to All When Receiving From

Adds this camera to all players when an event occurs.

##### Remove from All When Receiving From

Removes this camera from all players when an event occurs.

##### Focus On Target When Receiving From

When an event occurs, this function sets the camera to focus on a target instead of focusing on the player.

##### Focus On Player When Receiving From

When an event occurs, this function sets the camera to focus on the player. This applies to all players.

#### Events

This device has no events.

### Use Fixed Point Camera In Verse

You can use the code below to control a Fixed Point Camera device in [Verse](https://dev.epicgames.com/documentation/en-us/uefn/learn-programming-with-verse-in-unreal-editor-for-fortnite). This code shows how to use events and functions in the Fixed Point Camera device API. Modify it to fit the needs of your experience.

using { /Fortnite.com/Devices }
using { /Verse.org/Simulation }
using { /UnrealEngine.com/Temporary/Diagnostics }
## A Verse-authored creative device that can be placed in a level
gameplay_camera_fixed_point_device_verse_example := class(creative_device):
 # Reference to the Gameplay Camera Fixed Point Device in the level.
 # In the Details panel for this Verse device,
 # set this property to your Gameplay Camera Fixed Point Device.
 @editable
 MyFixedPointCamera:gameplay_camera_fixed_point_device = gameplay_camera_fixed_point_device{}

Expand code Copy full snippet(22 lines long)

To use this code in your UEFN experience, follow these steps.

-
Drag a Fixed Point Camera device onto your island.

-
Create a new Verse device named **gameplay_camera_fixed_point_device_verse_example**. See [Create Your Own Device Using Verse](https://dev.epicgames.com/documentation/en-us/uefn/create-your-own-device-in-verse#creatinganewdevicewithverse) for steps.

-
In Visual Studio Code, open **gameplay_camera_fixed_point_device_verse_example.verse** in Visual Studio Code and paste the code above.

-
Compile your code and drag your Verse-authored device onto your island. See [Adding Your Verse Device to Your Level](https://dev.epicgames.com/documentation/en-us/uefn/create-your-own-device-in-verse#addingyourversedevicetoyourlevel) for steps.

-
Add a reference for the device on your island to your Verse device. See [Adding a Verse Reference to a Creative Device in Your Level](https://dev.epicgames.com/documentation/en-us/uefn/customize-verse-device-properties-in-verse#addingaversereferencetoacreativedeviceinyourlevel) for steps.

Disable the **Add to Players on Start** property of the Camera device so that only Verse will add the camera to the player.

-
Save your project and click **Launch Session** to playtest.

#### Fixed Point Camera API

See the [gameplay_camera_fixed_point_device API Reference](https://dev.epicgames.com/documentation/en-us/uefn/verse-api/fortnitedotcom/devices/gameplay_camera_fixed_point_device) for more information on using the device in Verse.

---

## Using Orbit Camera Devices in Fortnite Creative

**כותרת מקורית:** Using Orbit Camera Devices in Fortnite Creative  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/using-orbit-camera-devices-in-fortnite-creative  
**מקור קלט:** `07C_שחקנים_קבוצות_תפקידים_ומצלמות(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `using-orbit-camera-devices-in-fortnite-creative`

The **Camera: Orbit** (Orbit Camera) device provides a view that follows a target player character but that the player can rotate to freely look around.

This camera differs from a [****](https://dev.epicgames.com/documentation/fortnite/using-fixed-point-camera-devices-in-fortnite-creative)**[Fixed Point Camera](https://dev.epicgames.com/documentation/fortnite/using-fixed-point-camera-devices-in-fortnite-creative)** device, where the camera maintains a set location, and a [Fixed Angle Camera](https://dev.epicgames.com/documentation/fortnite/using-fixed-angle-camera-devices-in-fortnite-creative) device, where the camera moves in sync with the player at a locked angle that provides a consistent perspective. The orbit camera follows the player, but the player can still rotate the view to see in different directions without turning.

You can use a [Third Person Controls](https://dev.epicgames.com/documentation/fortnite/using-third-person-controls-devices-in-fortnite-creative) device with this camera, but it also works without it.

To learn more about how to use the camera and control devices together, see [Designing with Cameras and Controls](https://dev.epicgames.com/documentation/fortnite/designing-with-cameras-and-controls-in-fortnite-creative).

For help on finding the **Orbit Camera** device in Creative, see [Using Devices](https://dev.epicgames.com/documentation/fortnite/using-devices-in-fortnite). To find this device in UEFN, open the Content Drawer and click **Fortnite > Devices > !Beta**.

To learn about using cameras and controls devices in **UEFN**, see:

-
[****](https://dev.epicgames.com/documentation/en-us/uefn/gameplay-camera-and-control-devices-in-unreal-editor-for-fortnite)**[Gameplay Camera and Control Devices](https://dev.epicgames.com/documentation/fortnite/gameplay-camera-and-control-devices-in-unreal-editor-for-fortnite)** for general information.

-
[****](https://dev.epicgames.com/documentation/en-us/uefn/making-a-title-sequence-in-unreal-editor-for-fortnite)**[Making a Title Sequence](https://dev.epicgames.com/documentation/fortnite/making-a-title-sequence-in-unreal-editor-for-fortnite)** for a gameplay example using UEFN.

Looking for new ways to use the Orbit Camera in Creative? See our [Orbit Camera Design Example](https://dev.epicgames.com/documentation/fortnite/orbit-camera-device-design-example-in-fortnite-creative)!

### Camera Terms and Definitions

When building a game, cameras are used for lots of different purposes. There are some specialized terms used for these in-game cameras that you might be unfamiliar with. Many of these terms are used in the device options for this and other camera devices. The list below gives some of these terms and their definitions.

 Term Definition
**field of view**

The term **field of view** (or **FOV** for short) refers to what the camera can actually "see". The field of view is represented as an angle, and is measured in degrees. Angles have two sides, joined at a point called the **vertex**. With cameras, the vertex is the lens (virtual in this case) of the camera. The arms of the angle spread up and down (the vertical axis) from that vertex. The higher the number of degrees, the wider the angle, and the more the camera can see.

**pitch, yaw**

**Pitch** and **yaw** are terms originating in aviation. They refer to the different types of rotation a plane can perform when moving. These terms were adopted into 3D design and game development to more precisely define a virtual 3D environment and how things are positioned in that virtual space. Pitch and yaw are measured relative to the object's original position. **Pitch** refers to up and down movement of an object, and **yaw** refers to horizontal left or right movement of an object. **Note**: the **axis of rotation** is different from the direction of movement. For example, if a plane **pitches**, the nose of the plane moves up or down; but the plane is **rotating** on the Y-axis (which is the left-right or east-west horizontal axis). See the terms **X-axis**, **Y-axis**, and **Z-axis** in this table.

**angle pitch**

This is a measurement of how much the camera points up or down while framing its target.

**angle yaw**

This is a measurement of how much the camera turns left or right while framing its target.

**camera offset**

Normally the camera view centers on its target. The **camera offset** is how far from the center the camera view is. The camera can have an offset amount on the X-, Y-, or Z-axis and it can have an offset on more than one axis at a time.

**X-axis**

In a 3D space (real or virtual), the X-axis represents horizontal forward/backward (or north/south) movement.

**Y-axis**

In a 3D space (real or virtual), the Y-axis represents horizontal left/right (or east/west) movement.

**Z-axis**

In a 3D space (real or virtual), the Z-axis represents vertical up/down movement.

**camera transition**

When you have multiple cameras active, a **transition** is when you move from one camera view to another. In Fortnite, camera devices have an **In Priority** and an **Out Priority**. The camera transition is determined by the highest priority, comparing the Out Priority of the current camera with the In Priority of the destination camera.

**transition types**

**Ease In**: the camera transition will start slowly and speed up as it continues. **Ease Out**: the camera transition will slow down as it ends. **Ease In-Out**: the camera transition will start slowly, speed up, then slow again as it ends. **Linear**: the camera transition moves smoothly from one camera to another at the same speed. **Fade**: The camera will fade in from black and fade out to black.

**priority system**

If multiple cameras are assigned to a player, priority determines which camera is active at any point in time. Priority can be set in the device options. If two cameras are tied for the highest priority, the most recently added camera will become active.

**boom collision**

In film, a boom jib is an apparatus that holds the camera. Boom operators can move and orient the camera with levers and wheels to get the shot they desire. The Boom Collision properties for fixed angle cameras allow you to determine the behavior of that camera when an object in the scene gets between the camera and its target.

**deadzone**

The **deadzone** refers to an established area within which the target can move around without affecting the camera. When the target moves to an edge of the deadzone, the camera will move to follow the target.

**look-at location**

Where the camera is looking at any time. With the orbit camera, it might be something other than the player.

**soft deadzone**

The area inside of the deadzone where the camera starts to accelerate to follow the player. This area blends the look-at location between remaining stationary and following the target.

### Contextual Filtering

Some devices are affected by a feature called **contextual filtering**. This feature hides or displays options depending on the values selected for certain related options. This feature reduces clutter in the Customize panel and makes options easier to manage and navigate.

However, it may not be easy to recognize which options or values trigger contextual filtering. To help you identify them, we use *italic* in our device docs for any values that trigger contextual filtering. All options are listed, including those affected by contextual filtering; if they are hidden or displayed based on a specific option's value, there will be a note about that in the Description field for that option.

### Device Options

You can control the position of the camera relative to the target, the size and shape of the camera.

Configure this device with the following options.
**

Default values are **bold**. Values that trigger contextual filtering are *italic*.

 Option Value Description
**Creative Preview**

**Start**, Stop

Click **Start** to preview what the camera is seeing. Click **Stop** to leave the preview and go back to editing your island.

**Field of View**

**80**, Pick or enter a number of degrees from 20-120

This option only displays if the **Projection Mode** option is set to **Perspective**. The term **field of view** refers to what the camera can actually see. This setting determines the angle on the vertical axis, in degrees, that represents the Field of View for this camera. A higher number makes a wider angle, which results in a larger field of view.

**Camera Shake**

On, **Off**

If this is set to **On**, the camera will support screen shake events in the game.

**Priority**

**0**, Pick or enter a number

Determines where this camera falls in the priority system. When multiple cameras are added to a player, the camera with the highest priority is considered the active camera.

**Affects Team**

**Any**, Pick or enter a team

Determines which team is affected by this device.

The camera does not react dynamically to changes in team during the game. If your island allows players to change teams during the game, you might have to manually re-add cameras to those players after a team change.

**Affects Class**

No Class, **Any**, Pick or enter a class

Determines which classes are affected by this device. **No Class** means only players with no assigned class are affected. **Any** means all players, including those with no assigned class, are affected.

**Invert Team**

On, **Off**

If this is set to **On**, all teams are affected by this device except the team selected in the **Affects Team** option.

**Invert Class**

On, **Off**

If this is set to **On**, all classes are affected by this device except the class selected in the **Affects Class** option.

**Enabled During Phase**

None, **Always**, Pre-Game Only, Gameplay Only

Determines which phases the camera is active in. If you choose **None**, the camera can only be enabled manually using events.

**Remove on Elimination**

On, **Off**

Determines whether this camera is removed from a player when they are eliminated.

**Add to Players on Start**

**On**, Off

Determines whether this camera is automatically added to all players when the game starts.

Preview Device Color**

**#74ABFFFF**, Pick an color

Changes the device's color.

**Transition In Priority**

**0**, Pick or enter a number

This is the priority used when this camera is the destination for a transition.

**Transition In Time**

**0.2 sec**, Pick or enter an amount

This is how long the transition lasts when this camera is the destination.

**Fade in Hold Time**

**0.0s**, Pick or enter a time

Determines the total time in seconds for the fade-out effect, when using fade-type transitions.

**Transition In Type**

Linear, Ease-In, Ease-Out, **Ease-In-Out**, *Fade*

This determines what type of transition this camera uses when it is the destination camera.

**Transition Out Priority**

**0**, Pick or enter a number

This is the priority used when this camera transitions to another.

**Transition Out Time**

**0.2 sec**, Pick or enter an amount

This is how long the transition lasts when this camera is the origin camera for a transition.

**Fade Out Hold Time**

**0.0s**, Pick or enter a time

Determines the total time in seconds in seconds for the fade-in effect, when using fade-type transitions.

**Transition Out Type**

Linear, Ease-In, Ease-Out, **Ease-In-Out**, *Fade*

This determines what type of transition this camera uses when it is the origin camera for a transition.

**Look At Focus Target On Activate**

On, **Off**

If this is set to **On**, when the camera activates it looks at the focus target override that has been set for this camera.

**Hide Player Character**

On, **Off**

Sets the player character to be invisible but only for that player.

**Distance**

**100 cm**, Pick or enter a number

Determines the distance between the camera and the player.

**Offset X**

**0 cm**, Pick or enter a positive or negative number

This setting can move the view forward or backward, relative to the camera's position. A positive number moves the view forward, a negative number moves the view backward.

**Offset Y**

**50 cm**, Pick or enter a positive or negative number

Normally the camera view centers on its target. This setting can move the view left or right, relative to the camera's position. A positive number moves the view to the left, a negative number moves the view to the right.

**Offset Z**

**75 cm**, Pick or enter a positive or negative number

Normally the camera view centers on its target. This setting can move the view up or down, relative to the camera's position. A positive number moves the view down, a negative number moves the view up.

**Offset When Crouched**

On, **Off**

If this is set to **On**, the camera will be offset on the vertical axis when the player crouches.

**Horizontal Speed**

**10 cm/s**, Pick or enter a number

Determines the speed at which the camera moves in the X axis (forward/back) and Y axis (left/right) in order to frame the target.

**Vertical Speed**

**0 cm/s**, Pick or enter a number

Determines the speed at which the camera moves in the Z axis (up/down) to frame the target.

**Clamp Horizontal Rotation**

*On*, **Off**

This restricts (clamps) the range for camera rotation horizontally. When you set to **On**, the **Clamp Horizontal Rotation Min** and **Max** options show.

**Clamp Horizontal Rotation Min**

**-90 degrees**, Pick an angle

This option only displays if the **Clamp Horizontal Rotation** is set to **On**. Determines the minimum amount the camera can rotate in a negative horizontal direction.

**Clamp Horizontal Rotation Max**

**90 degrees**, Pick an angle

This option only displays if the **Clamp Horizontal Rotation** is set to **On**. Determines the maximum amount the camera can rotate in a positive horizontal direction.

**Clamp Horizontal Mode**

**Player Relative**, Device Relative, World Relative

Determines the basis for locking horizontal rotation when the camera is attached to a player.

**Clamp Vertical Rotation**

*On*, **Off**

Clamps the range for camera rotation vertically. When you set to **On**, the **Clamp Vertical Rotation Min** and **Max** options show.

**Clamp Vertical Rotation Min**

**-45 degrees**, Pick an angle

When **Clamp Horizontal Rotation** is set to **On**, you can use this option to set the minimum the camera can rotate in a negative vertical direction.

**Clamp Vertical Rotation Max**

**45 degrees**, Pick an angle

When **Clamp Horizontal Rotation** is set to **On**, you can use this option to set the maximum rotation in a positive vertical direction.

**Boom Collision**

***On***, Off

By default, boom collision is **On**. This means objects in the world that are between the camera and its target will hide the target. Additional options for boom collision show, and you can use them to set the behaviors that occur in relation to collision.

**Collision Type**

Instant, ***Predictive***, *Transparency*

This option only displays if the **Boom Collision** option is set to **On**. This determines what the camera does if objects in the world obscure the target. If this option is set to **Predictive**, two more options show below this one. If this option is set to **Transparency**, three more options show.

**Collision In Time**

**0.5 sec**, Pick or enter an amount

This option only displays if the **Collision Type** option is set to **Predictive**. Determines how fast the camera pulls in when using Predictive Collision.

**Collision Out Time**

**0.5 sec**, Pick or enter an amount

This option only displays if the **Collision Type** option is set to **Instant** or **Predictive**. Determines how fast the camera pulls out when using Predictive Collision.

**Transparency Collision Radius**

**5.0 cm**, Pick or enter an amount

The radius from the camera's path to its target. This is used to identify which objects to make transparent.

**Transparency Amount**

**0.4**, Pick an amount

This option only displays if the **Collision Type** option is set to **Transparency**. Determines how opaque objects are when they break the line of sight of your character. **0** means they are totally transparent; **1** means they are totally opaque.

**Transparency Cutout Radius**

**100cm**, Pick or enter an amount

This option only displays if the **Collision Type** option is set to **Transparency**. Determines an area of full transparency around the camera target when a boom collision has occurred.

**Deadzone**

*On*, **Off**

If you choose **On**, this establishes an area in which the target can move without affecting the camera position. When the target reaches the edge of the deadzone, the camera moves to follow the target.

**Deadzone Type**

*Sphere*, ***Cylinder***, *Rectangle*

This option only shows if the **Deadzone** option is set to **On**, and determines the shape of the deadzone.

**Deadzone Height**

**0 cm**, Pick or enter an amount

This option displays if the **Deadzone Type** option is set to **Cylinder** or **Rectangle**, and determines the height of the deadzone.

**Deadzone Diameter**

**200 cm**, Pick or enter an amount

This option displays if the **Deadzone Type** option is set to **Sphere** or **Cylinder**.

**Deadzone Width**

**100 cm**, Pick or enter an amount

This option only displays if the **Deadzone Type** option is set to **Rectangle**. It determines the width of the deadzone.

**Deadzone Depth**

**100 cm**, Pick or enter an amount

This option only displays if the **Deadzone Type** option is set to **Rectangle**. Determines the depth of the deadzone.

**Deadzone Soft Percent**

**100\%**, Pick or enter a percentage

Determines an area within the deadzone where the camera blends between remaining stationary and following the player.

**Deadzone Jump Size**

**Off**, Pick or enter a size

If you specify a size, it determines the area within which a player can jump up and down without the camera following them.

**Auto Rotate When Moving**

*On*, **Off**

If this is set to **On**, the camera will automatically rotate to its default position when the player is moving.

**Auto Rotate Moving Yaw Speed**

**4°/S**, Pick or enter an amount

This option only displays if the **Auto Rotate When Moving** option is set to **On**. Determines the speed (in degrees per second) to rotate the camera ray while the player is moving.

**Auto Rotate Moving Pitch Speed**

**10°/S**, Pick or enter an amount

This option only displays if the **Auto Rotate When Moving** option is set to **On**. Determines the speed (in degrees per second) to rotate the camera pitch while the player is moving.

**Auto Rotate Moving Delay**

**0.75**, Pick or enter an amount of time

This option only displays if the **Auto Rotate When Moving** option is set to **On**. Determines how much time it takes before the device activates auto-rotation while moving.

**Auto Rotate Terrain Offset Enabled**

*On*, **Off**

This option only displays if the **Auto Rotate When Moving** option is set to **On**. If this is set to **On**, the camera automatically adjusts its pitch up and down based upon the slope of the terrain the player is traveling on.

**Auto Rotate Terrain Offset Max**

**15.0**, Pick or enter an amount

This option only displays if the **Auto Rotate Terrain Offset Enabled** option is set to **On**. Determines the maximum amount of offset that can affect the camera's pitch.

**Auto Rotate Terrain Offset Sensitivity**

**60**, Pick or enter an amount

This option only displays if the **Auto Rotate Terrain Offset Enabled** option is set to **On**. Determines how often the camera checks the elevation. The higher this value is, the more reactive to changing terrain the auto-rotation will be.

**Show Dead Zone in Preview**

On, **Off**

If this is set to **On**, the deadzone will be visible when previewing this camera.

### Direct Event Binding

Following are the [direct event binding](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) options for this device.

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

Enables the camera when an event occurs.

##### Disable When Receiving From

Disables the camera when an event occurs.

##### Add to Player When Receiving From

Adds this camera to the instigating player when an event occurs.

##### Remove from Player When Receiving From

Removes this camera from the instigating player when an event occurs.

##### Add to All When Receiving From

Adds this camera to all players when an event occurs.

##### Remove from All When Receiving From

Removes this camera from all players when an event occurs.

##### Focus On Target When Receiving From

When an event occurs, this function sets the camera to focus on a target instead of focusing on the player.

##### Focus On Player When Receiving From

When an event occurs, this function sets the camera to focus on the player. This applies to all players.

#### Events

This device has no events.

### Use The Orbit Camera In Verse

You can use the code below to control an Orbit Camera device with Verse. This code shows how to use events and functions in the Orbit Camera device API. Modify it to fit the needs of your experience.

using { /Fortnite.com/Devices }
using { /Verse.org/Simulation }
using { /UnrealEngine.com/Temporary/Diagnostics }

## A Verse-authored creative device that can be placed in a level
gameplay_camera_fixed_angle_device_verse_example := class(creative_device):
 # Reference to the Gameplay Camera Fixed Angle Device in the level.
 # In the Details panel for this Verse device,
 # set this property to your Gameplay Camera Fixed Angle Device.
 @editable

Expand code Copy full snippet(23 lines long)

To use this code in your UEFN experience, follow these steps.

-
Drag an Orbit Camera device onto your island.

-
Create a new Verse device named **gameplay_camera_orbit_device_verse_example**. See [Create Your Own Device Using Verse](https://dev.epicgames.com/documentation/fortnite/create-your-own-device-using-verse-in-unreal-editor-for-fortnite) for steps.

-
In Visual Studio Code, open **gameplay_camera_orbit_device_verse_example.verse** and paste the code provided above.

-
Compile your code and drag your Verse-authored device onto your island. See [Adding Your Verse Device to Your Level](https://dev.epicgames.com/documentation/fortnite/create-your-own-device-using-verse-in-unreal-editor-for-fortnite#adding-your-verse-device-to-your-level) for steps.

-
Add a reference for the Orbit Camera device on your island to your Verse device. See [Adding a Verse Reference to a Creative Device in Your Level](https://dev.epicgames.com/documentation/fortnite/editable-properties-in-verse) for steps.

Set the **Add to Players on Start** property of the Orbit Camera device, so that only Verse will add the camera to the player.

-
Save your project and click **Launch Session** to playtest.

#### Orbit Camera API

See the [gameplay_camera_orbit_device API Reference](https://dev.epicgames.com/documentation/en-us/uefn/verse-api/fortnitedotcom/devices/gameplay_camera_orbit_device) for more information on using the Orbit Camera device in Verse.

---

## Using Player Checkpoint Devices in Fortnite Creative

**כותרת מקורית:** Using Player Checkpoint Devices in Fortnite Creative  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/using-player-checkpoint-devices-in-fortnite-creative  
**מקור קלט:** `07C_שחקנים_קבוצות_תפקידים_ומצלמות(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `using-player-checkpoint-devices-in-fortnite-creative`

The **Player Checkpoint Pad** sets a player's spawn point when activated and can also be used to clear player inventories.

 For help on how to find the Player Checkpoint device, see [](https://dev.epicgames.com/documentation/assets/using-devices-in-fortnite-creative)[Using Devices](https://dev.epicgames.com/documentation/fortnite/using-devices-in-fortnite).

### Device Options

This device has some basic functionality, like playing sound effects and resetting inventories.
**

The default values are bold.

You can configure this device with the following options.

**אפשרויות, ערכים ותיאורים:**

##### Visible in Game**

- **Value / Values:** **On**, Off
- **Description:** Determines whether the device is visible during the game. This does affect its collision properties.

##### Reset Inventory

- **Value / Values:** Yes, No
- **Description:** Determines whether the player's inventory is reset when they activate the checkpoint.

##### Enabled During Phase

- **Value / Values:** None, **All**, Create Only, Game Countdown Only, Gameplay Only
- **Description:** Determines the game phases during which the device will be enabled.

##### Activating Team

- **Value / Values:** **Any**, Pick a team
- **Description:** Determines which team can activate the device.

##### Play Activate FX

- **Value / Values:** **On**, Off
- **Description:** Determines whether the device plays VFX and SFX when stepped on.

##### Allowed Class

- **Value / Values:** No Class, **Any**, Pick a class
- **Description:** Determines which class can activate the device.

### Direct Event Binding

#### Functions

A [function](https://dev.epicgames.com/documentation/en-us/fortnite-creative/fortnite-creative-glossary#function) listens for an event on a device then performs an action.

-
For any function, click the option, then **Select Device** to access and select from the **Device** dropdown menu.

-
Once you've selected a device, click **Select Event** to bind the device to an event that will trigger the function.

-
If more than one device or event triggers a function, click the **Add** button to add a line and repeat these steps.

**אפשרויות ותיאורים:**

##### Enable When Receiving From

Enables the device when an event occurs.

##### Disable When Receiving From

Disables the device when an event occurs.

##### Activate When Receiving From

Registers this checkpoint to the activating player when an event occurs.

#### Events

An [event](https://dev.epicgames.com/documentation/en-us/fortnite-creative/fortnite-creative-glossary#event) tells another device when to perform a function.

-
For any event, click the option, then **Select Device** to access and select from the **Device** dropdown menu.

-
Once you've selected a device, click **Select Function** to bind this event to a function for that device.

-
If more than one function is triggered by the event, click the **Add** button to add a line and repeat these steps.

**אפשרויות ותיאורים:**

##### On First Activation Per Player Transmit On

Sends an event each time a new player activates the checkpoint for the first time.

##### On First Activation Transmit On

Sends an event the first time the checkpoint is activated by any player.

---

## Using Player Marker Devices in Fortnite Creative

**כותרת מקורית:** Using Player Marker Devices in Fortnite Creative  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/using-player-marker-devices-in-fortnite-creative  
**מקור קלט:** `07C_שחקנים_קבוצות_תפקידים_ומצלמות(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `using-player-marker-devices-in-fortnite-creative`

**Player Marker** devices show players' positions on the [minimap](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#minimap), and you can choose what other information displays for marked players. Here are some examples:

-
[Health](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#health-bar) and [shield](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#shield) bars of marked players

-
Distance to a marked player

You can also change the appearance of the visual marker:

-
Determine whether the marker appears on the minimap.

-
Create a customized text label to display on marked players.

-
Choose an icon and the icon's color.

To find the Player Marker device, see [****](https://dev.epicgames.com/documentation/fortnite/using-devices-in-fortnite-creative)**[Using Devices](https://dev.epicgames.com/documentation/fortnite/using-devices-in-fortnite)**.

If you're using multiple copies of a device on an island, it can be helpful to [rename](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#rename-a-device) them. Choosing names that relate to a device's purpose makes it easier to remember what each one does, and easier to find a specific device when using the [Event Browser](https://dev.epicgames.com/documentation/fortnite/event-browser-in-fortnite-creative).

### Contextual Filtering

Some devices are affected by a feature called **contextual filtering**. This feature hides or displays options depending on the values selected for certain related options. This reduces clutter in the Customize panel and makes options easier to manage and navigate. To help identify them, values that trigger contextual filtering are in *italic*.

All options are listed, including those affected by contextual filtering; if they are hidden or displayed based on a specific option's value, there will be a note about it in the Description field for that option.

### Device Options

This device has some basic functionality, like auto saving and saving checkpoint data. Additionally, there are some advanced options, like saving a player's shield and health data.

You can configure this device with the following options.

Default values are **bold**. Values that trigger contextual filtering are *italic*.

**אפשרויות, ערכים ותיאורים:**

##### Show Marker

- **Value / Values:** ***Yes***, No
- **Description:** Determines whether the marker is visible or not. If the **Position Update Frequency** is set to **Always**, the marker is only visible if the Nameplate is also visible.

##### Beacon Style

- **Value / Values:** Hidden, ***Show (Direct Color)***, Show (Team Color)
- **Description:** This option is only displayed if the **Show Marker** option is set to **Yes**. Determines if the beacon is hidden, and whether a shown marker uses a custom defined color or whether it inherits the marked player's team color.

##### Beacon Primary Color

- **Value / Values:** **Sky Blue**, Pick a color
- **Description:** This option only displays if the **Beacon Style** option is set to **Show (Direct Color)**. Determines the primary color of the marker icon. Click the color swatch to open the Color Picker. You can scroll to select a color swatch, or you can use the Search bar at the top. Select the color swatch you want, then click the checkmark to select.

##### Beacon Secondary Color

- **Value / Values:** **#C88BFF**, Pick a color
- **Description:** This option only displays if the **Beacon Style** option is set to **Show (Direct Color)**. Determines the color of the marker icon. Click the color swatch to open the Color Picker. The hexadecimal code for the color is displayed next to the color swatch. You can scroll to select a color swatch, or you can type a hexadecimal code in the Search bar at the top and click the **Search** button. Select the color swatch you want, then click the checkmark to select.

##### Show Icon

- **Value / Values:** **None**, Pick an icon
- **Description:** Determines the icon used for the marker. Click the icon to open the **Icon Library Picker**. You can scroll through the icons to find one, or you can type a word into the Search bar at the top and click the **Search** button. Select an icon, then click the checkmark.

##### Icon Color

- **Value / Values:** **White**, Pick a color
- **Description:** Determines the color of the marker icon. You can scroll to select a color swatch, or you can use the Search bar at the top. Select the color swatch you want, then click the checkmark to select.

##### Show Marker Distance

- **Value / Values:** Yes, **No**
- **Description:** Determines if the distance to the player should be shown or not.

##### Show On Map

- **Value / Values:** **None**, Map and Minimap
- **Description:** Determines whether the marker is shown on the map and minimap.

##### Show Health Bar And Shield Bar

- **Value / Values:** **None**, Both, Only Health, Only Shield
- **Description:** Determines whether the health and shield bar of the tracked player are shown on the marker.

##### Marker Text

- **Value / Values:** **Custom Text Here**, Enter text
- **Description:** Choose the text that is shown on the marker. The text field is limited to 24 characters.

##### Visible For Class

- **Value / Values:** **Any**, No Class, Pick or enter a class
- **Description:** Determines which class can see the marker. If you choose **No Class**, only players without an assigned class can see the marker.

##### Invert Visible Class

- **Value / Values:** On, **Off**
- **Description:** If this is set to **On**, the class selected in the **Visible For Class** is the only class which cannot see the marker.

##### Visible For Team

- **Value / Values:** **Any**, Pick or enter a team
- **Description:** Determines which team can see the marker.

##### Invert Visible Team

- **Value / Values:** On, **Off**
- **Description:** If this is set to **On**, the team selected in the **Visible For Team** is the only team which cannot see the marker.

##### Position Update Frequency

- **Value / Values:** ***Constant***, Pick or enter an amount
- **Description:** Determines the frequency, in seconds, at which the marker's position is updated.

##### Hide Nearby Marker

- **Value / Values:** *On*, **Off**
- **Description:** Determines if a nearby marker is hidden or not. If you choose **On**, an additional option displays below this one.

##### Hide Nearby Marker Distance

- **Value / Values:** **5 Meters**, Pick or enter a number
- **Description:** This option only displays if the **Hide Nearby Marker** option is set to **On**. Determines the distance at which the beacon is hidden from a player.

##### Hide Distant Marker

- **Value / Values:** *On*, **Off**
- **Description:** If the player is farther away than the chosen distance, the marker isn't visible.

##### Hide Distant Marker Distance

- **Value / Values:** **50 Meters**, Pick or enter a number
- **Description:** This option only displays if the **Hide Distant Marker** option is set to **On**. The beacon is hidden when the player is farther away than the set distance.

##### Marker Line Of Sight

- **Value / Values:** **Always Show**, Hide Behind Obstacle
- **Description:** If you choose **Hide Behind Obstacle**, the marker is invisible if an obstacle blocks the player's line of sight.

##### Marker Focus Angle

- **Value / Values:** **Always Visible**, Pick an angle amount
- **Description:** Determines the angle from the player's direction of view for which the marker is still visible.

##### Applied to Class At Game Start

- **Value / Values:** No Class, **Any**, Pick or enter a class
- **Description:** All players of the selected class are given a marker at the start of the game.

##### Invert Applied to Class At Game Start

- **Value / Values:** **On**, Off
- **Description:** If this is set to **On**, a marker is added to all players who do NOT have the class selected in the **Applied to Class At Game Start** option.

##### Applied to Team At Game Start

- **Value / Values:** **All**, Pick or enter a team
- **Description:** All players on the selected team are given a marker at the start of the game.

##### Invert Applied to Team At Game Start

- **Value / Values:** **On**, Off
- **Description:** If this is set to **On**, a marker is added to all players who are NOT on the team selected in **Applied to Team at Game Start** option.

##### First Item Trigger Condition

- **Value / Values:** **Do Not Compare**, *Fewer Than*, *Equal or Fewer*, *Not Equal To*, *Equal To*, *Equal or More*, *More Than*
- **Description:** If you select a value other than **Don't Compare**, the **First Item Target Value** option displays. Determines if the trigger condition is the player having less, more, or equal to.

##### First Item Target Value

- **Value / Values:** **0**, Pick or enter a number
- **Description:** Determines the target value for the first tracked item.

##### Second Item Trigger Condition

- **Value / Values:** **Do Not Compare**, *Fewer Than*, *Equal or Fewer*, *Not Equal To*, *Equal To*, *Equal or More*, *More Than*
- **Description:** If you select a value other than **Don't Compare**, the **Second Item Target Value** option displays. Determines if the trigger condition is the player having less, more, or equal to.

##### Second Item Target Value

- **Value / Values:** **0**, Pick or enter a number
- **Description:** Determines the target value for the second tracked item.

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

##### Attach to Player When Receiving From

This function attaches a marker to a player when an event occurs.

##### Detach from Player When Receiving From

This function detaches a marker from a player when an event occurs.

##### Detach from All When Receiving From

This function detaches markers from all players when an event occurs.

##### Enable When Receiving From

This function enables the device when an event occurs.

##### Disable When Receiving From

This function disables the device when an event occurs.

#### Events

Direct event binding uses events as transmitters. An event tells another device to perform a function.

-
For any event option, click the **option**, then **Select Device** to access and select from the **Device dropdown menu**.

-
Once you've selected a device, click **Select Function** to bind the event to a function for that device.

-
If more than one function is triggered by the event, press the **Add** button and repeat.

**אפשרויות ותיאורים:**

##### On First Tracker Item Changed Send Event To

When the amount of the first item changes, an event is sent to the selected device, triggering the selected function.

##### On Second Tracker Item Changed Send Event To

When the amount of the second item changes, an event is sent to the selected device, triggering the selected function.

##### On First Item Value Reached Send Event To

When the first item reaches the target value, an event is sent to the selected device, triggering the selected function.

##### On Second Item Value Reached Send Event To

When the second item reaches the target value, an event is sent to the selected device, triggering the selected function.

---

## Using Player Movement Devices

**כותרת מקורית:** Using Player Movement Devices  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/using-player-movement-devices  
**מקור קלט:** `07C_שחקנים_קבוצות_תפקידים_ומצלמות(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `using-player-movement-devices`

**

This feature is in an experimental state so you can try it out, provide feedback, and see what we are planning. Please keep in mind that we do not guarantee backward compatibility for islands using the device during the experimental stage, the APIs for these features are subject to change, and we may remove entire experimental features or specific functionality at our discretion.

The Player Movement** device manages different types of movement through movement attributes. The customized movement determines how players move beyond what is controlled through **Island Settings. **This, in turn, adds a level of control to the island that creates a unique feeling to the in-game experience and supports different game genres.

The Player Movement device does not:

-
Customize the player input or relevant animations.

-
Override specific movement configurations to a certain gameplay item or vehicle.

Only one Player Movement Settings device can be actively used on one player at a time.

You can easily preview the movement changes within **[Edit mode](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#edit-mode)** so there’s no need to playtest the result. Previewing customized player movement settings in Edit mode can restrain your movements while editing. For example, actions like toggling **Fly** will be affected by any edits made to flight specific settings.
**
Use this device to:

-
Create gameplay movements similar to Fortnite Ballistic with the use of the [First Person camera devices](https://dev.epicgames.com/documentation/fortnite/using-first-person-camera-devices-in-fortnite-creative).

-
Create gameplay movement that complements the [Fixed Angle Camera](https://dev.epicgames.com/documentation/fortnite/fixed-angle-camera) and [Fixed Point Camera](https://dev.epicgames.com/documentation/fortnite/fixed-point-camera).

To find the Player Movement** device,

go to the **Creative menu** and select the **Devices **category. From there you can search or browse for the device. For more information on finding devices see [Using Devices](https://dev.epicgames.com/documentation/fortnite/using-devices-in-fortnite).
**

If you're using multiple copies of a device on an island, it can be useful to [rename](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#rename-a-device) them. Choosing names that relate to a device's purpose makes it easier to remember what each one does, and easier to find a specific device when using the [Event Browser](https://dev.epicgames.com/documentation/fortnite/event-browser-in-fortnite-creative).**

### Contextual Filtering

Some devices are affected by a feature called **contextual filtering**. This feature hides or displays options depending on the values selected for certain related options. This reduces clutter in the Customize panel and makes options easier to manage and navigate. To help identify them, values that trigger contextual filtering are in italic.

All options are listed, including those affected by contextual filtering; if they are hidden or displayed based on a specific option's value, there will be a note about it in the Description field for that option.

### Device Options

All movements can be customized individually or together based on Fortnite BR Classic movement styles and Fortnite Ballistice movement styles. Individual movements have broad customization options.
**

Default values are bold**. Values that trigger contextual filtering are *italic*.

You can configure this device with the following options.

 Option Values Description
**Creative Preview**

**Start**

Enables a preview of the movement settings in Live Edit.

**Priority**

**0**, Select a value

Determines which device is active, multiple devices can be present at any time, but only the one with the highest priority is considered active.

**Add to Players on Start**

**On**, Off

Determines whether the movement settings are applied to valid player characters at start of game.

**Enabled During Phase**

None, **Always**, Pre-Game Only, Gameplay Only

Determines at which phase the device is enabled.

**Movement Setting Preset**

**Current BR**, Current Ballistic

Determines which preset the device is applying to the movement settings of the player characters.

**Selected Team**

**Any**, Select a Team

Determines which teams can be affected by the device.

**Invert Team Selection**

On, **Off**

When this option is set to Off, only the selected team is affected by the device's customized movement options.

If this option is set to On, all teams except the selected team are affected by the device's customized movement options.

**Selected Class**

**Any**, Select a Class

Determines which classes can be affected by the device.

**Invert Class Selection**

On, **Off**

If Off, only the selected class is affected by the device. If On, all classes except the selected class are affected by the device.

**Category Filter**

**All**, *General, Walking, Jumping, Sprinting, Crouching, Sliding, Swimming, Gliding, Skydiving, DBNO, Mantling, Hurdling, Boost Jumping, Energy*

Filters the option list down to just the selected category of movement options.

Selecting any option other than **All** or **General** makes additional options available, or removes options that don't apply.

**Maximum Acceleration**

**Don’t Override**, select an acceleration amount

Sets the maximum acceleration, which is the rate of change of velocity.

This acceleration will be applied to any movement mode unless being overridden by the mode specifically.

**Braking Friction Factor**

**Don’t Override**, select an amount

Factor used to multiply actual value of friction used when braking.

This factor will be used to multiply the values specified for each game mode.

**Reloading Speed Multiplier**

**Don’t Override**, select a speed

Default multiplier to apply to the player’s speed if they are reloading.

This multiplier can be applied differently to each individual movement mode.

**Shooting Speed Multiplier**

**Don’t Override**, select a speed

Default multiplier to apply to the player’s speed if they are shooting.

This multiplier can be applied to each individual movement mode.

**Ground Friction**

**Don’t Override**, Select an amount

This setting affects movement control. Higher values allow faster changes in direction.

**Walk Maximum Speed**

**Don’t Override**, Select a speed

The maximum ground speed when walking.

**Jump Maximum Time**

**Don’t Override**, select a time

This option only becomes available when the **Category Filter** option is set to **Jumping**.

Maximum time the player is allowed to hold the jump button so the character can jump in the air.

**Jump Velocity**

**Don’t Override**, select a velocity

Initial velocity (instantaneous vertical acceleration) when jumping.

**Air Control**

**Don’t Override**, select an amount

Determines the amount of lateral movement control available to the character when falling.

-
0 = no control

-
1 = full control at max walk speed

**Crouch Maximum Walk Speed**

**Don’t Override**, select a speed

This option only becomes available when the **Category Filter** option is set to **Crouching**.

The maximum ground speed when walking and crouched.

**Allow Sprinting**

**Don’t Override**, *Yes*, No

Determines whether the associated player character can sprint.

Selecting **Yes **surfaces more **Sprinting **options.

**Sprint Maximum Speed**

**Don’t Override**, select a speed

The maximum ground speed when sprinting.

**Tactical Sprint Speed Multiplier**

**Don’t Override**, select a multiplier amount

This option only becomes available when **Allow Sprinting** is set to **Yes**.

Minimal speed multiplier to the maximum sprint speed when the tactical sprint reaches its highest speed.

**Tactical Sprint Jump Multiplier**

**Don’t Override**, select a multiplier amount

This option only becomes available when **Allow Sprinting** is set to **Yes**.

Maximum multiplier to the default Jump Velocity when the tactical sprint reaches its highest speed.

**Energy Cost on Sprinting**

**Don’t Override**, Select an amount

Determines how much **Energy **is drained per second while sprinting.

**DBNO Maximum Speed**

**Don’t Override**, select a speed

DBNO crawl speed for the character.

**Allow Hurdling**

**Don’t Override**, *Yes*, No

Whether hurdling is allowed.

**Allow Hurdling Over Jumpable Objects**

**Don’t Override**, *On*, Off

This option only becomes available when **Allow Hurdling** is set to **Yes**.

Determines whether players can hurdle over low obstacles that already can be jumped.

**Auto Hurdling**

**Don’t Override**, Yes, No

This option only becomes available when **Allow Hurdling** is set to **Yes**.

Determines whether the player character will automatically hurdle.

**Allow Mantling**

**Don’t Override**, *Yes*, No

Whether or not mantling is allowed.

**Mantling Minimal Ledge Height**

**Don’t Override**, select a height

This option only becomes available when **Allow Mantling** is set to **Yes**.

Determines the minimum height from the ground for a ledge to be a valid mantling location.

**Mantling Minimal Ledge Height in Water**

**Don’t Override**, select a height

This option only becomes available when **Allow Mantling** is set to **Yes**.

Determines the minimum height from the ground for a ledge to be a valid mantling location in water.

**Allow Sliding**

**Don’t Override**, *Yes*, No

Determines whether the associated player character can slide.

Selecting **Yes **surfaces more **Sliding** options.

**Sliding Maximum Forward Speed**

**Don’t Override**, select a speed

This option only becomes available when **Allow Sliding** is set to **Yes**.

The maximum speed in forward movement that can be reached while sliding.

**Sliding Dash Duration**

**Don’t Override**, select a duration

This option only becomes available when **Allow Sliding** is set to **Yes**.

The maximum dash duration for sliding.

**Allow Boosted Jumping**

**Don’t Override**, *Yes*, No

Whether boosted jumping is allowed.

**Allow Boosted Jumping**

**Don’t Override**, *Yes*, No

This option only becomes available when the **Category Filter** option is set to **Boosted Jumping**.

Whether boosted jumping is allowedt.

**Boosted Jump Vertical Velocity**

**Don’t Override**, select a velocity

This option only becomes available when **Allow Boost Jumping** is set to **Yes**.

Determines the maximum vertical velocity while in the **Boost Jumping** mode.

**Boosted Jump Horizontal Velocity**

**Don’t Override**, select a velocity

This option only becomes available when **Allow Boost Jumping** is set to **Yes**.

Determines the horizontal jump velocity while in **Boost Jumping** mode.

**Energy Cost on Jumping**

**Don’t Override**, Select an amount

Determines how much **Energy **is drained while jumping.

**Swimming Maximum Acceleration**

**Don’t Override**, select an acceleration amount

Max acceleration for the swimming mode, which is the rate of change of velocity.

**Swimming Maximum Speed**

**Don’t Override**, select a speed

The maximum normal speed when swimming.

**Swimming Maximum Sprinting Speed**

**Don’t Override**, select a speed

The maximum sprinting speed when Swimming.

**Skydiving Maximum Acceleration**

**Don’t Override**, select a speed

Max horizontal acceleration. Diminished when diving down in **Skydiving **mode.

**Skydiving Lateral Friction**

**Don’t Override**, select an amount

Determines how floaty or snappy the change in lateral direction is in **Skydiving **mode.

**Skydiving Maximum Latera Speed**

**Don’t Override**, select a speed

Max lateral speed. Diminished when diving down in **Skydiving **mode.

**Gliding Lateral Friction**

**Don’t Override**, select an amount

Determines how floaty or snappy changing lateral direction is in **Gliding **mode.

**Gliding Maximum Lateral Speed**

**Don’t Override**, select a speed

Max lateral speed. Diminished when diving down in **Gliding **mode.

**Gliding Terminal Velocity**

**Don’t Override**, select a speed

Max vertical velocity when falling down. Ignored if set to 0.

**Energy Max**

**Don’t Override**, Select an amount

Determines how much Energy is available. This affects **Sprint** and other abilities that use Energy.

**Energy Recharge Delay**

**Don’t Override**, Select an amount

Determines how long of a delay there is after players have stopped using Energy before it recharges.

**Energy Recharge Per Second**

**Don’t Override**, Select an amount

Determines how much Energy is recharged per second after **Energy Recharge Delay** occurs.

**Pause Energy Cost on Falling**

**Don’t Override**, On, Off

Determines whether energy consumption should be paused during a player’s fall.

**Stop Energy Regen on Paused**

**Don’t Override**, On, Off

Determines whether energy recharge should be stopped when the energy consumption is paused (on falling or sliding).

### Direct Event Binding

Following are the [direct event binding](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#direct-event-binding) options for this device.

#### Functions

A [function](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#function) listens for an event on a device then performs an action.

1. For any function, click the **option**, then **Select Device** to access and select from the **Device** dropdown menu.

2. Once you've selected a device, click **Select Event** to bind the device to an event that will trigger the function for the device.

3. If more than one device or event triggers a function, click the **Add** button to add a line and repeat these steps.

 Option Description
**Enable When Receiving From**

Enables the device.

**Disable When Receiving From**

Disables the device.

**Add to Player When Receiving From**

Adds the movement settings to the instigating Player, activating if the highest priority.

**Add to All Players When Receiving From**

Adds the movement settings to all the Players, activating if the highest priority.

**Remove from Player When Receiving From**

Removes the movement settings from the Instigating Player.

**Remove from All Players When Receiving From**

Removes the movement settings from all the Players.

This device has no events.

---

## Using Player Reference Devices in Fortnite Creative

**כותרת מקורית:** Using Player Reference Devices in Fortnite Creative  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/using-player-reference-devices-in-fortnite-creative  
**מקור קלט:** `07C_שחקנים_קבוצות_תפקידים_ומצלמות(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `using-player-reference-devices-in-fortnite-creative`

You can use the **Player Reference** device to relay player statistics to other devices and even to other players. Statistics such as the number of enemies the player has eliminated, the number of times the player is eliminated, or the player's scores can be transmitted by the device when certain conditions are met. The Player Reference can also project a hologram of the player and display text that can be altered in various positions and curvatures.

 For help on how to find the Vault device, see [Using Devices](https://dev.epicgames.com/documentation/fortnite/using-devices-in-fortnite).

 If you're using multiple copies of a device on an island, it can be useful to [rename](https://dev.epicgames.com/documentation/en-us/fortnite-creative/rename-a-device) them. Choosing names that relate to a device's purpose makes it easier to remember what each one does, and easier to find a specific device when using the [Event Browser](https://dev.epicgames.com/documentation/fortnite/event-browser-in-fortnite-creative).

### Device Options

This device has some basic functionality and can be customized to change the hologram animation and select which channel the device will register and clear data on.

You can configure this device with the following options.

Default values are **bold**.

#### Device Options

 Option Value Description
**Show Hologram**

**On**, Off

Determines if the hologram of the player's character will be shown in game. Only valid if the **Visible in Game** option is set to **On**.

**Color**

***Direct Color***, Team Color, Team Relationship Color

Determines the color of the displayed text. If you choose **Team Relationship**, the text is red if it's hostile to your team, green if it's neutral, and blue if it's friendly.

**Custom Color**

**White**, Select a color

Sets a custom color for the hologram and player details.

**Visible in Game**

***On***, Off

Determines if the device is visible during the game. This affects the device's collision properties.

**Show Player Details**

On, **Off**

Determines where to display the player's details on the device and the position it displays in. Only valid if the **Visible in Game** option is set to **On**.

Hologram Animation

Idle, Hands on Hips, Flex

Determines the animation that the hologram will play. Only valid if the Show Hologram and Visible in Game options set to On.

**Hologram Effect Strength**

Off, **100%**, Pick a percentage

Determines the brightness of the Hologram Effect. Only valid if the **Visible in Game** option is set to **On**.

**Show Base**

**On**, Off

Determines whether the device is visible during the game. This will always show during creation if everything else is disabled.

**Stat to Track**

**None**, Eliminations, Score, Eliminated

Determines which stats display if the **Show Player Details** option is not set to **Off**. This is also used to determine when the **Track Stat Changed** transmitter option triggers.

**Player Details Height**

**115CM**, Pick or enter a number

Determines if the player's details are displayed on the device and how high they are shown. This option is only valid if **Visible During Game** and **Shown Player Details** are both set to **On**.

**Player Details Curve Amount**

No Curve, Small Curve, Medium Curve, **Large Curve**

Determines the curvature degree that the player details will display.

**Track Game Total for Stats**

On, **No**

Selects if the tracking stats will come from the game total rather than the current round’s value.

**Update Registered Player**

**Always**, When No Registered Player, If Stat Is Higher, If Stat Is Higher Or Equal, If Stat Equal, If Stat Not Equal, If Stat Equal Or Lower, If Stat Is Lower

If there is a registered player, and the device receives a request to register a new player, this option determines if that update is successful. If there is no registered player, the update is always successful.

**Activated by Sequencers**

**On**, Off

Determines whether or not to activate the device when it is touched by a Sequencer or RNG Device pulse.

**Registered by Sequencers**

**On**, Off

Determines if this device uses the activating player of the Sequencer or the RNG Device as the registered instigator.

**Allow Activate without Player Reference**

Yes, **No**

Determines if the signal will be transmitted if you send an Activate signal without a player being locked into the device.

Several devices will only function with a valid instigator.

**Play Audio**

**Yes**, No

Determines if the device will play audio effects.

### Direct Event Binding

**Direct event binding** allows devices to communicate directly, which makes your workflow more intuitive and gives you more freedom to focus on your design ideas.

Below are the [functions](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) and [events](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) for this device.

#### Functions

A [**function**](https://dev.epicgames.com/documentation/en-us/fortnite-creative/fortnite-creative-glossary#function) listens for an event on a device and then performs an action.

-
For any function, click the option, then Select Device to access and select from the Device dropdown menu.

-
Once you've selected a device, click Select Event and select the event that triggers this function.

-
If more than one device or event triggers a function, press the Add button to add a line and repeat these steps.

#### Receivers

Receivers listen for a channel and perform an action when they hear any device (including themselves) send a signal on that channel.

**אפשרויות ותיאורים:**

##### Register Player When Receiving From

Registers the instigating player when the device receives a signal on the selected channel. This player will be used when transmitting.

##### Activate When Receiving From

Activates the device, sending an event with the stored player as its instigator.

##### Clear Player When Receiving From

Clears the device when the device receives a signal on the selected channel.

##### Enable When Receiving From

Enables the device when the device receives a signal on the selected channel.

##### Disable When Receiving From

Disables the device when the device receives a signal on the selected channel.

#### Events

Direct event binding uses events as transmitters. An event tells another device to perform a function.

-
For any event option, click the option, then Select Device to access and select from the Device dropdown menu.

-
Once you've selected a device, click Select Function to bind the event to a function for that device.

-
If more than one function is triggered by the event, press the Add button and repeat.

**אפשרויות ותיאורים:**

##### On Activated Send Event To

When the device is activated, it transmits a signal on the selected channel. Uses the stored player as the instigator.

##### **On Tracked Stat Changed **Send Event To

When a tracked stat is updated, the device transmits a signal on the selected channel. Uses the stored player as the instigator.

##### **On Player Updated **Send Event To

When the registered player is updated, the device transmits a signal on the selected channel.

##### **On Player Update Fails **Send Event To

When the device attempts to update but fails, the device transmits a signal on the selected channel with the player that attempted to register as the instigator.

##### **On Player Replaced **Send Event To

When the registered player is replaced, the device transmits a signal on the selected channel with the replaced player as the instigator.

---

## Using Player Spawn Pad Devices in Fortnite Creative

**כותרת מקורית:** Using Player Spawn Pad Devices in Fortnite Creative  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/using-player-spawn-pad-devices-in-fortnite-creative  
**מקור קלט:** `07C_שחקנים_קבוצות_תפקידים_ומצלמות(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `using-player-spawn-pad-devices-in-fortnite-creative`

The **Player Spawner** device spawns the player at any location on their island.his device can only spawn one player. You will need to place individual spawners for islands with multiple players. Otherwise, they will always fall from the sky and have to parachute down.For help on how to find the **Player Spawner** device, see [****](https://dev.epicgames.com/documentation/fortnite/using-devices-in-fortnite-creative)**[Using Devices](https://dev.epicgames.com/documentation/fortnite/using-devices-in-fortnite)**.

If you're using multiple copies of a device on an island, it can be helpful to [rename](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#rename-a-device) them. You can choose names that relate to each device's purpose, so it's easier to remember what each one does.

### Device Options

You can configure this device with the following options.

Default values are **bold**.

**אפשרויות, ערכים ותיאורים:**

##### Player Team

- **Value / Values:** None, **Any**, Pick a team
- **Description:** Determines which team [spawns](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#spawning) on this pad.

##### Visible in Game

- **Value / Values:** **On**, Off
- **Description:** Determines whether the spawner is visible during games.

##### Use as Island Start

- **Value / Values:** **On**, Off
- **Description:** Determines whether or not a spawner can be used when players are spawning in to the island during the [Pre-Game phase](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#pre-game-phase).

##### Enabled During Phase

- **Value / Values:** **Always**, None, Create Only, Pre-Game Only, Gameplay Only
- **Description:** Determines the [game phases](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#game-phase) during which this device will be [enabled](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) during which the device will be enabled.

##### Player Class

- **Value / Values:** **Any**, No Class, Pick a team
- **Description:** Determines which class can activate the device.

##### Priority Group

- **Value / Values:** **Don't Override**, Pick a number
- **Description:** Determines the priority in which spawners will be used. Use the arrows to pick a number, or click in the field and type in a number. If all Primary spawners are unavailable, players will spawn on Secondary spawners and the Tertiary.

##### Play Audio

- **Value / Values:** **No**, Yes, Only If Visible
- **Description:** Determines whether the device should play audio effects.

##### Enemy Range Check

- **Value / Values:** **None**, Pick a range
- **Description:** If an enemy is within this radius, you can prefer not to spawn at this location. If no other locations are suitable, the player may still spawn here.

##### Display Enemy Range

- **Value / Values:** Off, On, **When Near**
- **Description:** Visualizes the **Enemy Range Check** option value. The location sphere will never show while playing, only during Create mode.

##### Respawn Alive Players

- **Value / Values:** **Yes**, No
- **Description:** If a **Respawn at Player Spawner** function is triggered, this determines if players who are alive are also respawned.

#### User Options

You can configure these options for this device under the **User Options** category.

 Option Value Description
**Player Team**

**Any**, None, Team Index

Only players on this team can spawn from this pad.

**User as Island Start**

**On**, Off

Determines whether or not a spawner can be used when players are spawning into the island during the Pre-Game phase.

**Visible in Game**

**On**, Off

Determines whether the spawner is visible during games.
 Advanced
**Enabled During Phase**

**Always**, Pre-Game Only, Gameplay Only, Create Only.

Determines the game phases during which the device will be enabled.

**Player Class**

**Any**, Class Slot, No Class

Only players on this class can spawn from this spawner.

**Priority Group**

**Don't Override**, Enter a priority number.

Determines the priority in which spawners will be used. The lower the better.

**Play Audio**

**No**, Yes, Only if Visible

Determines whether the device should play audio effects.

**Enemy Range Check **

Enter a range in meters

If the enemy is within this radius, prefer to not spawn at this location. If no other locations are suitable, players may still spawn here.

**Display Enemy Players**

**When Near**, Off, On

This is a debug feature to visualize the **Enemy Range Check** option. The sphere will never show while player and only appears during **Edit** mode.

**Respawn Alive Players**

**On**, off

Determines whether or not we respawn players that are alive when the **Respawn at Player **spawner is called.

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

##### Enable When Receiving From

Enables the device when an event occurs.

##### Disable When Receiving From

Disables the device when an event occurs.

##### Spawn Player When Receiving From

Spawns a player at this spawner, or respawns an existing player, when an event occurs.

#### Events

An [event](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#event) tells another device when to perform a function.

-
For any event option, click the **option**, then **Select Device** to access and select from the **Device dropdown menu**.

-
Once you've selected a device, click **Select Function** to bind the timer to a function for that device.

-
If more than one device is affected by the function, press the **Add** button and repeat.

**אפשרויות ותיאורים:**

##### On Player Spawned Send Event To

When a player spawns or respawns from this spawner, this sends an event to the selected device, which triggers the selected function.

##### On Spawn Failed Send Event To

When a player would spawn or respawn from this spawner, but the spawner is invalid or ineligible for spawning, this sends an event to the selected device, which triggers the selected function.

### Gameplay Examples

-
[Loadout Lobby](https://dev.epicgames.com/documentation/fortnite/loadout-lobby-in-fortnite-creative)

-
[Tug of War](https://dev.epicgames.com/documentation/fortnite/tug-of-war-in-fortnite-creative)

---

## Using Round Settings Devices in Fortnite Creative

**כותרת מקורית:** Using Round Settings Devices in Fortnite Creative  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/using-round-settings-devices-in-fortnite-creative  
**מקור קלט:** `07C_שחקנים_קבוצות_תפקידים_ומצלמות(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `using-round-settings-devices-in-fortnite-creative`

**
The **Round Settings** device is used for any round-based game that has customized gameplay within specific rounds. It generally defines what happens to the player’s inventory and rewards in each round. An example of a game mode that uses Round Settings extensively is [Search and Destroy](https://dev.epicgames.com/documentation/fortnite/search-and-destroy).

For help on how to find the Round Settings** device, see [Using Devices](https://dev.epicgames.com/documentation/fortnite/using-devices-in-fortnite).

If you're using multiple copies of a device on an island, it can be useful to rename them. Choosing names that relate to a device's purpose makes it easier to remember what each one does, and easier to find a specific device when using the [Event Browser](https://dev.epicgames.com/documentation/fortnite/event-browser-in-fortnite-creative).

### Contextual Filtering

Some devices are affected by a feature called contextual filtering. This feature hides or displays options depending on the values selected for certain related options. This feature will reduce clutter in the Customize panel and make options easier to manage and navigate.

However, it may not be easy to recognize which options or values trigger contextual filtering. To help you identify them, in our device docs we use *italic* for any values that trigger contextual filtering. All options will be listed, including those affected by contextual filtering; if they are hidden or displayed based on a specific option's value, there will be a note about that in the Description field for that option.

### Device Options

This device lets you manage your players' inventory and rewards between rounds, for example classes, weapons, items, and building resources.

In its default state, this device does nothing. It grants no resources and does not decide what happens to resources between rounds.

You can configure this device with the following options.

Default values are **bold**. Values that trigger contextual filtering are *italic*.

The Round Settings device can override My Island settings. Refer to the following documents for more information about My Island settings:

-
[Island Settings](https://dev.epicgames.com/documentation/fortnite/island-settings-in-uefn-and-fortnite-creative)

-
[Island Settings in Fortnite Creative](https://dev.epicgames.com/documentation/fortnite/understanding-island-settings-in-fortnite-creative)

-
[User Interface Settings](https://dev.epicgames.com/documentation/fortnite/user-interface-settings-in-fortnite-creative)

#### Basic Options

 Option Value Description
**Round**

**All**, 1 to 100

Defines the specific round to be customized.

**Override Keep Items Between Rounds**

**Don't Override**, *Override*

Override whether players should keep items between rounds.

**Keep Items Between Rounds**

**No**, Yes

Only visible when **Override Keep Items Between Rounds **is set to **Override**.

Sets whether players should keep items between rounds.

**Reset Class Each Round**

**No**, Yes

Determines whether or not the player's class is reset in this round.

**Wood Given Per Round**

**None**, Pick a number

The amount of wood resource the player receives each round.

**Metal Given Per Round**

**None**, Pick a number

The amount of metal resource the player receives each round.

**Stone Given Per Round**

**None**, Pick a number

The amount of stone resource the player receives each round.

**Gold Given Per Round**

**None**, Pick a number

The amount of gold the player receives each round.

**Override Last Standing Wins**

**Don't Override**, *Override*

Only visible when Override Last Standing Wins is set to Override.

Override whether to set the winner of the round to the last one standing.

**Last Standing Wins**

**No**, Yes

Determines whether set the winner of the round to the last one standing.

#### All Options

**אפשרויות, ערכים ותיאורים:**

##### Enabled On Minigame Start

- **Value / Values:** **Enabled**, Disabled
- **Description:** Determines whether or not the device is enabled at the start of a minigame.

##### Override Keep Items Between Rounds

- **Value / Values:** **Don't Override**, *Override*
- **Description:** Only visible when Override Keep Items Between Rounds is set to Override.

##### Override whether players should keep items between rounds.

- **Value / Values:** **Keep Items Between Rounds**
- **Description:** **No**, Yes

##### Sets whether players should keep items between rounds.

- **Value / Values:** **Keep Resources Between Rounds**
- **Description:** **Don't Override (-1.0f)**, Pick a percentage amount

##### Defines what percent of resources acquired in the previous round can be brought over to the current round.

- **Value / Values:** **Override Reload & Restock Weapons Each Round**
- **Description:** **Don't Override**, *Override*

##### Override whether to reload and restock weapons between rounds.

- **Value / Values:** **Reload & Restock Weapons Each Round**
- **Description:** **No**, Yes

##### Only visible when **Override Reload & Restock Weapons Each Round **is set to **Override**.

- **Value / Values:** Determines whether or not weapons are reloaded and restocked in the current round.
- **Description:** **Respawn Player On Class Reset**

##### **No**, Yes

- **Value / Values:** Determines whether or not players are forced to respawn when their class is reset.
- **Description:** **Clear All Items On Class Reset**

##### No, **Yes**

- **Value / Values:** Determines whether or not a player's inventory is cleared when their class is reset.
- **Description:** **Reset Current Vitals On Class Reset**

##### No, **Yes**

- **Value / Values:** Determines whether or not the player's health and shields are reset when their class is reset.
- **Description:** **Wood Given To Winners Per Round**

##### **None**, Pick a number

- **Value / Values:** The amount of wood given to the winner in each round.
- **Description:** **Metal Given To Winners Per Round**

##### **None**, Pick a number

- **Value / Values:** The amount of metal given to the winner in each round.
- **Description:** **Stone Given To Winners Per Round**

##### **None**, Pick a number

- **Value / Values:** The amount of stone given to the winner in each round.
- **Description:** **Gold Given To Winners Per Round**

##### **None**, Pick a number

- **Value / Values:** The amount of gold given to the winner in each round.
- **Description:** **Disable Matchmaking on Round End**

##### On, **Off**

- **Value / Values:** At the end of the round, this disables the ability for matchmaking to spawn players into the island, or the ability to join in-progress games that have matchmaking.
- **Description:** Disabling Matchmaking on Round End may not occur instantly if an Enable Matchmaking request has recently been made.

### Direct Event Binding

Following are the [direct event binding](https://dev.epicgames.com/documentation/fortnite/direct-event-binding) options for this device.

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

Enables the device.

##### Disable When Receiving From

Disables the device.

##### Enable Matchmaking When Receiving From

Enables the ability for players to Matchmake into the Island. Only applies to published games that have matchmaking turned on in the Island settings.

##### Disable Matchmaking When Receiving From

Disables the ability for players to Matchmake into the Island. Only applies to published games that have matchmaking turned on in the Island settings.

##### Disable End Round Conditions When Receiving From

Disables all end round conditions. Round must be ended by sending a trigger.

##### End Round When Receiving From

Ends the round. If triggered by a player, then the player's team is set as the winner.

##### Toggle Matchmaking When Receiving From

Toggles the ability for players to Matchmake into the Island. Only applies to published games that have matchmaking turned on in the Island settings.

##### **

Enabling, disabling and toggling matchmaking will not occur instantly if a conflicting matchmaking request has recently been made. For example, toggling matchmaking will be delayed if a Enable Matchmaking **request has been made recently.

#### Events

An [event](https://dev.epicgames.com/documentation/fortnite/event) tells another device when to perform a function.

-
For any event, click the **option**, then **Select Device** to access and select from the **Device** dropdown menu.

-
Once you've selected a device, click **Select Function** to bind this event to a function for that device.

-
If more than one function is triggered by the event, click the **Add** button to add a line and repeat these steps.

**אפשרויות ותיאורים:**

##### On Round Start Send Event To

Transmit when the rounds starts.

---

## Using Side Scroller Controls Devices in Fortnite Creative

**כותרת מקורית:** Using Side Scroller Controls Devices in Fortnite Creative  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/using-side-scroller-controls-devices-in-fortnite-creative  
**מקור קלט:** `07C_שחקנים_קבוצות_תפקידים_ומצלמות(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `using-side-scroller-controls-devices-in-fortnite-creative`

The **Control: Side Scroller** (Side Scroller Controls) device clamps the player's facing direction to the left-right axis so that no matter how they move, they are always facing left or right. Used with the [Fixed Point](https://dev.epicgames.com/documentation/fortnite/using-fixed-point-camera-devices-in-fortnite-creative) or [Fixed Angle Camera](https://dev.epicgames.com/documentation/fortnite/using-fixed-angle-camera-devices-in-fortnite-creative) devices, this gives you a toolbox to create all kinds of 2D retro-style games, such as [side-scrolling platformers](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) or [beat 'em ups](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary).

For help on how to find the **Side Scroller Controls** device, see [Using Devices](https://dev.epicgames.com/documentation/fortnite/using-devices-in-fortnite).

If you're using multiple copies of a device on an island, it can be useful to [rename](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) them. Choosing names that relate to a device's purpose makes it easier to remember what each one does, and easier to find a specific device when using the [Event Browser](https://dev.epicgames.com/documentation/fortnite/event-browser-in-fortnite-creative).

### Contextual Filtering

Some devices are affected by a feature called **contextual filtering**. This feature hides or displays options depending on the values selected for certain related options. This reduces clutter in the Customize panel and makes options easier to manage and navigate. To help identify them, values that trigger contextual filtering are in *italic*.

All options are listed, including those affected by contextual filtering; if they are hidden or displayed based on a specific option's value, there will be a note about it in the Description field for that option.

### Device Options
**

Default values are **bold**. Values that trigger contextual filtering are *italic*.

You can configure this device with the following options.

 Option Value Description
**Creative Preview**

N/A

Click **Start** to preview the controls. Click **Stop** to leave the preview and go back to editing your island.

**Priority**

**0**, Pick or enter a number

Multiple control devices can be present at any time, but only the one with the highest priority is considered active.

**Add to Players on Start**

**On**, Off

Determines whether this device is automatically added to all players when the game starts.

**Remove on Elimination**

On, **Off**

Determines whether this control device is removed from a player when they are eliminated.

**Enabled During Phase**

None, **Always**, Pre-Game Only, Gameplay Only

Determines which phases the control device is active in. If you choose **None**, the camera can only be enabled manually using events.

**Constrain Movement**

**On**, Off

When set to **On**, player movement is constrained to the direction indicated by the arrow on the device itself.

**Jump**

Disabled, **Dedicated**, Movement

Determines whether jumping is enabled, and if so what controls players use to jump. Select **Dedicated** to have players use the default jump control. Select **Movement** to have players use the Up control to jump.

**Crouch**

Disabled, **Dedicated**, Movement

Determines whether crouching is enabled, and if so what controls player use to crouch. Select **Dedicated** to have players use the default crouch control. Select **Movement** to have players use the Down control to crouch.

**Ranged Direction**

**Facing**, Cardinal Movement, Full Range Movement,* Full Range Manual*

Determines how the player aims while in side scroller mode. Values included are:

-
**Facing**: Uses the direction the player is facing to aim.

-
**Cardinal Movement**: Players can use the Up/Down/Left/Right controls to aim in those directions.

-
**Full Range Movement**: Uses the direction the player is moving to aim. So if the player is holding forward and up, they will aim forward and up.

-
**Full Range Manual**: Players aim using the mouse or right stick similar to a twin stick shooter.

**Lock Direction While Aiming**

On, **Off**

If this is set to **On**, the player's facing direction is locked when they are aiming.

**Lock Direction While Shooting**

On, **Off**

If this is set to **On**, the player's facing direction is locked when they are shooting.

**Movement Speed Multiplier**

**1.0x**, Pick an amount

Determines how fast the player moves, as a multiple of the default speed.

**Movement Speed Multiplier When Shooting**

**1.0x**, Pick an amount

Determines how fast the player moves while shooting, as a multiple of the default speed.

**Movement Speed Multiplier When Aiming**

**1.0x**, Pick an amount

Determines how fast the player moves while aiming, as a multiple of the default speed.

**Targeting Lock On**

Never, Always, Shooting, Aiming, **Shooting or Aiming**

When the player has a target, this determines when the player aims toward that target.

**Target Retention Duration**

**1.5 sec**, Pick a number of seconds

Determines the amount of seconds a player will attempt to face their target after each ranged action.

**Require Target on Screen**

**On**, Off

Determines whether or not the target has to be on screen in order for a target to be valid.

Require Target Line of Sight**

**On**, Off

Determines whether or not line of sight is required in order for a target to be valid.

**Ranged Targeting Distance**

**1000 cm**, Pick or enter an amount

Determines the maximum distance targets can be from the player to be considered valid targets.

**Ranged Targeting Height**

**500 cm**, Pick or enter an amount

Determines the maximum vertical distance targets can be from the player to be considered valid targets.

**Targeting Distance When Aiming**

**1000 cm**, Pick or enter an amount

Determines the maximum distance targets can be from the player to be considered valid targets when the player is aiming.

**Targeting Height When Aiming**

**300 cm**, Pick or enter an amount

Determines the maximum vertical distance targets can be from the player to be considered valid targets when the player is aiming.

**Ranged Targeting Angle**

**85°**, Pick a number of degrees

From the player's facing direction, this is the angle within which targets must be to be considered valid targets.

**Targeting Angle When Aiming**

**85°**, Pick a number of degrees

From the player's facing direction, this is the angle within which targets must be to be considered valid targets when the player is aiming.

**Require Line of Sight**

**On**, Off

Determines whether or not line of sight is required in order for a target to be valid.

**Base Weight Player**

**1.0**, Pick a number

Determines the targeting prioritization assigned to players. If you select **0**, players cannot be targeted.

**Base Weight Creatures**

**0.5**, Pick a number

Determines the targeting prioritization assigned to creatures. If you select **0**, creatures cannot be targeted.

**Base Weight Vehicles**

**0.3**, Pick a number

Determines the targeting prioritization assigned to vehicles. If you select **0**, vehicles cannot be targeted.

**Scale Weight by Distance**

**0.5**, Pick a number

Scales the target's calculated priority weight, reducing the final value by the target's distance from the player.

**Scale Weight by Angle**

**1**, Pick a number

Scales the target's calculated priority weight, reducing the final value by the target's angle to the player.

**Affects Team**

**Any**, Pick or enter a team

Determines which team is affected by this device.

**Invert Team**

On, **Off**

If this is set to **On**, all teams are affected by this device except the team selected in the **Affects Team** option.

**Affects Class**

No Class, All, **Any**, Pick or enter a class

Determines which classes are affected by this device. **No Class** means only players with no assigned class are affected. **All** means all players, including those with no assigned class, are affected. **Any** means players with any assigned class are affected.

**Invert Class**

On, **Off**

If this is set to **On**, all classes are affected by this device except the class selected in the **Affects Class** option.

**Targetable Device in Edit Mode**

On, **Off**

Determines whether the device itself is targetable. If set to **On**, the device is only targetable when you are editing your island.

### Direct Event Binding

Following are the [direct event binding](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) options for this device.

#### Functions

A [function](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) listens for an event on a device then performs an action.

-
For any function, click the **option**, then **Select Device** to access and select from the **Device** **dropdown menu**.

-
Once you've selected a device, click **Select Event** to bind the device to an event that will trigger the function for the device.

-
If more than one device or event triggers a function, click the **Add** button to add a line and repeat these steps.

**אפשרויות ותיאורים:**

##### Enable When Receiving From

Enables the device when an event occurs.

##### Disable When Receiving From

Disables the device when an event occurs.

##### Add to When Receiving From

Adds this device to the instigating player when an event occurs.

##### Remove From When Receiving From

Removes this device from the instigating player when an event occurs.

##### Add to All When Receiving From

Adds this device to all players when an event occurs.

##### Remove From All When Receiving From

Removes this device from all players when an event occurs.

#### Events

This device has no events.

### Use Side Scroller Controls Device In Verse

#### Side Scroller Controls API

See the [Side Scroller Controls API Reference](https://dev.epicgames.com/documentation/en-us/uefn/verse-api/fortnitedotcom/devices/button_device) for more information on using the Side Scroller Controls device in Verse.

---

## Using Team Settings and Inventory Devices In Fortnite Creative

**כותרת מקורית:** Using Team Settings and Inventory Devices In Fortnite Creative  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/using-team-settings-and-inventory-devices-in-fortnite-creative  
**מקור קלט:** `07C_שחקנים_קבוצות_תפקידים_ומצלמות(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `using-team-settings-and-inventory-devices-in-fortnite-creative`

**
The **Team Settings & Inventory** device is important for most team-based games. It provides team and inventory configurations that go beyond the choices the [Island Settings](https://dev.epicgames.com/documentation/fortnite/understanding-island-settings-in-fortnite-creative) give you. You can also use this to customize individual devices, and create variations in team setup.

There is a hierarchy of setting overrides, described as follows:

-
Island Settings** are the baseline.

-
**Team Settings & Inventory** overrides Island Settings if there is a specific value set in the device.

-
**Class Designer** overrides both Team Settings & Inventory and Island Settings, if there is a specific value set in the device that differs from the Island Settings or Team Settings & Inventory values.

To find the Team Settings & Inventory device, go to the Creative inventory and select the Devices tab. From there you can search or browse for the device. For more information on finding devices see [Finding and Placing Devices](https://dev.epicgames.com/documentation/fortnite/using-devices-in-fortnite).

If you're using multiple copies of a device on an island, it can be helpful to [rename](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#rename-a-device) them. You can choose names that relate to each device's purpose, so it's easier to remember what each one does.

### Device Options

When this device is placed, the device uses settings inherited from the Island Settings in its default state. Because of this, it has no effect on the game until you customize it.

This device has some basic functionality, like setting max [health](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#health) and max [shields](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#shield), as well as setting a spawn limit. Additionally, there are some advanced options, like how much [resource](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#resource) or [score](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#score) a player is granted when they eliminate another player.

Default values are **bold**. Values that trigger contextual filtering are *italic*.

#### General Options

You can configure these options for this device under the **General** category.

 Option Value Description
**Team Name**

Enter a name

Type a name for the team in the text field. The text field has a character limit of 24 characters.

**Team Description**

Enter text

Type a description for the team in the text field. The text field has a character limit of 512 characters.

**Team**

 **All**, Pick or enter a team

Specifies which team the settings on this device apply to.

**Team Color**

 **Don't Override,** Pick a color

Determines whether the game uses the default color for the team, or if it uses the color you pick here.

 **Team Icon**

 **None**, Pick an icon

 Determines the icon used for the team. Click the icon to open the Icon Library Picker. You can scroll through the icons to find one, or you can type a word into the search bar at the top and click the Search button. Select an icon, then click the checkmark.
**

 Default Class Identifier**

 **Don't Override,** None, Pick a class number

Defines the default class assigned to players at the start of the game, or if a player's chosen class is reset.

-
**Don't Override: **Classes keep the default [class identifier](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#class-identifier) defined in the [Class Designer](https://dev.epicgames.com/documentation/fortnite/using-class-designer-devices-in-fortnite-creative) device or island settings.

-
**None: **There is no default class.

-
**Class Number:** Override the default class identifier defined in the [Class Designer](https://dev.epicgames.com/documentation/fortnite/using-class-designer-devices-in-fortnite-creative) device or island settings, and assign the selected class identifier instead.

**Max Initial Team Size**

**Don't Override,** Unlimited, Pick a team size

Determines the maximum team size at the start of the game. During the game, more players can be added to this team using the After Last Spawn Go To option.

**Initial Team Size Ratio**

 **Don't Override, **Pick an amount

Determines number of players to be placed in this team at the start of the game, relative to the size of other teams. This is capped by the number set in the Max Initial Team Size option.

#### Player Options

 You can configure these options for this device under the **Player **category.

Options

Value

Description
 Inventory
**Grant Items On Respawn**

Yes, **No**

Determines whether the device grants its items when players on this team respawn.

**Grant Condition**

**Always**, Only When Empty

Determines whether the device grants its items to a player when they respawn, or only if the player's inventory is empty. For this to be used, the Grant Items On Respawn option must be set to Yes.

**On-Grant Behavior**

**Clear All**, Clear Items, Keep All

Determines what happens to the player's inventory when the player respawns.

**Equip Granted Item**

**Don't Equip**, Pick an item

If the device grants items to the player, this determines which items (listed in order) should be equipped. If you choose an item slot that is higher than the total number of items in the device, the device grants the last item in the list.

**Initial Weapon Ammo**

**Don't Override**, Pick or enter an amount

Sets the amount of ammunition loaded in the weapon when granted, limited by the weapon's magazine size.

**Spare Weapon Ammo**

**Don't Override**, Pick or enter an amount

Sets how much spare ammunition is added to the player's inventory when a weapon is granted. Default provides ammo based on the ammo type used by the weapon.

**No Cooldowns After Use**

**Don't Override**, On, Off

Determines whether players have no cooldown on weapons and abilities during the game. This does not affect cooldowns prevented by the No Cooldowns After Swap setting.

**No Cooldowns After Swap**

**Don't Override**, On, Off

Determines whether players have no cooldown after swapping weapons or items during the game.

**Infinite Reserve Ammo**

**Don't Override**, On, Off

Determines whether players have infinite reserve ammunition during the game. If you have a Class Designer device, the options for that device can override this.

**Infinite Magazine Ammo**

**Don't Override**, On, Off

Determines whether players have infinite magazine ammunition during the game.

**Infinite Charges**

**Don't Override**, On, Off

Determines whether players have infinite charges for weapons and abilities during the game.

**Infinite Reserve Energy**

**Don't Override**, On, Off

Determines if players have infinite reserve energy for weapons and abilities during the game.

**Infinite Loaded Energy**

**Don't Override**, On, Off

Determines whether players have infinite loaded energy for weapons and abilities during the game.

**Infinite Durability**

**Don't Override**, On, Off

Determines if players have infinite durability for weapons and items during the game.

**Infinite Consumables**

**Don't Override, **On, Off

Determines whether players have infinite consumable items (such as grenades, health items, traps, and so on).

**Infinite Building Resources**

**Don't Override**, On, Off

Determines whether player building resources are infinitely available in-game.

**Infinite Gold**

**Don't Override**, On, Off

Determines whether players have infinite gold during the game.

**Infinite World Resources**

**Don't Override**, On, Off

Determines whether players have infinite world resources during the game.

**Eliminated Player's Items**

**Don't Override, **Drop, Keep, Delete

Determines what happens to the player's items when the player is eliminated. If you have a Class Designer device, the options for that device can override this. Values for this option are:

-
**Don't Override:** This device does not affect eliminated player items.

-
Drop: Items are dropped on the ground. Other players can pick them up.

-
Keep: Player keeps items.

-
**Delete:** Items are removed from the game.

**Eliminated Player's Resources**

**Don't Override, **Drop, Keep, Delete

Determines what happens to a player's resources when the player is eliminated. If you have a Class Designer device, the options for that device can override this. Values for this option are:

-
**Don't Override:** This device does not affect eliminated player resources.

-
**Drop:** Resources are dropped on the ground. Other players can pick them up.

-
**Keep:** Player keeps resources.

-
**Delete:** Resources are removed from the game.

**Eliminated Player's Game Resources**

**Don't Override, **Drop, Keep, Delete

Determines what happens to a player's game resources when the player is eliminated. If you have a Class Designer device, the options for that device can override this.

-
**Don't Override:** This device does not affect eliminated player resources.

-
**Drop:** Resources are dropped on the ground. Other players can pick them up.

-
**Keep:** Player keeps resources.

-
**Delete: **Resources are removed from the game.

**Allow Item Drop**

**Don't Override, **Yes, No

Determines if players can drop items from their inventory during the game. If you have a Class Designer device, the options for that device can override this.

**Display Empty Ammo Slots**

**Don't Override, **Yes, No

Determines whether empty ammo slots are shown in the player's inventory.
 Equipment
**Start With Pickaxe**

**Don't Override, **No, Yes

Determines whether or not players start the game with a pickaxe.

**Instant Reload**

**Don't Override, **On, Off

Determines whether weapons ignore their normal reload time and reload instantly instead. If you have a Class Designer device, the options for that device can override this.

**Maximum Equipment Slots**

**Don't Override, **None, Pick a number

Set the maximum number of equipment slots a player can have during the game.
 Health
**Invincibility**

**Don't Override, **On, Off

Determines if players should spawn with invincibility. If this is set to Don't Override or Off, the Starting Health Percentage option is displayed below this one.

**Starting Health Percentage**

**Don't Override, **Pick or enter an amount

This option only displays if the Invincibility option is set to Don't Override or Off. Determines how much health a player has when they spawn.

**Max Health**

**Don't Override, **Pick or enter an amount

Determines the maximum amount of health players can have during the game. If you have a Class Designer device, the options for that device can override this.

**Allow Heath Recharge**

**On**, Off

Determine if health recharge is available or not. Health recharge allows player health to regenerate over time.

**Health Recharge Period**

**6.5 seconds**, Pick or enter a number

When the **Allow Health Recharge** option is set to Yes, this option becomes available. Determines the tick period of the health recharge.
 Shields
**Starting Shield Percentage**

**Don't Override, **Pick or enter an amount

Determines the player's shield value when they spawn.

**Max Shields**

**Don't Override, **Pick or enter a number

Determines the maximum shield value a player can reach during the game.

**Allow Shield Recharge**

On, **Off**

Determines if shield recharge is available or not. Shield recharge allows player shields to regenerate over time.

**Shield Recharge Period**

**1.0 seconds**, Pick or enter a number

Determines the tick period that shields recharge.

**Allow Overshield**

**Don't Override, **On, Off

Determines whether the Overshield feature is available.

**Overshield Max**

**Don't Override, **Pick or enter an amount

This only displays if you have set the Overshield: More Options option to Show. Determines the maximum amount of Overshield a player can have. If you set an amount here, it will override any amount set in the Island Settings.

**Overshield Recharge Delay**

**Don't Override, **Pick or enter an amount

This only displays if you have set the Overshield: More Options option to Show. The Overshield starts to recharge after this amount of time if the player takes no damage during the delay. If you set the delay here, it will override the delay set in the Island Settings.

**Overshield Recharge Rate**

**Don't Override, **Pick or enter an amount

This only displays if you have set the Overshield: More Options option to Show. Determines how much the Overshield recharges each second, after the recharge delay has ended. If you set the recharge amount here, it will override the recharge amount in the Island Settings.

**Overshield Recharge Period**

**Don't Override, **Pick or enter an amount

This only displays if you have set the Overshield: More Options option to Show. Determines the tick period of time the Overshield recharges at .
 Locomotion
**Movement Multiplier**

**Don't Override, **Pick or enter a multiplier

Sets a value that is multiplied by the player's base movement speed. This defaults to 1. Numbers lower than 1 will make players move slower, numbers higher than 1 will make the player move faster.

**Allow Sprinting**

**Don't Override, **On, Off

Determines whether the Sprinting feature is available.

**Sprinting Energy Cost Per Second**

**Don't Override, **Pick or enter an amount

This only displays if you have set the Sprinting: More Options option to Show. Determines how fast Sprinting Energy is drained each second while a player is sprinting. If you set the energy cost here, it will override the energy cost set in the Island Settings.

**Sprinting Jump Multiplier**

**Don't Override, **Pick or enter a multiplier

This only displays if you have set the Sprinting: More Options option to Show. Determines how much higher or farther players jump when sprinting, as a multiple of normal jump height or length. If you set the jump multiplier here, it will override the jump multiplier set in the Island Settings.

**Sprinting Speed Multiplier**

**Don't Override, **Pick or enter a multiplier

This only displays if you have set the Sprinting: More Options option to Show. Determines how fast a player moves when sprinting, as a multiple of their speed when not sprinting. If you set the sprint speed here, it will override the sprint speed set in the Island Settings.

**Energy Max**

**Don't Override, **Pick or enter an amount

Determines how much Energy is available to the player. This affects Sprinting, as well as other abilities that use Energy.

**Energy Recharge Amount**

**Don't Override, **Pick or enter an amount

When Energy begins to recharge, this determines the amount of Energy recharged each second.

**Energy Recharge Delay**

**Don't Override, **Pick or enter a time

After a player stops using Energy, this sets the length of delay before the player's Energy begins to recharge.

**Allow Sliding**

**Don't Override, **On, Off

Determines whether the Sliding feature is available.

**Allow Slide Kick**

**Don't Override, **On, Off

Determines whether sliding players can use the Slide Kick to impact and knock away players on an opposing team.

**Allow Shoulder Bashing**

**Don't Override**, On, Off

Determines whether the Shoulder Bashing feature is available.

**Fall Damage**

**Don't Override, **On, Off

Determines whether players are affected by fall damage during the game. If you have a Class Designer device, the options for that device can override this.

**Gravity**

**Don't Override, **Very Low, Low, Normal, High, Very High

Changing the Gravity affects how high players can jump, as well as how much damage players take when they fall. If you have a Class Designer device, the options for that device can override this.

**Jump Fatigue**

**Don't Override**, On, Off

Determines whether continuous jumping applies a penalty to jump height. If you have a Class Designer device, the options for that device can override this.

**Player Flight**

**Don't Override**, On, Off

Determines whether players can fly during the game. If you have a Class Designer device, the options for that device can override this.

**Allow Mantling**

**Don't Override, **On, Off

Determines whether the Mantling feature is available.

**Mantling Minimum Height**

**Don't Override, **Very Low, Low, Normal, High

This only displays if you have set the Show More Options: Mantling option to Show. Determines the lowest height at which a player can use mantling on a ledge. You might want to adjust this value if gravity or other factors affect mantling.

**Mantling Minimum Height In Water**

**Don't Override, **Very Low, Low, Normal, High

This only displays if you have set the Show More Options: Mantling option to Show. Determines the lowest height at which a player can mantle from the water. You might want to adjust this value if gravity or other factors affect mantling.

**Allow Vaulting**

**Don't Override**, On, Off

Determines if players can vault over low obstacles. If you choose On, players will vault over obstacles automatically if they are sprinting toward the obstacle.

**Glider Redeploy**

**Don't Override**, On, Off

Determines whether players can freely deploy gliders without using an item item. If you have a Class Designer device, the options for that device can override this.
 Building Pickups Self Damage
**Allow Building**

**Don't Override**, None, All, Traps Only, No Traps

Determines whether players can build or place traps. If you have a Class Designer device, the options for that device can override this.Values for this option are:None: The player can neither build nor place traps.All: The player can build or place traps, if they have the required resources.Traps Only: The player cannot build, but can place traps.No Traps: The player can build, but not place traps.

**Maximum Building Resources**

**Don't Override**, Pick an amount

Sets the maximum amount of resources a player can carry during the game. If you have a Class Designer device, the options for that device can override this.

**Self-Damage On Hit Amount**

**Don't Override**, Pick an amount

Sets the amount of damage players deal to themselves when they hit something else.

**Self-Damage Only On Non-Zero Damage**

**Don't Override**, Yes, No

Determines whether or not the player only receives self-damage when the player inflicts non-zero damage to something else.

**Self-Damage Target Filter**

**Don't Override**, Non-Players, Players Only, All

Specifies which targets cause self-damage when hit.

**Self-Damage Weapon Filter**

**Don't Override**, Pickaxe Only, Melee Only, Ranged Only, All

Determines which weapons can inflict self-damage.

**Allow Item Pick Up**

**Don't Override**, Yes, No

Determines whether players can pick up items during the game. If you have a Class Designer device, the options for that device can override this.

#### In-Game Interface Options

You can configure these options for this device under the **In-Game Interface **category.

Options

Value

Description
 Nameplate
**Always Show Name Plates**

**Don't Override**, Always Show to Team, Always Show to All, Always Hide, No

Determines whether players names and locations can be seen by other players.

**Name Plate Max Distance**

**Don't Override,** pick a distance.

If set to a number, player name plates will disappear if that player is further away than that distance from the camera.

**Name Plate Line of Sight**

**Don't Override**, Always Show, Hide Behind Obstacles

If set, the name plates are hidden whenever a player is obstructed by an obstacle. If this is set to Hide Behind Objects, an additional option displays below this one.

**Focus for Name Plates**

**No**, Only Hostile, Always show to all

Defines if you need to be looking at a player for their name plate to appear.

**Focus Angle**

**Don't Override**, Pick or enter an angle

When focusing, this is the maximum angle a player can be from the look direction of another player in order to be valid for focusing.

**Focus Time**

**Don't Override**, Pick or enter an amount

How long you need to focus on a player for their name plate to be visible.

**Show Voice Indicator**

**Don't Override**, Don't Override Show Name Plates, Always Show to Team, Always Show to Hostiles, Always Show to All, Disable

Determines whether the voice indicator can be seen on a player's name plate. Can be used to control the voice indicator and name plate separately.

**Show Player Health Indicator**

**Don't Override**, Team Only, Enemies, Anyone, Never

Determines who can see the health indicators over players' heads. If you have a Class Designer device, the options for that device can override this.

**Limit Name Plate Max Distance**

**Don't Override**, Yes, No

Determines if name plates should disappear based on distance from the camera.
 HUD
**Display Health for All Players**

**Don't Override**, Yes, No

Determines whether all players get a health bar displayed on the HUD for this team or class. If this is enabled for a team with more than one player, or enabled for multiple teams, this will only display the health of one player at a time. If you have a Class Designer device, the options for that device can override this.

**Wood Resource Widget Is Visible**

**Don't Override**, Yes, No

If this is set to Yes, players can see the wood resource widget.

**Stone Resource Widget Is Visible**

**Don't Override**, Yes, No

If this is set to Yes, players can see the stone resource widget.

**Metal Resource Widget Is Visible**

**Don't Override**, Yes, No

If this is set to Yes, players can see the metal resource widget.

**Gold Resource Widget Is Visible**

**Don't Override**, Yes, No

If this is set to Yes, players can see the gold resource widget.

#### Mode Options

You can configure these options for this device under the **Mode** category.

Options

Value

Description
 Eliminations
**Down But Not Out**

**Don't Override**, Default, On, Off

Determines whether the player can be put into the **Down But Not Out** state. If you choose Default, this will be determined automatically depending on team size. If you have a **Class Designer** device, the options for that device can override this.

**Drop Reboot Card on Elimination**

**Don't Override**, On, Off

Determines if a player drops a Reboot Card when they are eliminated. Reboot Cards only drop if the eliminated player has a teammate eligible to use a Reboot Van.

**Health Granted On Elimination**

**Don't Override**, Pick an amount

Specifies how much health the player gets when they eliminate another player. Any health awarded above the player's **Max Health** value is awarded as shields instead.

**Wood Granted On Elimination**

**Don't Override**, Pick an amount

Specifies how much wood the player gets when they eliminate another player.

**Stone Granted On Elimination**

**Don't Override**, Pick an amount

Specifies how much stone the player gets when they eliminate another player.

**Metal Granted On Elimination**

**Don't Override**, Pick an amount

Specifies how much metal the player gets when they eliminate another player.

Gold Granted On Elimination

**Don't Override**, Pick an amount

Specifies how much gold the player gets when they eliminate another player.
 Spawning
**Respawn Time**

**Don't Override**, Pick or enter an amount of time

Determines the amount of time (in seconds) the player must wait after being eliminated before they are respawned back into the game. If you have a **Class Designer** device, the options for that device can override this.

**Only Allow Respawning If Spawn Pads Found**

**Don't Override**, No, Yes

If you choose Yes, players can only respawn if there is a spawn pad available.

**Respawn Type**

**Don't Override**, Individual, Wave

Changing the respawn type to Wave causes all eliminated team members during a certain window to respawn together. Set the time in the Respawn Time option.

**Spawn Limit**

**Don't Override**, Infinite, Pick a number

Determines the number of times the player can spawn into the game, including the initial spawn at the start of the game. If you choose 1 it means the player can't respawn after they are eliminated. If you have a **Class Designer** device, the options for that device can override this.

**After Last Spawn Go To**

**Don't Override**, Spectator, Pick a team

Determines which team a player joins after they use all of their permitted spawns.

**Spawn Location**

**Don't Override**, Spawn Pads, Sky, Current Location, Do Not Spawn

Determines where the player will spawn when the game starts. If you have a Class Designer device, the options for that device can override this. Values for this option are:

-
**Don't Override:** This device does not affect spawn location.

-
**Spawn Pads:** Players spawn on designated spawn pads.

-
**Sky: **Up in the air where the player will parachute down.

-
**Current Location:** Where the player is currently located.

-
**Do Not Spawn:** The player is not spawned.

**Override Spawn Immunity Time**

**Don't Override**, Yes, No

Determines if the invulnerability time granted to a player after respawn should be overridden. If this is set to Yes, an additional option displays below this one.

**Spawn Immunity Time**

**Don't Override**, Default, None, Pick or enter an amount of time

This option only displays if the Override Spawn Immunity Time option is set to Yes. Determines how long invulnerability is granted to a player when they respawn.

**Spawn Event Activates for AI**

**On**, Off

Determines if the On Team Member Spawned event will activate for AI that are on the device's team.

**Spawn Event Activates for Players**

**On**, Off

Determines if the **On Team Member Spawned** event will activate for players that are on the device's team.

**Respawn Alive Players**

Yes, No

Determines if players who are alive also respawn when the Respawn at Player Spawner function is triggered.
 Victory Condition
**Win on Time Out**

**Don't Override**, Yes, No

Sets the win condition for the team to be when the game ends by running out of time.
 Scoring
**Use Team Score**

**Don't Override**, Yes, No

Determines whether a team gains score with its players, or whether the team score uses a sum of its players' scores. If you choose Yes, the team retains its score even if a player leaves the team or the game.

**Elimination Score**

**Don't Override**, Pick an amount

Sets the amount of score awarded to a player on this team when they eliminate another player.

**Assist Score**

**Don't Override**, Pick an amount

Sets the amount of score awarded to a player on this team when they assist in eliminating another player.
 Team Settings
**Allow Friendly Fire**

**Don't Override**, Yes, No

Determines whether or not a player can damage another player on their team.

**Allow Impulsing Teammates**

On, Off

Determines whether teammates can use impulses such as Shockwave Grenades or Shove on each other.

**Dynamic Team Emotes**

**Don't Override**, Yes, No

Determines whether players on a team can use emotes to extend team invites to other players.If this is set to Enabled, a two-person emote will be added to players' collection. Players can press and hold B, then click Manage Teams to select the team invite emote.

**Dynamic Team Leave**

**Don't Override**, Yes, No

This setting is only editable if the **Dynamic Team Emotes** option is set to Enabled. Determines whether players invited to a team can leave it using emotes.

If this is set to Enabled, an emote is added to the player's collection that can be used to leave the player's current team. Players can press and hold B, then click Manage Teams to select the Leave Team emote.

#### Round Options

You can configure these options for this device under the **Round** category.

Options

Value

Description
 End Condition
**Eliminations To End**

**Don't Override**, Off, Pick a number

Causes the round to end when this team has gotten the chosen number of eliminations.

**Creature Eliminations To End**

**Don't Override**, Off, Pick a number

Causes the round to end when this team has destroyed the chosen number of creatures.

**Objectives To End**

**Don't Override**, Off, Pick a number

Causes the round to end when this team has completed the chosen number of objectives.

**Collect Items To End**

**Don't Override**, Off, All, Pick a number

Causes the round to end when this team has collected the chosen number of collectible objects.

**Collect Item Count to End**

**1**, Pick a number.

Requires **Collect Items to End** to be overridden and set to **Specific Count**.

Causes the round to end when the selected team has acquired the specific number of Collectible objects.

**Score To End**

**Don't Override**, Off, Pick a number

Causes the round to end when this team has achieved the chosen score.

#### World Options

You can configure these options for this device under the **World** category.

Options

Value

Description
 Harvesting
**Harvest Multiplier**

**Don't Override**, Pick a multiplier

Determines the rate at which players can harvest resources from world objects. If you have a Class Designer device, the options for that device can override this.

#### User Options

You can configure these options for this device under the **User Options** category.

**אפשרויות, ערכים ותיאורים:**

##### item Definition

- **Value / Values:** Pick an item definition asset
- **Description:** Choose and item definition to assign.

##### Item Quantity

- **Value / Values:** **1**, pick an amount.
- **Description:** Assign a quantity to the assigned item definition.

### Direct Event Binding

Direct event binding allows devices to communicate directly, which makes your workflow more intuitive, and gives you more freedom to focus on your design ideas.

Below are the following direct event binding options for this device.

#### Functions

A [function](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#function) listens for an event on a device then performs an action.

-
For any function, click the **option**, then **Select Device** to access and select from the **Device dropdown menu**.

-
Once you've selected a device, click **Select Event** to bind the device to an event that will trigger the function for the device.

-
If more than one device or event triggers a function, click the **Add** button to add a line and repeat these steps.

**אפשרויות ותיאורים:**

##### End Round When Receiving From

This function ends the round when an event occurs.

##### Respawn at Player Spawner When Receiving From

This function respawns the instigating player at the most appropriate player spawner.

##### Force Spectate

This function immediately forces the instigator into spectate mode without any elimination penalty. They will not respawn automatically. The instigator must match the device's team.

#### Events

An [event](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#event) tells another device when to perform a function.

-
For any event option, click the **option**, then **Select Device** to access and select from the **Device dropdown menu**.

-
Once you've selected a device, click **Select Function** to bind the timer to a function for that device.

-
If more than one device is affected by the function, press the **Add** button and repeat.

**אפשרויות ותיאורים:**

##### On Team Is Out of Respawns Send Event To

When a team is out of respawns, an event is sent to the selected device, which triggers the selected function.

##### On Enemy Eliminated by Team Member Send Event To

When an enemy is eliminated by a team member, an event is sent to the selected device, which triggers the selected function.

##### On Team Member Eliminated Send Event To

When a team memeber is eliminated, an event is sent to the selected device, which triggers the selected function.

##### On Team Member Spawned Send Event To

When a team member is spawned, an event is sent to the selected device, which triggers the selected function.

---

## Using Third Person Controls Devices in Fortnite Creative

**כותרת מקורית:** Using Third Person Controls Devices in Fortnite Creative  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/using-third-person-controls-devices-in-fortnite-creative  
**מקור קלט:** `07C_שחקנים_קבוצות_תפקידים_ומצלמות(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `using-third-person-controls-devices-in-fortnite-creative`

The **Control: Third Person** (Third Person Controls) device is designed for use alongside the [Fixed Angle Camera](https://dev.epicgames.com/documentation/fortnite/using-fixed-angle-camera-devices-in-fortnite-creative), [Fixed Point Camera](https://dev.epicgames.com/documentation/fortnite/using-fixed-point-camera-devices-in-fortnite-creative), and [Orbit Camera](https://dev.epicgames.com/documentation/fortnite/using-orbit-camera-devices-in-fortnite-creative) devices. The Third Person Controls device has two main functions:

-
Configuring movement and facing settings for players affected by camera devices

-
Configuring targeting behavior for players affected by camera devices

Because the camera devices change what the player sees, the usual controls for movement and other player actions will be different. This device is where you determine the direction the player faces, how they target enemies or objects for interaction, how fast they move, and so on.

To learn more about how to use the camera and controls devices together, see [Designing with Cameras and Controls](https://dev.epicgames.com/documentation/fortnite/designing-with-cameras-and-controls-in-fortnite-creative).
To learn about using cameras in UEFN, see:

-
[Gameplay Camera and Control Devices](https://dev.epicgames.com/documentation/en-us/uefn/gameplay-camera-and-control-devices-in-unreal-editor-for-fortnite)

-
[Making a Title Sequence](https://dev.epicgames.com/documentation/en-us/uefn/making-a-title-sequence-in-unreal-editor-for-fortnite) gameplay example

For help on how to find the **Third Person Controls** device, see [Using Devices](https://dev.epicgames.com/documentation/fortnite/using-devices-in-fortnite).

### Contextual Filtering

Some devices are affected by a feature called **contextual filtering**. This feature hides or displays options depending on the values selected for certain related options. This feature will reduce clutter in the Customize panel and make options easier to manage and navigate.

However, it may not be easy to recognize which options or values trigger contextual filtering. To help you identify them, in our device docs we use *italic* for any values that trigger contextual filtering. All options will be listed, including those affected by contextual filtering; if they are hidden or displayed based on a specific option’s value, there will be a note about that in the Description field for that option.

### Device Options

Configure this device with the following options.
**

Default values are **bold**. Values that trigger contextual filtering are *italic*.

**אפשרויות, ערכים ותיאורים:**

##### Creative Preview

- **Value / Values:** N/A
- **Description:** Click **Start** to preview what the camera is seeing. Click **Stop** to leave the preview and go back to editing your island.

##### Priority

- **Value / Values:** **0.0**, Pick or enter a number
- **Description:** Multiple cameras can be present at any time, but only the one with the highest priority is considered active.

##### Add to Players on Start

- **Value / Values:** **On**, Off
- **Description:** Determines whether this device is automatically added to all players when the game starts.

##### Remove on Elimination

- **Value / Values:** On, **Off**
- **Description:** Determines whether this camera is removed from a player when they are eliminated.

##### Enabled During Phase

- **Value / Values:** None, **Always**, Gameplay Only
- **Description:** Determines which phases the camera is active in. If you choose **None**, the camera can only be enabled manually using events.

##### Facing Direction

- **Value / Values:** **Movement**, *Twin Stick*, *Fixed*
- **Description:** Determines which direction the player is facing during gameplay. If you choose **Fixed**, another option displays below this one. Values for this option are:

#### -
**Movement**: Players face in the direction they are moving.

- **Value / Values:** -
**Twin Stick**: Players can change their facing direction based on an input, such as the mouse cursor position or the direction a joystick is pushed on a controller.
- **Description:** -
**Fixed**: Players always face a specific direction, inferred from the value of the **Fixed Facing Angle** option.

##### Twin Stick Mouse Aim Mode

- **Value / Values:** **Target Cursor**, Dial Aiming
- **Description:** This option only displays if you set the **Facing Direction** option to **Twin Stick**. This determines where the player will aim when they are using a mouse. Values for this option are:

#### -
**Target Cursor**: The player will aim towards the mouse cursor's location.

- **Value / Values:** -
**Dial Aiming**: The mouse will act as analog joystick, and the player will aim in the direction the mouse is moved.
- **Description:** **Auto Fire On Controller**

##### On, **Off**

- **Value / Values:** Determines whether the player's weapon automatically fires when the player is using the right stick on a controller.
- **Description:** **Fixed Facing Angle**

##### **0 degrees**, pick or enter a number

- **Value / Values:** This option only displays if the **Facing Direction** option is set to **Fixed**. Determines the direction that players face during gameplay.
- **Description:** **Movement Speed Multiplier**

##### **1.0x**, Pick an amount

- **Value / Values:** Determines how fast the player moves, as a multiple of the default speed.
- **Description:** **Movement Speed Multiplier When Shooting**

##### **1.0x**, Pick an amount

- **Value / Values:** Determines how fast the player moves while shooting, as a multiple of the default speed.
- **Description:** **Movement Speed Multiplier When Aiming**

##### **1.0x**, Pick an amount

- **Value / Values:** Determines how fast the player moves while aiming, as a multiple of the default speed.
- **Description:** **Turn Speed Multiplier**

##### **1.0**, Pick an amount

- **Value / Values:** Determines the player's speed while turning, as a multiplier of the default speed.
- **Description:** **Turn Speed Multiplier When Shooting**

##### **1.0x**, Pick an amount

- **Value / Values:** Determines the player's turning speed while shooting, as a multiplier of the default speed.
- **Description:** **Turn Speed Multiplier When Aiming**

##### **1.0x**, Pick an amount

- **Value / Values:** Determines the player's turning speed while aiming, as a multiplier of the default speed.
- **Description:** **Turn Speed Multiplier When Sprinting**

##### **1.0x**, Pick an amount

- **Value / Values:** Determines the player's turning speed while sprinting, as a multiplier of the default speed.
- **Description:** **Targeting Assistance**

##### **On**, Off

- **Value / Values:** When this is set to **On**, players will auto-select a target based on distance, angle and targeting priorities.
- **Description:** If you have **Facing Direction** set to **Twin Stick**, and you have **Targeting Assistance** set to **On**, players can break out of auto-targeting by moving the right joystick or their mouse after the target is locked on.

##### Targeting Lock On

- **Value / Values:** Never, Always, Shooting, Aiming, **Shooting or Aiming**
- **Description:** This option only displays if the **Targeting Assistance** option is set to **On**. Determines when players turn towards their target, when a target is selected.

##### Target Retention Duration

- **Value / Values:** **1.5 sec**, Pick a number of seconds
- **Description:** This option only displays if the **Targeting Assistance** option is set to **On**. The amount of seconds a player will attempt to face their target after each ranged action.

##### Targeting Distance

- **Value / Values:** **1000 cm**, Pick an amount
- **Description:** This option only displays if the **Targeting Assistance** option is set to **On**. Determines the maximum distance targets can be from the player to be considered valid targets.

##### Targeting Distance When Aiming

- **Value / Values:** **1000 cm**, Pick an amount
- **Description:** This option only displays if the **Targeting Assistance** option is set to **On**. Determines the maximum distance targets can be from the player to be considered valid targets.

##### Targeting Angle

- **Value / Values:** **85°**, Pick a number of degrees
- **Description:** This option only displays if the **Targeting Assistance** option is set to **On**. From the player's facing direction, this is the angle within which targets must be to be considered valid targets.

##### Targeting Angle When Aiming

- **Value / Values:** **85°**, Pick a number of degrees
- **Description:** This option only displays if the **Targeting Assistance** option is set to **On**. From the player's facing direction, this is the angle within which targets must be to be considered valid targets.

##### Require Target Line of Sight

- **Value / Values:** **On**, Off
- **Description:** This option only displays if the **Targeting Assistance** option is set to **On**. Determines whether a clear line of sight is required for a target to be considered valid.

##### Require Target on Screen**

- **Value / Values:** On, **Off**
- **Description:** Determines whether or not a target has to be on screen in order for a target to be valid.

##### Base Weight Players

- **Value / Values:** **1.0**, Pick a number
- **Description:** This option only displays if the **Targeting Assistance** option is set to **On**. Determines the targeting prioritization assigned to players. If you select **0**, players cannot be targeted.

##### Base Weight Creatures

- **Value / Values:** **0.5**, Pick a number
- **Description:** This option only displays if the **Targeting Assistance** option is set to **On**. Determines the targeting prioritization assigned to creatures. If you select **0**, creatures cannot be targeted.

##### Base Weight Vehicles

- **Value / Values:** **0.3**, Pick a number
- **Description:** This option only displays if the **Targeting Assistance** option is set to **On**. Determines the targeting prioritization assigned to vehicles. If you select **0**, vehicles cannot be targeted.

##### Scale Weight by Distance

- **Value / Values:** **0.5**, Pick a number
- **Description:** This option only displays if the **Targeting Assistance** option is set to **On**. Scales the target's calculated priority weight, reducing the final value by the target's distance from the player.

##### Scale Weight by Angle

- **Value / Values:** **1**, Pick a number
- **Description:** This option only displays if the **Targeting Assistance** option is set to **On**. Scales the target's calculated priority weight, reducing the final value by the target's angle to the player.

##### Affects Team

- **Value / Values:** **Any**, Pick or enter a team
- **Description:** Determines which team is affected by this device.

##### Affects Class

- **Value / Values:** No Class, **Any**, Pick or enter a class
- **Description:** Determines which classes are affected by this device. **No Class** means only players with no assigned class are affected. **Any** means all players, including those with no assigned class, are affected.

##### Invert Team

- **Value / Values:** On, **Off**
- **Description:** If this is set to **On**, all teams are affected by this device except the team selected in the **Affects Team** option.

##### Invert Class

- **Value / Values:** On, **Off**
- **Description:** If this is set to **On**, all classes are affected by this device except the class selected in the **Affects Class** option.

##### Targetable Device in Edit Mode

- **Value / Values:** On, **Off**
- **Description:** Determines whether the device itself is targetable. If set to **On**, the device is only targetable when you are editing your island.

### Direct Event Binding

Following are the [direct event binding](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) options for this device.

#### Functions

A [function](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) listens for an event on a device then performs an action.

-
For any function, click the **option**, then **Select Device** to access and select from the **Device** dropdown menu.

-
Once you've selected a device, click **Select Event** and select the event that triggers this function.

-
If a function can be triggered by more than one event, press the **Add** button to add a line and repeat these steps.

**אפשרויות ותיאורים:**

##### Enable When Receiving From

Enables the device when an event occurs.

##### Disable When Receiving From

Disables the device when an event occurs.

##### Add to When Receiving From

Adds this device to the instigating player when an event occurs.

##### Add to All When Receiving From

Adds this device to all players when an event occurs.

##### Remove from When Receiving From

Removes this device from the instigating player when an event occurs.

##### Remove from All When Receiving From

Removes this device from all players when an event occurs.

#### Events

This device has no events.

### Use Third Person Controls In Verse

You can use the code below to control a Third Person Controls device in Verse. This code shows how to use events and functions in the Third Person Controls device API. Modify it to fit the needs of your experience.

using { /Fortnite.com/Devices }
using { /Verse.org/Simulation }
using { /UnrealEngine.com/Temporary/Diagnostics }
## A Verse-authored creative device that can be placed in a level
gameplay_controls_third_person_device_verse_example := class(creative_device):
 # Reference to the Gameplay Control: Third Person Device in the level.
 # In the Details panel for this Verse device,
 # set this property to your Gameplay Control: Third Person Device.
 @editable
 MyThirdPersonControlsDevice:gameplay_controls_third_person_device = gameplay_controls_third_person_device{}

Expand code Copy full snippet(22 lines long)

To use this code in your UEFN experience, follow these steps.

-
Drag a Third Person Controls device onto your island.

-
Create a new Verse device named **gameplay_controls_third_person_device_verse_example**. See [Create Your Own Device Using Verse](https://dev.epicgames.com/documentation/en-us/uefn/create-your-own-device-in-verse#creatinganewdevicewithverse) for steps.

-
In Visual Studio Code, open **gameplay_controls_third_person_device_verse_example.verse** in Visual Studio Code and paste the code above.

-
Compile your code and drag your Verse-authored device onto your island. See [Adding Your Verse Device to Your Level](https://dev.epicgames.com/documentation/en-us/uefn/create-your-own-device-in-verse#addingyourversedevicetoyourlevel) for steps.

-
Add a reference for the device on your island to your Verse device. See [Adding a Verse Reference to a Creative Device in Your Level](https://dev.epicgames.com/documentation/en-us/uefn/customize-verse-device-properties-in-verse#addingaversereferencetoacreativedeviceinyourlevel) for steps.

Disable the **Add to Players on Start** property of the Third Person Controls device so that only Verse will add the controls to the player.

-
Save your project and click **Launch Session** to playtest.

#### Third Person Controls API

See the [Gameplay Controls Third Person API Reference](https://dev.epicgames.com/documentation/en-us/uefn/verse-api/fortnitedotcom/devices/gameplay_controls_third_person_device) for more information on using the device in Verse.
