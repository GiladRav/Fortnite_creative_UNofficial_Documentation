# מטרות, התקדמות, ניקוד, Items ומשאבים

> **מטרת הקובץ:** לרכז פריטים, משאבים, איסוף, מטרות, Tracker, Timer, Stats, Score, Save Point וסיום משחק.  
> **מתי להשתמש בו:** כאשר בונים שרשרת משימה, מערכת התקדמות, כלכלה, איסוף או תנאי ניצחון.  
> **לא כלול:** HUD והודעות שאינן חלק ישיר ממערכת המטרה, וטעינת Level Instances.  
> **מקורות עיקריים:** `07D_מטרות_התקדמות_מדדים_וניקוד(1).md`, `08_Items_משאבים_ופריטי_משימה(1).md`

## תוכן עניינים

- [Using Capture Area Devices in Fortnite](#using-capture-area-devices-in-fortnite)
- [Using Capture Item Spawner Devices in Fortnite Creative](#using-capture-item-spawner-devices-in-fortnite-creative)
- [Using Carryable Spawner Devices in Fortnite](#using-carryable-spawner-devices-in-fortnite)
- [Using Collectibles Object Devices in Fortnite Creative](#using-collectibles-object-devices-in-fortnite-creative)
- [Using End Game Devices in Fortnite Creative](#using-end-game-devices-in-fortnite-creative)
- [Using Item Granter Devices in Fortnite Creative](#using-item-granter-devices-in-fortnite-creative)
- [Using Item Placer Devices in Fortnite Creative](#using-item-placer-devices-in-fortnite-creative)
- [Using Item Remover Devices in Fortnite Creative](#using-item-remover-devices-in-fortnite-creative)
- [Using Item Spawner Devices in Fortnite Creative](#using-item-spawner-devices-in-fortnite-creative)
- [Using Objective Devices in Fortnite Creative](#using-objective-devices-in-fortnite-creative)
- [Using Progress Based Mesh Devices in Fortnite](#using-progress-based-mesh-devices-in-fortnite)
- [Using Save Point Devices in Fortnite Creative](#using-save-point-devices-in-fortnite-creative)
- [Using Score Manager Devices in Fortnite Creative](#using-score-manager-devices-in-fortnite-creative)
- [Using Stat Counter Devices in Fortnite Creative](#using-stat-counter-devices-in-fortnite-creative)
- [Using Stat Creator Devices in Fortnite Creative](#using-stat-creator-devices-in-fortnite-creative)
- [Using Stat Powerup Devices in Fortnite Creative](#using-stat-powerup-devices-in-fortnite-creative)
- [Using Timed Objective Devices in Fortnite Creative](#using-timed-objective-devices-in-fortnite-creative)
- [Using Tracker Devices in Fortnite Creative](#using-tracker-devices-in-fortnite-creative)
- [Using Vending Machine Devices in Fortnite Creative](#using-vending-machine-devices-in-fortnite-creative)
- [Shove Gameplay Item in Fortnite](#shove-gameplay-item-in-fortnite)
- [Using Crafting Items in Fortnite Creative](#using-crafting-items-in-fortnite-creative)
- [Using Crystal Crafting Items in Fortnite Creative](#using-crystal-crafting-items-in-fortnite-creative)
- [Using Dino Egg Items in Fortnite Creative](#using-dino-egg-items-in-fortnite-creative)
- [Using Disguise Items in Fortnite Creative](#using-disguise-items-in-fortnite-creative)
- [Using Gold Items in Fortnite Creative](#using-gold-items-in-fortnite-creative)
- [Using Items in Fortnite Creative](#using-items-in-fortnite-creative)
- [Using Nature Items in Fortnite Creative](#using-nature-items-in-fortnite-creative)
- [Using Objective Items in Fortnite Creative](#using-objective-items-in-fortnite-creative)
- [Using Travel Items in Fortnite Creative](#using-travel-items-in-fortnite-creative)
- [Using World Resource Items in Fortnite Creative](#using-world-resource-items-in-fortnite-creative)

---
## Using Capture Area Devices in Fortnite

**כותרת מקורית:** Using Capture Area Devices in Fortnite  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/using-capture-area-devices-in-fortnite  
**מקור קלט:** `07D_מטרות_התקדמות_מדדים_וניקוד(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `using-capture-area-devices-in-fortnite`

###### Prerequisite topics

In order to understand and use the content on this page, make sure you are familiar with the following topics:

- [Getting Started with Devices](https://dev.epicgames.com/documentation/fortnite/getting-started-with-devices-in-fortnite)

The **Capture Area** device is a zone that can [trigger](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#trigger) effects once players enter or interact with it. It displays capture progress, uses visual effects to show when an area is being captured, and pulses when interacted with or captured.

You can configure the device to be captured by teams, grant score over time while controlled, or require players to deliver a specific item. Players typically interact by entering the area, but the device can also respond to item drop-off when configured.

### Using the Device

Depending on the options you customize, events can trigger when players enter the area or remain inside it for a set duration. For example:

-
The capture area can be used as an **item capture** device, such as for Capture the Flag games. When you drop an item onto the device in [Create mode](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#create-mode), the item can be set to require players to interact with this device.

-
The capture area can hold one item. If an item is held, the **Item Filter** option determines whether players need the item in question to interact with the device. You can drop a new item to replace the one currently in the device.

-
The capture area can be used as a **periodic scoring** device. While within the area, players can gain a certain amount of score for every defined time period.

-
The capture area can be used as a **control point** that is owned by a team and capturable by other teams. You can set how control of the area is gained and lost by teams.

**

If you're using multiple copies of a device on an island, you can [rename](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#rename-a-device) them for organization. Choosing names that relate to a device's purpose helps you to remember what each one does, and makes it easier to find a specific device when using the [Event Browser](https://dev.epicgames.com/documentation/fortnite/event-browser-in-fortnite-creative).

The general flow of using the device is as follows:

-
Place the device in your level.

-
Set the team ownership using Starting Team** and **Can be Captured By Team**.

-
Configure capture behavior using **Control Time**, **Neutralize Time**, and **Take Control Faster Per Player**.

-
Set up scoring using **Periodic Scoring**, **Periodic Scoring Time**, **Periodic Score Value**, and **Score on Taking Control**.

-
Configure player feedback using **Show in Objective HUB** and related visual options.

The capture area can have a floating [HUD](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#hud) marker that shows players where the Capture Area is. This can display the Capture Area's current status, such as its captured percentage, its letter designation (if it has one), and the team that owns the Capture Area.

-
Set when the device is active using** Enable During Phase** and **Capture Allowed on Game Start**.

For fundamentals on how to find, place, and customize a device, see [Getting Started with Devices](https://dev.epicgames.com/documentation/fortnite/getting-started-with-devices-in-fortnite).

Looking for a spark of creative freedom? See **[Down But Not Out Device Design Example](https://dev.epicgames.com/documentation/fortnite/down-but-not-out-device-design-examples-in-fortnite-creative)** to liberate your imagination!

### Device Options

In its [default](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#default) state, the capture area has no interaction. It requires setup before it can be used.
**

Default values are in **bold**. Values that trigger [contextual filtering](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#contextual-filtering) are in *italics*.

**אפשרויות, ערכים ותיאורים:**

##### Accent Color**

- **Value / Values:** **Aqua**, Pick a color
- **Description:** This option only displays if the **Accent Color Type** option is set to **Direct Color**. Determines the color of the capture area and the base.

##### Capture Radius

- **Value / Values:** **0.25**, Pick a size
- **Description:** Determines the radius of the capture area, in tiles.

##### Visible During Game

- **Value / Values:** **On**, Off
- **Description:** Determines whether the device is visible during the game. This affects its collision properties; if the device is not visible, it has no collision.

##### Item Filter

- **Value / Values:** **None**, Both, For Periodic Scoring, To Take Control
- **Description:** Determines when the player needs to have the item in the capture area.

##### Item Delivery Score

- **Value / Values:** **1**, Pick a score amount
- **Description:** The amount of score a player gains for an item being delivered to the area.

##### Periodic Scoring

- **Value / Values:** **Off**, Each Player, One Player Per Team, Owning Team
- **Description:** Determines if every player in the area gains score, or if only one player for each team gains score (if you are counting the score for a team game). You can also set it to provide score to the owning team even if there is not a player currently inside the area.

##### Score on Taking Control

- **Value / Values:** **0**, Pick a score amount
- **Description:** When a player or team gains control, they gain this score.

##### Count as Objective

- **Value / Values:** On, **Off**
- **Description:** Determines whether the capture area counts as an objective for a team. If set to **On**, the capture area can be used as an objective recognized by the **Objectives to End** option in the **Game** tab of the My Island settings. Setting this to** On** also means the** Scoreboard Win Condition** option in the **UI** tab of the My Island settings must be set to **Objectives**.

##### Show in Objective HUD

- **Value / Values:** On, **Off**
- **Description:** Determines whether the HUD shows the capture area and its current state along with other objectives. If this is set to **On**, it gives players an easy way to track which team owns each capture area.

##### Starting Team

- **Value / Values:** **All**, Pick a team
- **Description:** Which team owns the capture area at the start of the game. Can be used to determine who can interact with it (only friendlies or only enemies).

##### Accent Color Type

- **Value / Values:** **Direct Color**, Team Color, Team Relationship
- **Description:** Choose what determines the color of the capture area zone and base.** Direct Color** is the default; if you choose another value for this option, the **Accent Color** option will be hidden.

##### Capture Height

- **Value / Values:** **0.25**, Pick a size
- **Description:** Determines the height of the capture area, in tiles.

##### Item Visible In Game

- **Value / Values:** **On**, Off
- **Description:** Determines whether the device displays a hologram of the item during the game.

##### Consume Item on Scoring

- **Value / Values:** **On**, Off
- **Description:** Determines whether the item gets removed from the player's inventory when they get a score for being in the capture area. If not, the player gains a score but keeps the item.

##### Consume Item When Dropped

- **Value / Values:** **On**, Off
- **Description:** Determines whether the item gets consumed if a player drops it into the capture area. If the item is consumed when dropped, it means the player must hold it.

##### Can Receive Items From

- **Value / Values:** **Allies**, Hostiles, None, All, Pick a team
- **Description:** Only allows a specific team to drop off items to the capture area. This can be relationship-based. For example, by setting this option to Allies, you can require a team to capture the area before they can drop off items.

##### Can Be Used for Periodic Scoring By

- **Value / Values:** **Allies**, Hostiles, None, All, Pick a team
- **Description:** Only allows a specific team to use the capture area for periodic scoring. This can be relationship-based, so that only hostiles or the owning team can gain periodic scores.

##### Periodic Scoring Time

- **Value / Values:** **1 second**, Pick an amount of time
- **Description:** Sets how often the area provides score.

##### Periodic Score Value

- **Value / Values:** **1**, Pick a Score Amount
- **Description:** Set how much score is given during each period.

##### Enemies Contest Scoring

- **Value / Values:** On, **Off **
- **Description:** Determines which teams can capture the area. Allows for game modes where one team starts in control and needs to defend the area from the attacking team.

##### Can be Captured By Team

- **Value / Values:** **None**, All, Pick a team
- **Description:** Determines which teams can capture the area. Allows for game modes where one team starts in control and needs to defend the area from the attacking team.

##### Control Time

- **Value / Values:** **Instant**, Pick an amount of time
- **Description:** Determines how long a player needs to stand inside the area to gain control.

##### Neutralize Time Override

- **Value / Values:** **No Neutralization**, Instant, Pick an amount of time
- **Description:** This determines whether there is a period of time where an area is neutral (not controlled by any team) when an enemy team is capturing an area that is controlled by an opposing team. If set, the area must return to the neutral state before it can be controlled by the capturing team. There is an option to have no neutralization state, in which case the area transfers control directly from one team to another.

##### Take Control Faster Per Player

- **Value / Values:** **No Boost**, Pick a multiplier
- **Description:** Allows for the area to be captured faster if multiple players on the same team are within the area.

##### Take Control Faster While Emoting

- **Value / Values:** **No Boost**, Pick a multiplier
- **Description:** Allows for the area to be captured faster if the players in the area are [emoting](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#emote).

##### Progress Decay Type

- **Value / Values:** **No Decay**, Instant, Over Time
- **Description:** Determines whether the player needs to be carrying the correct item to capture the area or gain periodic score

##### Partial Progress Decay Speed

- **Value / Values:** **Instant**, No Decay, Pick a multiplier
- **Description:** If the team that has partially captured an area stops capturing, this determines how fast (as a percentage of the capture or neutralization speed) any partial progress decays.

##### Controlling Team Can Revert Partial Progress

- **Value / Values:** **On**, Off
- **Description:** If this is set to **Yes**, players on the team owning the area can reverse some of the progress of other teams by standing in the area.

##### Capture Allowed on Game Start

- **Value / Values:** **On**, Off
- **Description:** The area is either in a capturable or non-capturable state. This determines whether it is in the capturable state when the game starts. This differs from the enabled state, because in the enabled state the area is visible to players and appears on the HUD, but cannot be captured.

##### Enabled During Phase

- **Value / Values:** **Always**, None, Pre-Game Only, Gameplay Only, Create Only
- **Description:** Determines when the area is [enabled](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#enable). A disabled area is powered down, the capture zone is disabled, and only the device base is visible. It cannot be captured when disabled.

##### Display Control Progress VFX

- **Value / Values:** **On**, Off
- **Description:** Determines whether to show color changes on the area while the area is being captured by another team.

##### Display Ownership Change VFX

- **Value / Values:** **On**, Off
- **Description:** Determines whether the area shows a visual effect when a team gains ownership of the area.

##### Show Capture Progress on HUD

- **Value / Values:** On, **Off**
- **Description:** If set to **On**, a meter will display capture progress for all players in the area.

##### HUD Elements

- **Value / Values:** **None**, Badge, Beacon, Both
- **Description:** Determines if the HUD displays the Capture Area to the players. If you choose **Badge**, **Beacon**, or **Both** additional options are displayed.

##### Beacon

- **Value / Values:** Off, **Arrow**, Light Beam, Flare
- **Description:** This option only displays if the **HUD Elements** option is set to **Beacon** or **Beacon and Badge**. The beacon is a glowing particle effect that appears on the device. It has a number of different effects that can play.

##### Beacon Size

- **Value / Values:** **1.0X**, Pick a size
- **Description:** This option only displays if the **HUD Elements** option is set to **Beacon** or **Beacon and Badge**. Determines the size of the beacon above the objective.

##### Beacon Color

- **Value / Values:** **Friendly/Enemy**, Custom
- **Description:** Determines the color of the beacon. If you choose **Friendly/Enemy** the beacon will match the color of the team that holds the Capture Area. This option only displays if **HUD Elements** is set to **Beacon **or **Both**.

##### Beacon Color Picker

- **Value / Values:** **Blue**, Pick a color
- **Description:** This option only displays if the **Beacon Color** option is set to **Custom**. Choose a color for the beacon.

##### Requires Line of Sight

- **Value / Values:** **On**, Off
- **Description:** Determines whether direct line of sight is required to see the HUD icon. This option only displays if **HUD Elements** is set to **Badge** or **Both**.

##### Hostile Icon Text

- **Value / Values:** Enter text in the field
- **Description:** This option only displays if the HUD Elements option is set to Badge or Beacon and Badge. You can type text to be displayed on the HUD icon for hostile players. The text field is limited to 30 characters.

##### Hide HUD Icon At

- **Value / Values:** **20m**, Pick a distance
- **Description:** This option only displays if **HUD Elements** is set to** Badge** or **Beacon and Badge**. Determines the distance at which the HUD icon will stop being visible.

##### Icon Identifier

- **Value / Values:** **None**, Pick an icon
- **Description:** This option only displays if **HUD Elements** is set to **Badge** or **Beacon and Badge**. Select the icon to be displayed on the map or in-game.

##### Display Distance Text

- **Value / Values:** On, **Off**
- **Description:** This option only displays if **HUD Elements** is set to **Badge** or **Beacon and Badge**. When showing an icon as a HUD element, also display the distance between the associated object and the player.

##### Clamp to Screen

- **Value / Values:** On, **Off**
- **Description:** This option only displays if **HUD Elements** is set to **Badge** or **Beacon and Badge**. When showing an icon as a HUD element, the icon stays clamped to the screen.

##### Show Offscreen Arrow

- **Value / Values:** On, **Off**
- **Description:** This option only displays if the **Clamp to Screen** option is set to **Yes**. When showing as a HUD element, shows an arrow pointing in the offscreen direction when the actual rendering is offscreen.

##### Showing Owning Team Name

- **Value / Values:** On, **Off**
- **Description:** This option only displays if **HUD Elements** is set to **Badge** or **Beacon and Badge**. Determines whether the icon shows the name of the team which currently owns it. If you choose **No**, the HUD will simply show teams as Friendly/Neutral/Enemy.

##### Friendly Icon Text

- **Value / Values:** Enter text in the field
- **Description:** This option only displays if **HUD Elements** is set to **Badge** or **Beacon and Badge**. You can type text to be displayed on the HUD icon for Friendly players. The text field is limited to 30 characters.

##### Neutral Icon Text

- **Value / Values:** Enter text in the field
- **Description:** This option only displays if **HUD Elements** is set to **Badge** or **Beacon and Badge**. You can type text to be displayed on the HUD icon for Neutral players. The text field is limited to 30 characters.

##### HUD Text Size

- **Value / Values:** **1x**, Pick a size
- **Description:** This option only displays if **HUD Elements** is set to **Badge** or **Beacon and Badge**. Determines the size of the text, relative to the normal text size, that is displayed on the HUD icon.

##### Play Sound Alerts

- **Value / Values:** **On**, Off
- **Description:** If you choose **Yes**, sound alerts are played when players interact with the Capture Area.

##### Show Objective Pulse to Instigator Only

- **Value / Values:** **On**, Off
- **Description:** The Objective Pulse will only appear for the player who activated it. It will only disappear for the player who activated it.

##### Show Objective Pulse to Friendly Players

- **Value / Values:** **On**, Off
- **Description:** An Objective Pulse will appear to Friendly players indicating the location of the device in relation to the player.

##### Show Objective Pulse to Enemy Players

- **Value / Values:** **On**, Off
- **Description:** An Objective Pulse will appear to Enemy players indicating the location of the device in relation to the player.

##### Direction to Score

- **Value / Values:** **All**, Up, Down
- **Description:** Determines what direction the Capture Object needs to be moving in order to register a capture.

##### Object Scoring VFX Style

- **Value / Values:** **Default**, Confetti
- **Description:** Determines what type of VFX are displayed when a Capture Object is dropped and the score is registered. If you choose** Player Scoring**, an effect displays on the player; if you choose **Confetti**, a confetti cloud displays around the captured object.

##### Display Score Update on HUD

- **Value / Values:** On, **Off**
- **Description:** Determines if a player score event is displayed on the HUD.

##### HUD Message

- **Value / Values:** **Score!**, Enter a message
- **Description:** Message to display on the HUD with the score.

##### HUD Message Score Color

- **Value / Values:** **#BFEBFFFF**, Pick a color
- **Description:** Determines the color of the HUD message score. Click the swatch to open the Color Picker. Select the color swatch you want, then click the checkmark to close the Color Picker.

##### HUD Message Color

- **Value / Values:** **#00BAFFFF**, Pick a color
- **Description:** Determines the color of the HUD message. Click the swatch to open the Color Picker. Select the color swatch you want, then click the checkmark to close the Color Picker.

##### Reset HUD Message Score

- **Value / Values:** On,** Off**
- **Description:** When this device displays a score message on the HUD, should it start from 0.

##### Show Map Marker

- **Value / Values:** On, **Off**
- **Description:** Should the objective icon show on the Map / Minimap.

##### Sort Order

- **Value / Values:** **0**, Pick or enter a number
- **Description:** Determines the order in which objectives are listed in the HUD.

##### Use Spline Shape for Boundary

- **Value / Values:** On, **Off**
- **Description:** Whether to use a custom spline shape for the capture area boundary.

##### Spline Boundary Height Factor

- **Value / Values:** **1**, Pick or enter a number
- **Description:** Set the height for the spline shape used as the visual capture area boundary in relation to Capture Height.

##### Hide Base Mesh

- **Value / Values:** On,** Off**
- **Description:** Determine if the base mesh is hidden during the game.

### Functions and Events

For more information on how events and functions work, see [Using Devices](https://dev.epicgames.com/documentation/fortnite/using-devices-in-fortnite).

#### Functions

**אפשרויות ותיאורים:**

##### Enable When Receiving From

This function enables the device when an event occurs.

##### Disable When Receiving From

This function disables the device when an event occurs.

##### Allow Capture When Receiving From

This function allows capture of the area when an event occurs.

##### Disallow Capture When Receiving From

This function disallows capture of the area when an event occurs.

##### Give Control When Receiving From

This function gives control of the capture area to the instigating team when an event occurs.

##### Neutralize When Receiving From

This function sets ownership of the capture area to neutral when an event occurs.

##### Reset Team Control When Receiving From

This function resets control of the capture area to the original owning team when an event occurs.

##### Activate Objective Pulse When Receeivng From

This function creates an objective pulse pointing towards this capture area when an event occurs.

##### Deactivate Objective Pulse When Receivng From

This function deactivates an objective pulse pointing towards this capture area when an event occurs.

##### Toggle Enabled When Receiving From

This function toggles the device between enabled and disabled when an event occurs.

##### Toggle Capture Allowed When Receiving From

This function toggles between allowing and disallowing capture of area when an event occurs.

#### Events
**

Events in UEFN are read-only**. When you set a function on another device that binds to an event on this device, the events are set automatically but cannot be edited.

In Creative, you can link events to functions as well as functions to events.

**אפשרויות ותיאורים:**

##### On Item Is Consumed Send Event To

When the captured item is consumed, an event is sent to the selected device, which triggers the selected function.

##### On Item is Delivered Send Event To

When the captured item is delivered, an event is sent to the selected device, which triggers the selected function.

##### On Area Is Scored Send Event To

When the capture area awards score, an event is sent to the selected device, which triggers the selected function.

##### On Area Is Contested Send Event To

When the capture area becomes contested, an event is sent to the selected device, which triggers the selected function.

##### On Control Change Starts Send Event To

When a team begins to capture the area, an event is sent to the selected device, which triggers the selected function.

##### On Control Change Send Event To

When control of the capture area changes, an event is sent to the selected device, which triggers the selected function.

##### On Player Entering Zone Send Event To

When a player enters the capture area, an event is sent to the selected device, which triggers the selected function.

##### On Player Exiting Zone Send Event To

When a player exits the capture area, an event is sent to the selected device, which triggers the selected function.

##### On First Player Entering Zone Send Event To

When the first player enters the capture area, an event is sent to the selected device, which triggers the selected function.

##### On Last Player Exiting Zone Send Event To

When the last player exits the capture area, an event is sent to the selected device, which triggers the selected function.

### Capture Area Device API

To learn more about how the [Verse API Reference](https://dev.epicgames.com/documentation/fortnite/verse-api) works with your device in UEFN, see [Expand Device Functionality with the Verse API Reference](https://dev.epicgames.com/documentation/en-us/fortnite/getting-started-with-devices-in-fortnite#expanddevicefunctionalitywiththeverseapireference).

### Gameplay Examples and Island Tutorials Using Capture Areas

-
[Tug of War](https://dev.epicgames.com/documentation/fortnite/tug-of-war-in-fortnite-creative)

-
[Domination](https://dev.epicgames.com/documentation/fortnite/domination-gameplay-example-in-fortnite-creative)

-
[Capture the Flag](https://dev.epicgames.com/documentation/fortnite/build-a-capture-the-flag-in-unreal-editor-for-fortnite)

---

## Using Capture Item Spawner Devices in Fortnite Creative

**כותרת מקורית:** Using Capture Item Spawner Devices in Fortnite Creative  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/using-capture-item-spawner-devices-in-fortnite-creative  
**מקור קלט:** `07D_מטרות_התקדמות_מדדים_וניקוד(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `using-capture-item-spawner-devices-in-fortnite-creative`

The **Capture Item Spawner** is a special type of [item spawner](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) that will only [spawn](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) a single [item](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary).

With this device, you can restrict interaction with that item to a single team, send messages to players based on the state of the item, and transmit signals to other devices based on the state of the item. In this way, you can use an item as an objective.

The Capture Item Spawner holds only one item. Dropping a new item will replace the one currently in the device.

The device has a pulse effect when it is captured or interacted with, and shows current capture percentage on the capture area material. When starting to capture an area, an effect will play on the players that are capturing.

To find the Capture Item Spawner device, go to the Creative inventory and select the Devices tab. From there you can search or browse for the device. For more information on finding devices see [Finding and Placing Devices](https://dev.epicgames.com/documentation/fortnite/using-devices-in-fortnite).

### Device Options

In its default state, the Capture Item Spawner has no interaction. You need to [place](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) an item on the device before it can be used.

Once an item has been placed, it will spawn at the start of the game and relay messages to players when the item is picked up, dropped, or captured by a capture area.

#### Contextual Filtering

Some devices are affected by a feature called **contextual filtering**. This feature hides or displays options depending on the values selected for certain related options. This reduces clutter in the Customize panel and makes options easier to manage and navigate. To help identify them, values that trigger contextual filtering are in *italic*.

All options are listed, including those affected by contextual filtering; if they are hidden or displayed based on a specific option's value, there will be a note about it in the Description field for that option.

Default values are **bold**. Values that trigger contextual filtering are *italic*.

You can configure this device with the following options.

**אפשרויות, ערכים ותיאורים:**

##### Friendly Team

- **Value / Values:** **All**, Pick a team
- **Description:** The team that owns the area at the start of the game. Can be used to determine who can interact with it (only friendlies, or only enemies), and determines what messages are displayed if capture areas are [enabled](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary).

##### Captured By

- **Value / Values:** **Friendly Team**, Hostile Teams
- **Description:** Determines whether friendly teams need to pick up the item, or whether enemies need to pick it up.

##### Accent Color Type

- **Value / Values:** **Team Color**, *Direct Color*
- **Description:** Determines how the device should be colored.

##### Accent Color

- **Value / Values:** **Aqua**, Pick a color
- **Description:** Changes the device color to a specific color preset. *This option only appears if the **Accent Color Type** is set to **Direct Color***.

##### Score Value

- **Value / Values:** **0**, Pick a score amount
- **Description:** When capturing the item, a player gains this much score.

##### Return Dropped Items

- **Value / Values:** Instantly, **Never**, Pick an amount of time
- **Description:** If the item is dropped, it returns to the capture area after this defined amount of time.

##### Play Capture Sounds

- **Value / Values:** **On**, Off
- **Description:** Determines whether the item should play sound when it is captured.

##### Show Capture Messages

- **Value / Values:** **On**, Off
- **Description:** Prints messages to the chat when the item is dropped, captured, picked up, or returned.

##### Enabled At Game Start

- **Value / Values:** **Enabled**, Disabled
- **Description:** Determines whether the spawner is enabled at the start of the game. A disabled spawner is powered down, and will not spawn items.

##### Initial Weapon Ammo

- **Value / Values:** **Don't Override**, select a number from 1 to 999
- **Description:** Sets the amount of ammunition loaded in the weapon when granted, limited by the weapon's magazine size.

##### Spare Weapon Ammo

- **Value / Values:** **Default**, select a number from 1 to 999
- **Description:** Sets how much spare ammunition is added to the player's inventory when a weapon is granted. **Default** provides ammo based on the ammo type used by the weapon.

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

Enable the spawning of a capture item when an event occurs.

##### Disable When Receveing From

Disable the spawning of a capture item when an event occurs.

#### Events

An [event](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) tells another device when to perform a function.

-
For any event option, click the **option**, then **Select Device** to access and select from the **Device dropdown menu**.

-
Once you've selected a device, click **Select Function** to bind the timer to a function for that device.

-
If more than one device is affected by the function, press the **Add** button and repeat.

**אפשרויות ותיאורים:**

##### On Item Picked Up Send Event To

When an item is picked up, it sends an event to the selected device, which triggers the selected function.

##### On Item Dropped Send Event To

When an item is dropped, it sends an event to the selected device, which triggers the selected function.

##### On Item Is Returned Send Event To

Item is returned.

##### On Item Captured

When an item is captured, it sends an event to the selected device, which triggers the selected function.

---

## Using Carryable Spawner Devices in Fortnite

**כותרת מקורית:** Using Carryable Spawner Devices in Fortnite  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/using-carryable-spawner-devices-in-fortnite  
**מקור קלט:** `07D_מטרות_התקדמות_מדדים_וניקוד(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `using-carryable-spawner-devices-in-fortnite`

**
The Carryable Spawner** device can spawn carryable objects on your island. These carryable items can be picked up, carried, dropped, and thrown by players.

Carried items spawned by this device are clearly visible to other players (since they are carried above the head), and restrict the carrying player's movement. You can even set the carried item to explode on impact with a character, or when it collides with another object!

If you are using this device in UEFN, you can customize the mesh, the sound effect for the explosion, and the VFX for the explosion.

For help on how to find the **Carryable Spawner** device, see [Using Devices](https://dev.epicgames.com/documentation/fortnite/using-devices-in-fortnite).
**

If you're using multiple copies of a device on an island, it can be useful to rename them. Choosing names that relate to a device's purpose makes it easier to remember what each one does, and easier to find a specific device when using the [Event Browser](https://dev.epicgames.com/documentation/fortnite/event-browser-in-fortnite-creative)**.

### Using the Device

To use the Carryable Spawner device, follow this workflow.

-
Determine where you want to spawn the carryable object, and place the device.

-
Choose what object to spawn (if you are using custom meshes in UEFN).

-
Customize the options for spawning and respawning the object.

-
Customize the options that determine how players interact with the object, such as when it is dropped or whether players can jump while holding the object.

-
Customize the options for whether the carryable object can damage structures and world objects in the environment.

-
Customize the SFX and VFX (if you are using UEFN).

-
Start the game to playtest.

 Demonstration of how the Carryable item works for players

### Contextual Filtering in Creative

Some devices are affected by a feature called **contextual filtering**. This feature hides or displays options depending on the values selected for certain related options. This reduces clutter in the Customize panel and makes options easier to manage and navigate. To help identify them, values that trigger contextual filtering are in *italic*.

All options are listed, including those affected by contextual filtering; if they are hidden or displayed based on a specific option's value, there will be a note about it in the Description field for that option.

### Options

This section details the device options (in Creative) or user options (in UEFN).

-
To customize options in Creative, approach a device and press **E** to open the **Customize **panel.

-
To customize options in UEFN, select the device in your viewport or in the Outliner. Options for this device are found in the **Details **panel, in the **User Options** section.

**

Default values are bold**. Values that trigger contextual filtering are *italic*.

You can configure this device with the following options.

 Option Values Description
**Enabled at Game Start**

-
**Creative**: **On**, Off

-
**UEFN**: **True (checked)**, False (unchecked)

By default, this device is enabled when the game starts. If this is set to **Off (False)**, the device will only be enabled by event binding or Verse.

**Spawn Automatically**

-
Creative: *On*, Off

-
**UEFN**: **True (checked)**, False (unchecked)

By default, a carryable item spawns automatically when the device is enabled. In Creative, if this is set to **Off**, the Time Before First Spawn option is not displayed in the **Customize** panel.

**Time Before First Spawn**

**0.0**, Pick or enter an amount

In Creative, this option is only displayed if the **Spawn Automatically** option is set to **On**.

Determines how long it takes for the first item to spawn, in seconds.

**Respawn Automatically**

-
**Creative**: ***On***, Off

-
UEFN: True (checked), False (unchecked)

By default, items will respawn automatically after the previous spawned item explodes or despawns.

In Creative, if this is set to** Off**, the **Time Before Respawn** option is not displayed in the **Customize** panel.

**Time Before Respawn**

**5.0**, Pick or enter an amount

In Creative, this option is only displayed if the Respawn Automatically option is set to On.

Determines how long it takes for an item to respawn, in seconds.

**Carryable Takes Damage**

-
Creative: *On*, Off

-
**UEFN**: **True (checked)**, False (unchecked)

Determines if the carryable item can take damage.

In Creative, if this is set to **Off**, the **Carryable Starting Health** and **Show Health Bar** options are not displayed in the **Customize** panel.

**Carryable Starting Health**

**200**, Pick or enter an amount

In Creative, this option is only displayed if the **Carryable Takes Damage** option is set to **On**.

Determines how much health the spawned carryable item has.

**Show Health Bar**

-
Creative: *On*, Off

-
UEFN: True (checked), False (unchecked)

In Creative, this option is only displayed if the **Carryable Takes Damage** option is set to **On**.

Determines if a health bar is displayed for the carryable item.

**Can Be Thrown**

-
Creative: On, Off

-
**UEFN**: **True (checked)**, False (unchecked)

Determines whether the carryable item can be thrown by the player who is carrying it.

**Can Be Dropped**

-
**Creative**: **On**, Off

-
UEFN: True (checked), False (unchecked)

Determines whether the carryable item can be manually dropped by the player carrying it.

**Drop on Carrier Take Damage**

-
Creative: On, Off

-
**UEFN**: **True (checked)**, False (unchecked)

Determines whether the player carrying a spawned item will drop it when they take damage.

**Can Jump While Carrying**

-
**Creative**: **On**, Off

-
UEFN: True (checked), False (unchecked)

Determines whether a player can jump while they are carrying a spawned item (without dropping it).

If this is set to **Off**, a player carrying a spawned item will not be able to jump.

**Allow Friendly Fire Damage**

-
Creative: On, **Off **

-
**UEFN**: True (checked), **False (unchecked)**

Determines if everyone takes damage from impact or explosion of the carried item, even if they are on the carrying player's team.

**Impact Character Damage**

**20.0**, Pick or enter an amount

Determines how much damage to apply to a character (player or AI) hit by the carryable object.

Damage is scaled by impact magnitude. A thrown carryable object's velocity is always the same, but if you set the **Initial Spawn Velocity** to a value higher than 0, the object will do more damage when impacting a character, depending on the velocity you set.

**Impact Environmental Damage**

**50.0**, Pick or enter an amount

Determines how much damage to apply to structures and world objects that are hit by the carryable object.

 Damage is scaled by impact magnitude. A thrown carryable object's velocity is always the same, but if you set the **Initial Spawn Velocity** to a value higher than 0, the object could potentially do more damage when impacting the environment, depending on the velocity you set.

**Explode on Throw Impact**

Off, Someone, **Anything**

Determines if the carryable item explodes on impact with the first thing it hits after being thrown.

Values for this option:

-
**Off**: The carried item does not explode on impact after being thrown.

-
**Someone**: The carried item explodes on impact with players, AI characters, and driven vehicles.

-
**Anything**: The carried item explodes when it hits anything.

**Explode on Collision**

Off, Someone, **Anything**

Determines if the carried item will explode when it collides with something (aside from thrown impact).

Values for this option:

-
**Off**: The carried item does not explode on impact.

-
**Someone**: The carried item explodes on impact with players, AI characters, and driven vehicles.

-
**Anything**: The carried item explodes when it hits anything.

**Explosion Radius**

**5.0**, Pick or enter a number

Determines the radius of the explosion, in meters.

**Explosion Character Damage**

**25.0**, Pick or enter a number

Determines how much damage is taken by characters within the carried item's explosion area.

**Explosion Environmental Damage**

**100.0**, Pick or enter a number

Determines how much damage a carried item's explosion does to structures and world objects in its explosion area.

**Explosion Impulse**

**0.0**, Pick or enter a number

Determines how much an explosion launches characters away from the blast.

**Prevent Fall Damage from Knockback**

-
**Creative**: On, **Off**

-
**UEFN**: True (checked), **False (unchecked)**

By default, characters knocked back by an explosion will take fall damage. If this is set to **On (True)**, characters knocked back won't take fall damage. The fall damage amount is set in Island Settings, or can be overridden by certain devices.

**Explosion Check Line of Sight**

-
**Creative**: **On**, Off

-
**UEFN**: **True (checked)**, False (unchecked)

By default, the explosion will not hit characters who are not within line of sight of the blast. If this is set to **Off (False)**, anyone within the explosion area will be damaged and knocked back, even if they are not within line of sight of the blast.

**Explode on Enter Water**

-
**Creative**: **On**, Off

-
**UEFN**: **True (checked)**, False (unchecked)

By default, the carryable item will explode when it touches water (if it is not being carried). A carryable item that is being held will not explode when touching water.

**Initial Spawn Velocity**

**0.0**, Pick or enter a number

Determines the velocity applied to the carryable item when it spawns. By default, the item drops to the ground with no velocity.

**Initial Spawn Angle**

**0.0**, Pick or enter a number of degrees

Enter a number of degrees to define an angle.

By default, the carryable item spawns in the device's location. If the **Initial Spawn Velocity** option is set to a value higher than **0**, the spawned item will move in a random direction within the angle you define.

**Allowed Team**

**Any**, Pick or enter a team number

Determines which team is allowed to pick up carryable items spawned by this device.

**Invert Team Selection**

-
Creative: On, **Off **

-
**UEFN**: True (checked), **False (unchecked)**

If this is set to **On (True)**, all teams except the one selected in the **Allowed Team** option can pick up items spawned by this device.

**Allowed Class**

**Any**, Pick or enter a class number

Determines which class is allowed to pick up carryable items spawned by this device.

**Invert Class Selection**

-
**Creative**: On, **Off **

-
UEFN: True (checked), False (unchecked)

If this is set to **On (True)**, all classes except the one selected in the **Allowed Class** option can pick up items spawned by this device.

### UEFN-Specific Options

If you use this device in UEFN, the following additional user options are available.

**אפשרויות, ערכים ותיאורים:**

##### Custom Mesh

- **Value / Values:** Click the dropdown to select a mesh
- **Description:** You can add a custom mesh to the Carryable Spawner device, to replace the default mesh.

##### Custom Explode SFX

- **Value / Values:** Click the dropdown to select an audio sound effect
- **Description:** You can add a custom sound effect for the explosion of a carryable item, to replace the default explosion SFX.

##### Custom Explode VFX

- **Value / Values:** Click the dropdown to select a Niagara visual effect
- **Description:** You can add a custom explosion VFX system to replace the default explosion VFX.

---

## Using Collectibles Object Devices in Fortnite Creative

**כותרת מקורית:** Using Collectibles Object Devices in Fortnite Creative  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/using-collectibles-object-devices-in-fortnite-creative  
**מקור קלט:** `07D_מטרות_התקדמות_מדדים_וניקוד(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `using-collectibles-object-devices-in-fortnite-creative`

**
The **Collectibles Object** device provides a variety of collectible objects that you can use as **[economy drivers](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary)**, or [mediums of exchange](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary). You can also use these items as objectives that drive gameplay.

When used as an economy driver, these items can trigger item granting devices like the [Item Granter](https://dev.epicgames.com/documentation/fortnite/item-granter) when collected. Through item granting devices, you can offer usable items, weapons, or items like **[Gold](https://dev.epicgames.com/documentation/fortnite/using-gold-items-in-fortnite-creative)** whenever the collectible is picked up.

For example, whenever a player picks up a **Music Note**, it can trigger the player to collect a Boogie Bomb through the Item Granter.

You can also use the items from this device as a win condition through either points or item accumulation:

-
Change the **My Island > Game** settings for either **Collect Items to End** or **Score to End** to use collectible items as gameplay objectives.

-
To use the **Collect Items to End** setting, set the amount of items required to be collected. The first player or team to collect the required amount wins the game.

-
To use the **Score to End** setting, set the amount of score required to end the game. Then, set a score amount for each collectible item using the Collectible Object's Customize panel. The first team or player to reach the required score wins the game.

To find the Collectible Object device, press M to open the menu screen and select Content**. From there you can search or browse for the device. For more information on finding devices see [Using Devices](https://dev.epicgames.com/documentation/fortnite/using-devices-in-fortnite).

### Contextual Filtering

Some devices are affected by a feature called **contextual filtering**. This feature hides or displays options depending on the values selected for certain related options. This feature will reduce clutter in the Customize panel and make options easier to manage and navigate.

However, it may not be easy to recognize which options or values trigger contextual filtering. To help you identify them, in our device docs we use *italic* for any values that trigger contextual filtering. All options will be listed, including those affected by contextual filtering; if they are hidden or displayed based on a specific option's value, there will be a note about that in the Description field for that option.

### Device Options

By [default](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary), each collectible [object](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) will be visible to all players. When a player touches it, they gain a score of **1**, and the object disappears. The object is only hidden for players that have already picked it up. Other players will still see the collectible object and be able to pick it up.

You can configure this device with the following options.

Default values are **bold**. Values that trigger contextual filtering are *italic*.

**אפשרויות, ערכים ותיאורים:**

##### Collecting Team

- **Value / Values:** **All**, Pick or enter a team
- **Description:** Determines which team can pick up the item. If you choose **All**, it allows all teams to interact with the item.

##### Allowed Class

- **Value / Values:** No Class, **Any**, Pick or enter a class
- **Description:** Determines which class can pick up the item. If you choose **No Class**, only players who are not assigned a class can collect it. If you choose **Any**, all players with an assigned class can collect it.

##### Visible to Opposing Players

- **Value / Values:** **Never**, Always, Until Collected
- **Description:** Determines whether teams can see the item even if they can't collect it.

##### Visible on Game Start

- **Value / Values:** **On**, Off
- **Description:** Determines whether the item is visible and can be collected at the start of the game, or if it needs to be made visible by a [receiver](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary).

##### Show Pickup Effects

- **Value / Values:** Off, Only Audio, Only Visuals, **On**
- **Description:** Determines what effects will play when a player picks up the item. The default setting of **On** plays both audio and visual effects.

##### Display Score Update on HUD

- **Value / Values:** *On*, **Off**
- **Description:** Determines whether score updates are displayed as a HUD message. If you choose **On**, several additional options are displayed below this one.

##### Reset HUD Message Score

- **Value / Values:** **Off**, On
- **Description:** This option only displays if the **Display Score Update on HUD** option is set to **On**. When the device displays a score message on the HUD, this determines whether it starts at zero.

##### HUD Message

- **Value / Values:** **Score!**, Enter text
- **Description:** This option only displays if the **Display Score Update on HUD** option is set to **On**. Determines what message is displayed on the HUD with the score. Use the default, or enter custom text. The text field has a limit of 150 characters.

##### HUD Message Score Color

- **Value / Values:** **#BFEBFFFF**, Pick a color
- **Description:** This option only displays if the **Display Score Update on HUD** option is set to **On**. Determines the color of the score displayed on the HUD. Click the swatch to open the Color Picker. You can click to select a swatch, or enter a Hex code in the Search bar to find that color.

##### HUD Message Color

- **Value / Values:** **#00BAFFFF**, Pick a color
- **Description:** This option only displays if the **Display Score Update on HUD** option is set to **On**. Determines the color of the text in the message you set in the **HUD Message** option. Click the swatch to open the Color Picker. You can click to select a swatch, or enter a Hex code in the Search bar to find that color.

##### Collectible Color

- **Value / Values:** **None**, *Direct Color*, Collecting Team Color, Collecting Team Relationship, *Specific Team Color*, *Specific Team Relationship*
- **Description:** This option only displays if the **Display Score Update on HUD** option is set to **On**. For those objects that support it, you can choose a custom color for the object. If you choose the **Direct Color** option, the **Custom Color** option displays below this one. If you choose **Specific Team Color** or **Specific Team Relationship**, the the **Specific Team Index** option displays below this one.

##### Custom Color

- **Value / Values:** **White**, Pick a color
- **Description:** This option only displays if the **Collectible Color** option is set to **Direct Color**. Click the swatch to open the Color Picker. You can click to select a swatch, or enter a Hex code in the Search bar to find that color.

##### Specific Team Index

- **Value / Values:** Pick a team index number
- **Description:** This option only displays if the Collectible Color option is set to Specific Team Color or Specific Team Relationship. Determines which team is friendly for the purpose of coloring the collectible object.

##### Play Ambient VFX

- **Value / Values:** **On**, Off
- **Description:** Determines the visibility of the ambient glow effect on the collectible object.

##### Collectible Object

- **Value / Values:** Coin, Pick an object
- **Description:** Select the type of object players can collect. When you change to a new object, it will visually appear once you select OK.

##### Score

- **Value / Values:** 1, Pick or enter an amount
- **Description:** Determines how much score a player gets for collecting the item.

##### Ambient Audio

- **Value / Values:** On, Off
- **Description:** Determines whether the item plays ambient audio in the area around it. If audio plays, this is heard by players who haven’t collected the item yet.

##### Consume if Collected By

- **Value / Values:** Self, Anyone, Team
- **Description:** By default, each player is tracked individually, and the collectible will be visible to a player until they consume it. If you choose Anyone, any player can pick up the item. If you choose Team, only players on the team selected in the Collecting Team can pick up the item.

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

##### Turn Visibility On When Receiving From

Makes the collectible object visible when an event occurs.

##### Turn Visibility Off When Receiving From

Makes the collectible object invisible when an event occurs.

##### Respawn When Receiving From

Respawns the collectible object when an event occurs.

##### Respawn For All When Receiving From

Respawns collectible object for all players when an event occurs.

#### Events

Direct event binding uses events as transmitters. An event tells another device to perform a function.

-
For any event option, click the option, then Select Device to access and select from the Device dropdown menu.

-
Once you've selected a device, click Select Function to bind the event to a function for that device.

-
If more than one function is triggered by the event, press the Add button and repeat.

**אפשרויות ותיאורים:**

##### On Collected Send Event To

Sends an event to the selected device when a collectible object is picked up by a player.

### Gameplay Examples Using Collectible Object Devices

-
[Loo Roll Rush](https://dev.epicgames.com/documentation/fortnite/loo-roll-rush-in-fortnite-creative)

-
[Lava Bounce](https://dev.epicgames.com/documentation/fortnite/lava-bounce-gameplay-example-in-fortnite-creative)

---

## Using End Game Devices in Fortnite Creative

**כותרת מקורית:** Using End Game Devices in Fortnite Creative  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/using-end-game-devices-in-fortnite-creative  
**מקור קלט:** `07D_מטרות_התקדמות_מדדים_וניקוד(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `using-end-game-devices-in-fortnite-creative`

You can set the **End Game** device to end either the current [round](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) or the entire game, and determine which team met the conditions for the [win condition](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary).

This device can be activated by another device using [direct event binding](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary).

 To find the End Game device, see [Using Devices](https://dev.epicgames.com/documentation/fortnite/using-devices-in-fortnite).

If you're using multiple copies of a device on an island, it can be helpful to [rename](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) them. Choosing names that relate to a device's purpose makes it easier to remember what each one does, and easier to find a specific device when using the [Event Browser](https://dev.epicgames.com/documentation/fortnite/event-browser-in-fortnite-creative).

### Contextual Filtering

Some devices are affected by a feature called **contextual filtering**. This feature hides or displays options depending on the values selected for certain related options. This feature will reduce clutter in the Customize panel and make options easier to manage and navigate.

However, it may not be easy to recognize which options or values trigger contextual filtering. To help you identify them, in our device reference documents we use *italic* for any values that trigger contextual filtering. All options will be listed, including those affected by contextual filtering; if they are hidden or displayed based on a specific option's value, there will be a note about that in the Description field for that option.

### Device Options

This device has some basic functionality, like displaying custom victory callouts and determining which team wins the game as well as more advanced functions.

Default values are **bold**. Values that trigger contextual filtering are *italic*.

Use the options below to customize this device.

**אפשרויות, ערכים ותיאורים:**

##### What to End

- **Value / Values:** End Round, **End Game**
- **Description:** When activated, it determines whether the round ends or the entire game ends.

##### Winning Team

- **Value / Values:** **Winning Team**, Activating Team, Pick a team
- **Description:** Determines which team will win when the device is activated. Requires the selected team to have at least one player. Use the arrows to choose a team, or click in the field to type in a team number.

##### Custom Victory Callout

- **Value / Values:** Enter text
- **Description:** Enter a message to be displayed on victory or cooperative game end. The field has a 150-character limit.

##### Custom Defeat Callout

- **Value / Values:** Enter text
- **Description:** Enter a message to be displayed on the defeat screen. The field has a 150-character limit.

##### Game End Callout

- **Value / Values:** **You Win/Lose**, Placement, Cooperative
- **Description:** This determines what displays on the game-end screen. By default, it displays **You Win** or **You Lose**. If you choose **Cooperative**, everyone is shown the same game-end screen, which uses the sound selected in the **Victory Sound** setting and the text entered in the **Custom Victory Callout** setting.

##### Enabled at Game Start

- **Value / Values:** **Enabled**, Disabled
- **Description:** Determines if this device is enabled when the game is started.

##### Activating Team

- **Value / Values:** **Any**, Pick a team
- **Description:** Determines which team can activate the device. Use the arrows to choose a team, or click in the field to type in a team number.

##### Allowed Class

- **Value / Values:** No Class, **Any**, Pick a class
- **Description:** Determines which class can activate the device. Use the arrows to choose a class, or click in the field to type in a class number.

##### Post Game Type

- **Value / Values:** **Classic**, Battle Royale, *Custom*
- **Description:** **Classic** uses the Creative game-end screen. If you choose **Battle Royale**, your game uses the Fortnite Battle Royale game-end screen. If you choose **Custom**, more options display that you can use to customize the game-end screen.

##### Custom Show Scoreboard

- **Value / Values:** **Off**, On
- **Description:** Determines whether the scoreboard is displayed at the end of the game. This option only displays if you set the **Post Game Type** as **Custom**.

##### Custom Victory Animation Style

- **Value / Values:** **Lightning Bolts**, Pick a style
- **Description:** Determines the style used for the custom victory game-end animation. Only displays if **Post Game Type** is **Custom**.

##### Custom Victory Animation Color Set

- **Value / Values:** **Golden Yellow**, Pick a color
- **Description:** Determines the color set used for the custom Victory game-end animation. Only displays if **Post Game Type** is **Custom**.

##### Custom Victory Animation Text

- **Value / Values:** Enter text
- **Description:** Type in the text you want displayed at game-end for the ictory condition. The text field is limited to 15 characters. Only displays if **Post Game Type** is **Custom**.

##### Custom Victory Animation Sub Text

- **Value / Values:** Enter text
- **Description:** Type in [flavor text](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) displayed at game end for the victory condition. The text field is limited to 84 characters.

##### Custom Defeat Animation Style

- **Value / Values:** **Lightning Bolts**, Pick a style
- **Description:** Determines the style used for the custom defeat game-end animation.

##### Custom Defeat Animation Color Set

- **Value / Values:** **Golden Yellow**, Pick a color
- **Description:** Determines the color set used for the custom defeat game-end animation.

##### Custom Defeat Animation Text

- **Value / Values:** Enter text
- **Description:** Type in the text you want displayed at game end for the Defeat condition. The text field is limited to 15 characters.

##### Custom Defeat Animation Sub Text

- **Value / Values:** Enter text
- **Description:** Type in flavor text displayed at game end for the Defeat condition. The text field is limited to 84 characters.

##### Custom Tie Animation Style

- **Value / Values:** **Lightning Bolts**, Pick a style
- **Description:** Determines the style used for the custom tie game-end animation. Only displays if **Post Game Type** is **Custom**.

##### Custom Tie Animation Color Set

- **Value / Values:** **Golden Yellow**, Pick a color
- **Description:** Determines the color set used for the custom tie game-end animation. Only displays if **Post Game Type** is **Custom**.

##### Custom Tie Animation Text

- **Value / Values:** Enter text
- **Description:** Type in the text you want displayed at game end for the tie condition. The text field is limited to 15 characters. Only displays if **Post Game Type** is **Custom**.

##### Custom Tie Animation Sub Text

- **Value / Values:** Enter text
- **Description:** Type in flavor text to display at game end for the tie condition. The text field is limited to 84 characters. Only displays if **Post Game Type** is **Custom**.

### Direct Event Binding

Following are the [direct event binding](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) options for this device.

#### Functions

A [function](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) listns for an event on a device then performs an action.

-
For any function, click the **option**, then **Select Device** to access and select from the **Device** dropdown menu.

-
Once you've selected a device, click **Select Event** to bind the device to an event that will trigger the function for the device.

-
If more than one device or event triggers a function, click the **Add** button to add a line and repeat these steps.

**אפשרויות ותיאורים:**

##### Activate When Receiving From

Ends the round or game when an event occurs.

##### Enable When Receiving From

Enables the device when an event occurs.

##### Disable When Receiving From

Disables the device when an event occurs.

#### Events

This device has no events.

---

## Using Item Granter Devices in Fortnite Creative

**כותרת מקורית:** Using Item Granter Devices in Fortnite Creative  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/using-item-granter-devices-in-fortnite-creative  
**מקור קלט:** `07D_מטרות_התקדמות_מדדים_וניקוד(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `using-item-granter-devices-in-fortnite-creative`

The **Item Granter** device can automatically place items into player inventories during your game, or you can set conditions for manually placing items in player inventories.

You can determine what items are granted and when, and set other conditions by configuring the device using the options listed below. You can set whether to send an item to a player's inventory, or drop it near a player in-game. You can also use other devices to trigger the Item Granter.

To register items with the Item Granter, follow these steps.

-
In the Creative inventory, use the Weapons and Items tabs to find the items you want to register with the Item Granter. Click **EQUIP** to put them in your Player inventory.

-
Stand directly beside the Item Granter.

-
Press the **Tab** key to open the Creative inventory screen, then click **PLAY** to switch to the Player inventory screen.

-
Click the desired item, then press either **Z** or **X** to split or drop the item. You can also drag the item to the side until a [backpack icon](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#backpack-icon) appears.

When an item is registered with the Item Granter using the steps above, a hologram of the registered item will float above the device.

Like the [Item Spawner](https://dev.epicgames.com/documentation/fortnite/using-item-spawner-devices-in-fortnite-creative), this device is the recommended method of delivering [items](https://dev.epicgames.com/documentation/fortnite/using-items-in-fortnite-creative) and weapons to players in game.

The difference between the Item Spawner and the Item Granter is that the Item Spawner creates the [registered](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#register) item and drops it into the game world for players to pick up while the Item Granter automatically places the registered devices into the player's inventory.

**Looking for more inspiration?** See **[D-Launcher Device Design Examples](https://dev.epicgames.com/documentation/fortnite/dlauncher-device-design-examples-in-fortnite-creative)** to kick off your imagination!

To find the Item Granter device, go to the Creative inventory and select the Devices tab. From there you can search or browse for the device. For more information on finding devices see [Using Devices](https://dev.epicgames.com/documentation/fortnite/using-devices-in-fortnite).

If you're using multiple copies of a device on an island, it can be helpful to [rename](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#rename-a-device) them. You can choose names that relate to each device’s purpose, so it’s easier to remember what each one does.

### Device Options

The Item Granter has some basic functionality, like what item to grant to players, what to do with a player's existing inventory when granting an item, and whether to give a player extra ammo if the player is given a weapon. Additionally, there are some advanced options, like setting conditions for when a player is granted an item, if players from certain teams get different items, and how the items in the device are cycled.

#### Contextual Filtering

Some devices are affected by a feature called **contextual filtering**. This feature hides or displays options depending on the values selected for certain related options. This reduces clutter in the Customize panel and makes options easier to manage and navigate. To help identify them, values that trigger contextual filtering are in *italic*.

All options are listed, including those affected by contextual filtering; if they are hidden or displayed based on a specific option's value, there will be a note about it in the Description field for that option.

You can configure this device with the following options.

Default values are **bold**. Values that trigger contextual filtering are *italic*.

**אפשרויות, ערכים ותיאורים:**

##### Enabled on Game Start

- **Value / Values:** **Yes**, No
- **Description:** Determines whether or not the device is enabled when the game starts.

##### Receiving Players

- **Value / Values:** Triggering Team, **Triggering Player**, All, Pick a team
- **Description:** Determines which players receive the item.

##### On Grant Action

- **Value / Values:** **Clear Inventory**, Clear Items, Clear Resources, Keep All
- **Description:** Defines the action that occurs when the device grants an item to a player.

##### Grant

- **Value / Values:** **Current Item**, All Items
- **Description:** **Current Item**: Only the item selected on the device is granted to the player. **All Items**: All the items registered with the device are granted to the player.

##### Grant Condition

- **Value / Values:** **Always**, Only If Empty, Only If Space, Only If Not Owned
- **Description:** Only grants items to players that meet this condition.

##### Values for this option are:

- **Value / Values:** -
**Always**: Always grants items to players.
- **Description:** -
**Only If Empty**: Only grants items to players if their inventory is completely empty.

#### -
**Only If Space**: Only grants items to players if there is space in the player's inventory.

- **Value / Values:** -
**Only If Not Owned**: Only grants items to players if the item is not already in the player's inventory.
- **Description:** **Grant on Cycle**

##### **Yes**, No

- **Value / Values:** When the device cycles to a new item, it grants that new item to the player.
- **Description:** **Equip Granted Item**

##### **No**, *Yes*

- **Value / Values:** If the device gives items, equip the item listed. If **Yes** is selected, the **Item On Grant** option becomes available.
- **Description:** **Item to Grant**

##### **Item 1**, Pick an item number

- **Value / Values:** *This option only appears if **Equip Granted Item** is set to **Yes***. If the device gifts items, equip the item listed here. If you choose an item later than the number gifted, the last item will be equipped instead.
- **Description:** **Remove Item On Grant**

##### **No**, Yes

- **Value / Values:** When an item is granted, it is removed from the Item Granter.
- **Description:** **Initial Weapon Ammo**

##### **Don't Override**, select a number from 1 to 999

- **Value / Values:** Sets the amount of ammunition loaded in the weapon when granted, limited by the weapon's magazine size.
- **Description:** **Spare Weapon Ammo**

##### **Default**, select a number from 1 to 999

- **Value / Values:** Sets how much spare ammunition is added to the player's inventory when a weapon is granted. **Default** provides ammo based on the ammo type used by the weapon.
- **Description:** **Cycle Behavior**

##### **Stop**, Wrap

- **Value / Values:** Determines how the device cycles through the items registered to the device.
- **Description:** Values for this option are:

#### -
**Stop**: The device cannot cycle forward past the last item, or cycle backward past the first item.

- **Value / Values:** -
**Wrap**: When the device reaches the last item registered, it will cycle around to the first item.
- **Description:** **Grant while offline**

##### **No**, Yes

- **Value / Values:** If you choose **Yes** the device will continue granting items to players, even while they are not on the island.
- **Description:** **Drop Items at Player Location**

##### Never, Always, **If Inventory Full**

- **Value / Values:** Determines when an inventory item should be dropped at the player's location rather than place it in the player's inventory. If set to **Never**, the **Ownership of Dropped Item** option becomes hidden.
- **Description:** **Ownership of Dropped Item**

##### All, **Receiving Player**, Instigator

- **Value / Values:** Determines who can pick up a dropped item.
- **Description:** Values for this option are:

#### -
**All**: Any player can pick up the item.

- **Value / Values:** -
**Receiving Player**: Only the receiving player can pick up the item.
- **Description:** -
**Instigator**: Only the player who instigates the device can pick up the item.

##### Grant on Timer

- **Value / Values:** **Off**, Pick an amount of time
- **Description:** If this option is set to an amount of time, the device grants items to players every time that amount of time has passed.

##### Grant Time

- **Value / Values:** Pick a time
- **Description:** Grants an item at intervals based on time set.

##### Play Audio

- **Value / Values:** **No**, Yes
- **Description:** Determines whether the device plays audio effects.

##### Grant on Game Start

- **Value / Values:** **Off**, On
- **Description:** Set whether player gets the item at the start of the game.

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

##### Grant Item When Receiving From

Grants an item when an event occurs.

##### Cycle To Previous Item When Receiving From

The device cycles to the previous item when an event occurs.

##### Cycle To Next Item When Receiving From

The device cycles to the next item when an event occurs.

##### Cycle To Random Item When Receiving From

The device cycles to a random item when an event occurs.

##### Restock Items When Receiving From

If items have been removed from the device, the device is restocked with items when an event occurs.

##### Clear Save Data For Player When Receiving From

This option only works when the **Grant While Offline** is set to **Yes**. The instigating player no longer receives items when that player is offline.

#### Events

An [event](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#event) tells another device when to perform a function.

-
For any event option, click the **option**, then **Select Device** to access and select from the **Device dropdown menu**.

-
Once you've selected a device, click **Select Function** to bind the timer to a function for that device.

-
If more than one device is affected by the function, press the **Add** button and repeat.

**אפשרויות ותיאורים:**

##### On Item Granted Send Event To

When the device grants an item to a player, it sends an event to the selected device, which triggers the selected function.

### Gameplay Examples Using Item Granters

-
[Mazey Escape](https://dev.epicgames.com/documentation/fortnite/mazey-escape-in-fortnite-creative)

---

## Using Item Placer Devices in Fortnite Creative

**כותרת מקורית:** Using Item Placer Devices in Fortnite Creative  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/using-item-placer-devices-in-fortnite-creative  
**מקור קלט:** `07D_מטרות_התקדמות_מדדים_וניקוד(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `using-item-placer-devices-in-fortnite-creative`

The **Item Placer** device gives you a way to place weapons or [item](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) items in locations that are more realistic, as opposed to [Item Spawners](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#item-spawner) or chests that just drop items and weapons on the ground. You can drop an item or weapon onto the Item Placer to register it. The device acts as a container, but is shaped like the item registered. When a player interacts with the device, it grants the registered item to that player. If the device is mounted on a destructible object and that object is destroyed, the registered item drops to the ground. Destructible objects can include [props](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#prop), building pieces, and terrain, depending on the settings you have modified in [My Island](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) or in other devices.

To find the Item Placer device in Creative, see [**Using Devices**](https://dev.epicgames.com/documentation/fortnite/using-devices-in-fortnite-creative). To find the Item Placer in UEFN, open the Content Drawer and click **Fortnite > Devices > Item**.

If you're using multiple copies of a device on an island, it can be helpful to [rename](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#rename-a-device) them. Choosing names that relate to a device's purpose makes it easier to remember what each one does, and easier to find a specific device when using the [Event Browser](https://dev.epicgames.com/documentation/fortnite/event-browser-in-fortnite-creative).

### Contextual Filtering

Some devices are affected by a feature called **contextual filtering**. This feature hides or displays options depending on the values selected for certain related options. This reduces clutter in the Customize panel and makes options easier to manage and navigate. To help identify them, values that trigger contextual filtering are in *italic*.

All options are listed, including those affected by contextual filtering; if they are hidden or displayed based on a specific option's value, there will be a note about it in the Description field for that option.

### Device Options

This device has some basic functionality, like setting the interaction time and which teams or [classes](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#class) can interact with the device. Additionally, there are some advanced options, like inverting the class or team selection and determining whether the device is enabled when the game starts.

You can configure this device with the following options.

Default values are **bold**. Values that trigger contextual filtering are *italic*.

**אפשרויות, ערכים ותיאורים:**

##### Allow Interact

- **Value / Values:** ***On***, Off
- **Description:** Determines whether players can interact with this device. If this is set to **Off**, the **Interact Text**, **Interact Time**, **Allowed Team**, and **Allowed Class** options do not display.

##### Interact Text

- **Value / Values:** **Pick Up {item}**, Enter text
- **Description:** This text appears to players when they look at the item. The keyword **{item}** displays the name of the item that is registered with this device. The text field is limited to 150 characters. This option only displays if the **Allow Interact** option is set to **On**.

##### Interact Time

- **Value / Values:** **Instant**, Pick an amount of time
- **Description:** Determines how long the player must hold the interaction control in order to activate the device. Use the arrows to choose an amount of time, or click in the field to type in a number. This option only displays if the **Allow Interact** option is set to **On**.

##### Allowed Team

- **Value / Values:** None, **Any**, Pick a team
- **Description:** Determines which team can interact with the device. Click the arrows to choose, or click in the field to type in a number. This option only displays if the **Allow Interact** option is set to **On**.

##### Invert Team Selection

- **Value / Values:** **Off**, On
- **Description:** If you choose **On**, all teams except the one selected in the **Allowed Team** option can interact with the device.

##### Allowed Class

- **Value / Values:** No Class, **Any**, Pick a class
- **Description:** Determines which class can interact with the device. Click the arrows to choose, or click in the field to type in a number. If this is set to **No Class**, only players with no assigned class can interact with the device. This option only displays if the **Allow Interact** option is set to **On**.

##### Invert Class Selection

- **Value / Values:** **Off**, On
- **Description:** If you choose **On**, all classes except the one selected in the **Allowed Class** option can interact with the device.

##### Show Rarity Effects

- **Value / Values:** **On**, Off
- **Description:** Determines whether or not rarity effects for placed items are displayed when the device is enabled.

##### Play Audio

- **Value / Values:** **On**, Off
- **Description:** Determines whether the device plays audio effects.

##### Enabled at Game Start

- **Value / Values:** **Enabled**, Disabled
- **Description:** Determines whether the device is enabled when the game starts.

##### Allow Respawn

- **Value / Values:** **Off**, On
- **Description:** Determines whether the device can respawn.

##### Can Be Damaged at Game Start

- **Value / Values:** **Yes**, No
- **Description:** Determines whether the device can be damaged during the game.

##### Item Health

- **Value / Values:** **1**, Pick a number
- **Description:** If the device can be damaged, this determines the amount of health the device has. Click the arrows to choose, or click in the field to type in a number.

##### Allowed Class to Damage

- **Value / Values:** No Class, All, **Any**, Pick or enter a class number
- **Description:** Determines which class can interact with the device. Click the arrows to choose, or click in the field to type in a number.

##### Invert Class Selection to Damage

- **Value / Values:** **Off**, On
- **Description:** If you choose **On**, all classes except the one selected in the **Allowed Class to Damage** option can damage.

##### Allowed Team to Damage

- **Value / Values:** None, All, **Any**, Pick or enter a number
- **Description:** Determines which team can interact with the device. Click the arrows to choose, or click in the field to type in a number.

##### Invert Team Selection to Damage

- **Value / Values:** **Off**, On
- **Description:** If you choose **On**, all teams except the one selected in the **Allowed Team** option can damage.

##### Visual Style

- **Value / Values:** **Model**, Icon, Icon (Camera Facing)
- **Description:** Determines if the item is placed as its regular model or if it is placed as an icon.

##### Wood Cost of Item

- **Value / Values:** **No Cost**, Pick or enter a number
- **Description:** Determines how much the item costs in wood.

##### Metal Cost of Item

- **Value / Values:** **No Cost**, Pick or enter a number
- **Description:** Determines how much the item costs in metal.

##### Stone Cost of Item

- **Value / Values:** **No Cost**, Pick or enter a number
- **Description:** Determines how much the item costs in stone.

##### Gold Cost of Item

- **Value / Values:** **No Cost**, Pick or enter a number
- **Description:** Determines how much the item costs in gold.

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

##### Enable Device When Receiving From

This function enables the device when an event occurs.

##### Disable Device When Receiving From

This function disables the device when an event occurs.

##### Respawn Device When Receiving From

This function respawns the item when an event occurs.

##### Allow Damage When Receiving From

This function allows the device to take damage when an event occurs.

##### Disallow Damage When Receiving From

This function disallows the device to take damage when an event occurs.

#### Events

Direct event binding uses events as transmitters. An event tells another device to perform a function.

-
For any event option, click the **option**, then **Select Device** to access and select from the **Device dropdown menu**.

-
Once you've selected a device, click **Select Function** to bind the event to a function for that device.

-
If more than one function is triggered by the event, press the **Add** button and repeat.

**אפשרויות ותיאורים:**

##### On Item Dropped Send Event To

When the device drops an item, it sends an event to the selected device, which triggers the selected function.

##### On Item Granted Send Event To

When the device grants an item, it sends an event to the selected device, which triggers the selected function.

##### On Item Respawned Send Event To

When the device respawns an item, it sends an event to the selected device, which triggers the selected function.

---

## Using Item Remover Devices in Fortnite Creative

**כותרת מקורית:** Using Item Remover Devices in Fortnite Creative  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/using-item-remover-devices-in-fortnite-creative  
**מקור קלט:** `07D_מטרות_התקדמות_מדדים_וניקוד(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `using-item-remover-devices-in-fortnite-creative`

The **Item Remover** gives gives you the ability to designate events in your games that will cause players to [drop](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#drop) or lose items from their [inventory](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#inventory). For example, if a player is [Down But Not Out](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#down-but-not-out), they could drop items from their inventory, and other players could then pick up those items.

To find the Item Remover device, see **[Using Devices](https://dev.epicgames.com/documentation/fortnite/using-devices-in-fortnite)**.

**Looking for more inspiration?** See the [Item Remover Device Design Example](https://dev.epicgames.com/documentation/fortnite/item-remover-device-design-example-in-fortnite-creative) to kick off your imagination!

If you're using multiple copies of a device on an island, it can be helpful to [rename](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#rename-a-device) them. Choosing names that relate to a device's purpose makes it easier to remember what each one does, and easier to find a specific device when using the [Event Browser](https://dev.epicgames.com/documentation/fortnite/event-browser-in-fortnite-creative).

### Contextual Filtering

Some devices are affected by a feature called **contextual filtering**. This feature hides or displays options depending on the values selected for certain related options. This reduces clutter in the Customize panel and makes options easier to manage and navigate. To help identify them, values that trigger contextual filtering are in *italic*.

All options are listed, including those affected by contextual filtering; if they are hidden or displayed based on a specific option's value, there will be a note about it in the Description field for that option.

### Device Options

You can configure this device with the following options.

Default values are **bold**. Values that trigger contextual filtering are *italic*.

**אפשרויות, ערכים ותיאורים:**

##### Enabled During Phase

- **Value / Values:** None, **All**, Pre-Game Only, Gameplay Only
- **Description:** Determines the [phases](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#game-phase) in which the device is enabled. **Pre-Game** includes all phases that occur before the game starts.

##### Affected Objects

- **Value / Values:** All Objects, Building Materials, World Resources, **Objects in Device**, Weapons and Items, Weapons, Items
- **Description:** Determines what items in the player's inventory are considered for removal.

##### Amount to Remove

- **Value / Values:** **Amount in Device**, *Percentage*
- **Description:** Determines the amount of affected items that are removed from the player. If you choose **Percentage**, an additional option displays.

##### Percentage to Remove

- **Value / Values:** **100%**, Pick a percentage
- **Description:** This option only displays if the **Amount to Remove** option is set to **Percentage**. Determines the percentage of a player's affected items that are removed.

##### Removal Method

- **Value / Values:** **Remove Items**, Drop Items, Drop Items On Previous Ground Location
- **Description:** Determines how items are removed. If you choose **Remove Items**, the items are removed from the player's inventory. If you choose **Drop Items**, the player's items drop and other players can pick them up.

##### Remove All Variations of the Selected Item

- **Value / Values:** **Off**, On
- **Description:** When turned on, all variations and rarities of the selected item will be removed from the player.

##### Allowed Team

- **Value / Values:** **Any**, Pick a team
- **Description:** Determines which team can activate the device.

##### Allowed Class

- **Value / Values:** No Class, **Any**, Pick a class
- **Description:** Determines which [class](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#class) can activate the device. If you choose **No Class** only players without an assigned class can activate the device. If you choose **Any**, all players can activate it.

##### Apply To

- **Value / Values:** **Player**, Players of Team, Players of Class, All Players
- **Description:** Determines which players have items removed from their inventory.

##### Play Audio

- **Value / Values:** **On**, Off
- **Description:** Determines whether the device plays a sound when items are removed.

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

##### Remove When Receiving From

This function removes items from a player when an event occurs.

#### Events

This device has no events.

---

## Using Item Spawner Devices in Fortnite Creative

**כותרת מקורית:** Using Item Spawner Devices in Fortnite Creative  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/using-item-spawner-devices-in-fortnite-creative  
**מקור קלט:** `07D_מטרות_התקדמות_מדדים_וניקוד(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `using-item-spawner-devices-in-fortnite-creative`

This is a device that creators can use to create a [spawn point](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#spawning) for various [Items](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#item), and to assign specific items to each spawn location.

The **Item Spawner** is one of several devices in Creative that spawns items — in this case, spawning them just above the location of the device.

To find the Item Spawner device, go to the Content Browser and select the Devices category. From there you can search or browse for the device. For more information on finding devices, see [Using Devices](https://dev.epicgames.com/documentation/fortnite/using-devices-in-fortnite).

It’s helpful to [customize device names](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#rename-a-device) when you use multiple copies of the same device.

### Device Options

This device has some basic functionality, like how much time passes between item spawns, and which classes can pick up spawned items. Additionally, there are some advanced options, such as setting a resource cost for spawned items.

The default state of the Item Spawner when it is first placed is Inactive.

#### Contextual Filtering

Some devices are affected by a feature called contextual filtering. This feature hides or displays options depending on the values selected for certain related options. This feature will reduce clutter in the Customize panel and make options easier to manage and navigate.

However, it may not be easy to recognize which options or values trigger contextual filtering. To help you identify them, in our device docs we use italic for any values that trigger contextual filtering. All options will be listed, including those affected by contextual filtering; if they are hidden or displayed based on a specific option’s value, there will be a note about that in the Description field for that option.

Default values are **bold**.

You can configure this device with the following options.

**אפשרויות, ערכים ותיאורים:**

##### Items Respawn

- **Value / Values:** **On**, Off
- **Description:** Determines whether the device will keep the items in the list after they are spawned, or whether items are removed from the list when spawned. If you choose **Off**, If this is disabled, the device will eventually run out of items and be unable to spawn more.

##### Random Spawns

- **Value / Values:** **Off**, Random, No Repeats
- **Description:** This option controls randomized spawning. If you choose **No Repeats**, the device randomly spawns every item in the device once before repeating an item.

##### Base Visible During Games

- **Value / Values:** **On**, Off
- **Description:** Determines whether the device is visible to player during the game.

##### Spawn Item On Timer

- **Value / Values:** **On**, *Off*
- **Description:** Set to specify how much time before an item spanws. When the option is set to **Off**, the **Time Before First Spawn** option is hidden.

##### Time Before First Spawn

- **Value / Values:** Never, Instant, **10 seconds**, Pick an amount of time
- **Description:** After the game starts, this is how much time must pass before the device spawns an item.

##### Respawn Item On Timer

- **Value / Values:** **On**, *Off*
- **Description:** Use Time Between Spawns to specify how much time to wait before spawning the next item. When set to **Off**, the **Time Between Spawns** option is hidden.

##### Time Between Spawns

- **Value / Values:** Never, Instant, **10 seconds**, Pick an amount of time
- **Description:** This is how much time passes between one item spawn and the next one.

##### Wood [Cost of Item](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary)

- **Value / Values:** **No Cost**, Pick an amount
- **Description:** How much wood the item costs.

##### Stone Cost of Item

- **Value / Values:** **No Cost**, Pick an amount
- **Description:** How much stone the item costs.

##### Metal Cost of Item

- **Value / Values:** **No Cost**, Pick an amount
- **Description:** How much metal the item costs.

##### Gold Cost of Item

- **Value / Values:** **No Cost**, Pick an amount
- **Description:** How much gold the item costs.

##### Initial Weapon Ammo

- **Value / Values:** **Don't Override**, select a number from 1 to 999
- **Description:** Sets the amount of ammunition loaded in the weapon when granted, limited by the weapon's magazine size.

##### Spare Weapon Ammo

- **Value / Values:** **Default**, select a number from 1 to 999
- **Description:** Sets how much spare ammunition is added to the player's inventory when a weapon is granted. **Default** provides ammo based on the ammo type used by the weapon.

##### Run Over Pickup

- **Value / Values:** *On*, **Off**
- **Description:** Determines the size of the item displayed.

##### Allow Spawning When Blocked

- **Value / Values:** Yes, **No**
- **Description:** Only displayed when **Run Over Pickup** is set to **On**. Determines if an item can spawn even when a player blocks the spawner.

##### Initial Movement of Item

- **Value / Values:** None, **Gravity**, Toss
- **Description:** Initial movement of item spawned. **None**: Item is not tossed or falls on spawn. **Gravity**: Item falls on spawn. **Toss** Item is tossed on spawn.

##### Item Scale

- **Value / Values:** **1x**, Pick a size
- **Description:** By default, the items are displayed at normal size. You can choose to make the display larger so that items are more visible.

##### Enabled At Game Start

- **Value / Values:** **Yes**, No
- **Description:** By default, the device is enabled when the game starts. If you want to set conditions for enabling the device, set this option to **No**.

##### Continuously Spawn Items

- **Value / Values:** On, **Off**
- **Description:** Determines whether the device continues spawning items even if the previous items have not been picked up. Use with caution, as this can result in large numbers of items spawning in a single location if combined with other options such as **Items Respawn**, or **Time Between Spawns**. The last item spawned is tracked by the device, but the rest are left in the world and are not cleaned up if the device is disabled, or if **Cycle to Next Item** is [called](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#call).

##### Allowed Team

- **Value / Values:** **Any**, Pick a team
- **Description:** Only players on this team are allowed to pick up items spawned by this device.

##### Invert Team

- **Value / Values:** **No**, Yes
- **Description:** **No:** The chosen team is the only one that cannot activate the device. **Yes:** The chosen team is the only one that can activate the device.

##### Affects Team

- **Value / Values:** All But Selected, **Only Selected**
- **Description:** If you choose **All But Selected**, anyone can pick up spawned items except players on the team selected in **Allowed Team**. If you choose **Only Selected**, only players on the team selected in **Allowed Team** can pick up spawned items.

##### Allowed Class

- **Value / Values:** No Class, **Any**, Pick a class
- **Description:** Determines which class is allowed to pick up an item spawned by this device. If you choose **No Class**, only players without an assigned class can pick up items spawned by this device.

##### Invert Class

- **Value / Values:** **No**, Yes
- **Description:** **No:** The chosen class is the only one that cannot activate the device. **Yes:** The chosen classis the only one that can activate the device.

##### Affects Class

- **Value / Values:** All But Selected, **Only Selected**
- **Description:** If you choose **All But Selected**, anyone can pick up spawned items except players assigned the class selected in **Allowed Class**. If you choose **Only Selected**, only players assigned the class selected in **Allowed Class** can pick up spawned items.

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

##### Enable When receiving From

Enables the device when an event occurs.

##### Disable Device When Receiving From

Disables the device when an event occurs.

##### Cycle to Next Item When Receiving From

Cycles the time spawner to the next item when an event occurs.

##### Spawn Item When Receiving From

Spawns an item from the item spawner when an event occurs.

#### Events

An [event](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#event) tells another device when to perform a function.

-
For any event option, click the **option**, then **Select Device** to access and select from the **Device dropdown menu**.

-
Once you've selected a device, click **Select Function** to bind the timer to a function for that device.

-
If more than one device is affected by the function, press the **Add** button and repeat.

**אפשרויות ותיאורים:**

##### On Item Pick Up Send Event To

When a player picks up the items, it sends an event to the selected device, which triggers the selected function.

### Design Examples

Here is an example of how you can use the Item Spawner device.

#### Continuous Item Spawning

To have items spawn nonstop after an event, combine an Item Spawner with a Switch.

**Devices used**:

-
1 x **Item Spawner**

-
1 x [**Switch**](https://dev.epicgames.com/documentation/fortnite/using-switch-devices-in-fortnite-creative)

-
Place an **Item Spawner** and drop as many items as you would like near the device to register them. Customize it to the following settings:

 Option Value Description
Random Spawns

Random

Each time the Item Spawner spawns an item, a random item from the device’s registered items will be spawned.

Base Visible During Game

Off

The base will not be visible during gameplay.

Time Before First Spawn

1 Second

After being enabled, there will be a 1 second delay before the Item Spawner begins to spawn items.

Time Between Spawns

Instant

There will be no delay between item spawns.

Enabled At Game Start

No

The Item Spawner will not begin enabled and will not spawn items until it is enabled.

Continuously Spawn Items

On

The Item Spawner will continue to spawn items regardless of whether or not they have been picked up.

-
Place a **Switch** and customize it to the following settings:

 Option Value Description
Device Model

Antique Lever

The Switch will appear as an Antique Lever in game.

-
Set the direct event bindings of the Switch to the following:

 Function Device Event Description
On Turned On Send Event To

ItemSpawner

Enable

When the Switch is turned on, the Item Spawner will begin spawning items.

On Turned Off Send Event To

ItemSpawner

Disable

When the Switch is turned off, the Item Spawner will stop spawning items.

Here’s an overview of how devices communicate in this Design Example:

 Device A Function Device B Event Explanation
**ItemSpawner**

Enable

**Switch**

On Turned On Send Event To

When the Switch is turned on, the Item Spawner will begin spawning items.

**ItemSpawner**

Disable

**Switch**

On Turned Off Send Event To

When the Switch is turned off, the Item Spawner will stop spawning items.

You now have the basic functionality for continuously spawning items.

This is a very effective technique to create rewards and sources of power for players. Try using different gameplay devices to enable the Item Spawner and begin the flow of items. Use a [Trigger](https://dev.epicgames.com/documentation/fortnite/using-trigger-devices-in-fortnite-creative) to start the spawning when a player enters a room, or try connecting a [Guard Spawner](https://dev.epicgames.com/documentation/fortnite/guard-spawner-device) so that the player will be rewarded after eliminating a guard.

Adjust the **Time Between Spawns** setting to find the spawn frequency that best fits your game mode.

### Gameplay Examples Using Item Spawners

-
[Mazey Escape](https://dev.epicgames.com/documentation/fortnite/mazey-escape-in-fortnite-creative)

-
[Shooting Gallery](https://dev.epicgames.com/documentation/fortnite/shooting-gallery-in-fortnite-creative)

---

## Using Objective Devices in Fortnite Creative

**כותרת מקורית:** Using Objective Devices in Fortnite Creative  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/using-objective-devices-in-fortnite-creative  
**מקור קלט:** `07D_מטרות_התקדמות_מדדים_וניקוד(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `using-objective-devices-in-fortnite-creative`

The **Objective Device** provides a collection of destructible devices that you can select from to use as [objectives](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#objective) in your game.

You can also control various features like how many [health points](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#hp) (HP) a device has, and how many points the player gets for destroying it.

An Objective device has optional [particle effects](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#particle-effect) and a [HUD marker](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#hud-marker) that displays its state. It also can provide [HUD messages](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) to all players as it takes damage.

If the **Objectives to End** option under **Island Settings > Round > End Condition** is set to **1**, the player or team that destroys the Objective device will win the game.

For information on finding devices, see [****](https://dev.epicgames.com/documentation/fortnite/using-devices-in-fortnite-creative)**[Using Devices](https://dev.epicgames.com/documentation/fortnite/using-devices-in-fortnite)**.

### Contextual Filtering

Some devices are affected by a feature called **contextual filtering**. This feature hides or displays options depending on the values selected for certain related options. This feature will reduce clutter in the Customize panel and make options easier to manage and navigate.

However, it may not be easy to recognize which options or values trigger contextual filtering. To help you identify them, in our device docs we use *italic* for any values that trigger contextual filtering. All options will be listed, including those affected by contextual filtering; if they are hidden or displayed based on a specific option's value, there will be a note about that in the Description field for that option.

### Device Options

Each device in the gallery has a default value of 100 HP, is set as an objective for all players, and uses a HUD marker for any player who gets within 5 tiles (25.6 meters) of it.

You can configure this device with the following options.

Default values are **bold**. Values that trigger contextual filtering are *italic*.

 Option Value Description
**Mesh**

**Shocktower**, Burgerhead, Tomatohead, Satellite Dish, Server Rack, Single Bed, Arctic Base Transmitter, Sphere, Cylinder, Cube

Choose the type of objective device you want to use.

**Invulnerable**

On, ***Off***

Determines if the objective device can take damage. If this is set to **Off**, the **Health** option is displayed below this option.

**Owning Team**

**None**, Pick or enter a team

Determines the team that will defend the Objective. The HUD Marker will appear blue for this team, and it will appear as a Defend if you are using the Objective HUD. By default, every team is attacking the device.

**Health**

**100**, Pick an amount, Invulnerable

Determines how many health points the device has. Set it to maximum health if you want to use events to destroy it, or if you want the device to be destroyed another way, such as with explosive barrels.

**Blast Radius**

**No Explosion**, Pick a distance

You can set the device to explode when it is destroyed. When it does this, the device will destroy everything within the selected blast radius.

**Beacon**

**Off**, *Arrow*, *Light Beam*, *Flare*

Determines if a beacon displays to mark the objective item. If a beacon is displayed, this determines the shape of the beacon that shows players the objective's location. If you choose one of the beacon shapes, the **Beacon Color** option displays.

**Beacon Color**

***Color***, Team Relationship

This option only displays if you have selected a beacon shape in the **Beacon** option. This determines whether the beacon has a custom color or if it uses team colors. If you select **Color**, the **Custom Beacon Color** option displays below this one.

**Custom Beacon Color**

**#5995FFFF**, Pick a color

Determines the color of the beacon. Click the swatch to open the Color Picker. You can click to select a swatch, or enter a Hex code in the Search bar to find that color.

**Beacon Scale**

**No Scaling**, 0.25 Extra Small, 0.5 Small, 1.0 Medium, 2.0 Large, 4.0 Extra Large

If there is a beacon, this determines how large the beacon is. By default, the objective device has no scaling.

**Friendly Badge Visibility**

Hidden, **Within Distance**, Always Show

Whether the badge for the objective device is shown to friendly players.

**Hostile Badge Visibility**

Hidden, **Within Distance**, Always Show

Whether the badge for the objective device is shown to hostile players.

**Badge Visibility Distance**

**25M**, Pick or enter an amount

This determines the distance at which players will see the health bar of the objective device, if the **Friendly Badge Visibility** or **Hostile Badge Visibility** options are set to **Within Distance**.

**Show Badge On Damage**

**No**, *Friendlies*, *Hostiles*, *All*

Determines whether the badge is shown when the objective device takes damage, regardless of what is set for the **Friendly Badge Visibility** or **Hostile Badge Visibility** options. If this option is not set to **No**, the **Show on Damage Duration** option is shown below this one.

**Show on Damage Duration**

**10S**, Pick or enter an amount of time

If the badge is shown when the objective device is damaged, this determines how long it is shown.

**Clamp to Screen**

On, **Off**

Determines whether the badge is always shown within the screen.

**Show in Objective HUD**

**Objective Identifier**

**None**, Pick an icon

You can select an icon from the Icon Library Picker by scrolling through the library, or by typing a word into the Search bar. The selected icon displays in the Objective HUD widget and distinguishes this device from other Objective devices.

**Custom Objective Text**

Enter text

You can enter customized text that is attached to the objective and is shown in the HUD. The text field is limited to 12 characters. If this field is left empty, the HUD displays the name of the **Objective Identifier** icon.

**Display Damage Numbers**

**On**, Off

When the objective item takes damage, this determines whether floating damage numbers are displayed over it.

**Visible During Games**

**On**, Off

Determines whether the device is visible during a game.

**Show Destroy Messages**

On, **Off**

When the device takes damage or is destroyed, this determines whether a HUD Message displays.

**Critical Notification Threshold**

**None**, 5%, 10%, 25%

If **Show Destroy Messages** is set to **On**, a HUD message is displayed when the selected threshold of critical damage is reached.

**Warning Notification Threshold**

**None**, 35%, 50%, 75%

If **Show Destroy Messages** is set to **On**, a HUD message notifies players that the objective item is being damaged when the selected threshold of damage is reached.

**Play Audio/VFX**

**On**, Off

Determines whether the device plays audio/VFX when it takes damage.

**Score**

**0**, Pick an amount

When destroyed, the Objective device provides the selected amount of score to the player or team that destroys it.

**Collision During Games**

Off, **On**, Only when Visible

Determines whether the Objective has collision properties. If you choose **Only When Visible**, you can turn off the objective item's visibility and players will not bump into it.

**Collides With**

**Everything**, Weapons Only

Defines the collision profile of this device. It can be set to collide only with weapons, so that the device can take damage but doesn't restrict player movement.

**Show Objective Pulse to Instigator Only**

**Yes**, No

If set to **Yes**, the objective pulse will only appear or disappear for the player who activated it.

**Show Objective Pulse to Friendly Players**

**Yes**, No

If set to **Yes**, the objective pulse will appear to Friendly players and it indicates the location of the device in relation to the player.

**Show Objective Pulse to Enemy Players**

**Yes**, No

If set to **Yes**, the objective pulse will appear to Enemy players and it indicates the location of the device in relation to the player.

**Display Score Update on HUD**

**Off**, *On*

Determines whether score updates are displayed as a HUD message. If you choose **On**, several additional options are displayed below this one in the Customize panel.

**Reset HUD Message Score**

**Off**, On

When the device displays a score message on the HUD, this determines whether it starts at zero.

**HUD Message**

**Score!**, Enter text

Determines what message is displayed on the HUD with the score. Use the default, or enter custom text. The text field has a limit of 150 characters.

**HUD Message Score Color**

**#BFEBFFFF**, Pick a color

Determines the color of the score displayed on the HUD. Click the swatch to open the Color Picker. You can click to select a swatch, or enter a Hex code in the Search bar to find that color.

**HUD Message Color**

**#00BAFFFF**, Pick a color

Determines the color of the text in the message you set in the **HUD Message** option. Click the swatch to open the Color Picker. You can click to select a swatch, or enter a Hex code in the Search bar to find that color.

**Damage Event Cooldown**

**0S**, Pick an amount

Determines how often the **On Damaged** event can activate.

### UEFN-Only Device Options

The following options are only available when using the VFX Spawner inside UEFN.

 Option Value Explanation
**Custom Mesh**

Select a custom mesh for the objective item.

This option allows you to replace the existing objective items with your own custom mesh.

**Custom Badge UI**

Select or create a custom Badge UI

This option allows you to create or select a custom Badge UI.

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

##### Destroy when Receiving From

This function destroys the objective device when an event occurs.

##### Turn on Visibility when Receiving From

Makes the objective device visible when an event occurs.

##### Turn Off Visibility when Receiving From

Makes the objective device invisible when an event occurs. This will also hide its HUD marker.

##### Activate Objective Pulse When Receiving From

Activates and objective pulse at the player's location when an event occurs.

##### Deactivate Objective Pulse When Receiving From

Deactivates the objective pulse at the player's location when an event occurs.

##### Set Invulnerable When Receiving From

Sets the objective device to be invulnerable when an event occurs.

##### Set Damageable When Receiving From

Sets the objective device to be damageable when an event occurs.

##### Reset Health When Receiving From

Resets the objective device's health to maximum when an event occurs.

#### Events

Direct event binding uses events as transmitters. An event tells another device to perform a function.

-
For any event option, click the **option**, then **Select Device** to access and select from the **Device dropdown menu**.

-
Once you've selected a device, click **Select Function** to bind the event to a function for that device.

-
If more than one function is triggered by the event, press the **Add** button and repeat.

**אפשרויות ותיאורים:**

##### On Destroyed Send Event To

When the objective device is destroyed, an event is sent to the selected device, triggering the selected function.

##### On Damaged Send Event To

When the objective device is damaged, an event is sent to the selected device, triggering the selected function.

---

## Using Progress Based Mesh Devices in Fortnite

**כותרת מקורית:** Using Progress Based Mesh Devices in Fortnite  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/using-progress-based-mesh-devices-in-fortnite  
**מקור קלט:** `07D_מטרות_התקדמות_מדדים_וניקוד(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `using-progress-based-mesh-devices-in-fortnite`

###### Prerequisite topics

In order to understand and use the content on this page, make sure you are familiar with the following topics:

- [Getting Started with Devices](https://dev.epicgames.com/documentation/fortnite/getting-started-with-devices-in-fortnite)

**
The Progress Based Mesh** device provides the option to create a visual system for the progress of an item. The device can swap between meshes and materials to visually represent different stages. The default mesh is a jar with a liquid material to show filling and draining.

You can use the device to simulate players placing objects inside other objects, track the progress of an event, and more. The device options and use cases change between Fortnite Creative and Unreal Editor for Fortnite (UEFN). To learn more, see the [Using the Device](https://dev.epicgames.com/documentation/fortnite/using-progress-based-mesh-devices-in-fortnite#using-the-device) section on this page.

### Using the Device

The device creates a visual representation of progress. You can use buttons, triggers, and receivers for players to interact with the device.

If you're using multiple copies of a device on an island, you can rename them for organization. Choosing names that relate to a device's purpose helps to remember what each one does, and finding a specific device when using the [Event Browser](https://dev.epicgames.com/documentation/fortnite/event-browser-in-fortnite-creative).

The general flow of using the device is as follows:

-
Place the device into your level.

-
Set the[ progression values](https://dev.epicgames.com/documentation/fortnite/using-progress-based-mesh-devices-in-fortnite#user-options).

-
Create a [threshold list of meshes](https://dev.epicgames.com/documentation/fortnite/using-progress-based-mesh-devices-in-fortnite#visuals-nbsp) (predefined in Creative).

-
Trigger the [device's functions](https://dev.epicgames.com/documentation/fortnite/using-progress-based-mesh-devices-in-fortnite#direct-event-binding), or set the value directly in [Verse](https://dev.epicgames.com/documentation/fortnite/using-progress-based-mesh-devices-in-fortnite#verse-api) (UEFN only) to activate the threshold meshes.

-
Add [visual and sound effects](https://dev.epicgames.com/documentation/fortnite/using-progress-based-mesh-devices-in-fortnite#additional-uefn-options-nbsp) (UEFN only).

 For fundamentals on how to find, place, and customize a device, see Getting Started with Devices.

#### Creative

In Creative, the Progress Based Mesh devices come with a predefined list of threshold meshes that are not configurable.

You can adjust the options around the progression values, functions, and events. The material for the device is dynamic, meaning you can rotate the jar, and the liquid physically moves with it.

#### UEFN

In UEFN, you can use the default or custom meshes to create a mesh sequence. The default jar behaves the same as in Creative.
**

You can't change the static mesh from the component. You must use the [Threshold Mesh](https://dev.epicgames.com/documentation/fortnite/using-progress-based-mesh-devices-in-fortnite#visuals-nbsp) option to add meshes. When the progress of the device changes, the static mesh component updates with the active threshold mesh.

You can build a range of mechanics like:

-
Growing or decaying plants in a garden

-
The filling and draining of fuel tanks

-
Progress bar for players' rank in a game

-
Tip jar for your restaurant tycoon

The device also writes its progression state to the mesh's material via a FillAmount** scalar material parameter. You can create your own materials using this parameter to get smooth transitions. This parameter becomes active through the **Fill Material Index** in the [Visuals](https://dev.epicgames.com/documentation/fortnite/using-progress-based-mesh-devices-in-fortnite#visuals-nbsp) category of the device.

The index represents the material slot attached to your static mesh. For the fundamentals of working with materials, see [Materials in UEFN](https://dev.epicgames.com/documentation/fortnite/materials-in-unreal-editor-for-fortnite).

To assign the material index:

-
In a new or existing material, create a **ScalarParameter** node.

-
Set the **Parameter Name** to **FillAmount**. You must use this name for the device to register the **Fill Material Index**.

-
Connect the node as needed in the material graph.

-
Assign the material to your static mesh.

-
In the **Threshold Mesh** list, set the **Fill Material Index** to the material slot containing the **FillAmount** parameter. Only one material slot per mesh supports the fill parameter.

To view and adjust the material slots, open the mesh in the Static Mesh Editor and use the Details panel.

[
](https://dev.epicgames.com/community/api/documentation/image/20c5d622-158c-4550-8266-3a0deed7ff59?resizing_type=fit) Progress Bar Material

### Contextual Filtering

Some devices are affected by a feature called contextual filtering. This feature hides or displays options depending on the values selected for certain related options. This organization reduces clutter in the Details panel, helping to manage and navigate the settings. To identify these options, values that trigger contextual filtering in the settings tables on this page are in italic.

All options are listed in the following sections, including those affected by contextual filtering. If an option is hidden or displayed based on a specific value, there will be a note about it in the **Description** field of the table for that option.

### Device Options

The core options for the device are the target value for complete progress and the rate of progression.

You can configure this device with the following options. Default values are bold. Values that trigger contextual filtering are italic.

Option

Value

Description

**Progress Target**

**100**, choose a value

The maximum progress for the device to reach.

Value ranges from 0 - 100.

**Game Start Progress Amount**

**0**, choose a value

The amount of progress the device has at the start of the game.

Value ranges from 0 - 100.

**Progress Rate**

**5**, choose a value

The rate at which to increase the progress amount based on the **Progression Type**.

If set to continuous, it's the rate at which progress changes. If set to instant rate, it's how much to change by per event call.

Value ranges from 0 - 100.

**Regress Rate**

**5**, choose a value

The rate at which to decrease the progress amount based on the **Progression Type**.

If set to continuous, it's the rate at which progress changes. If set to instant rate, it's how much to change by per event call.

Value ranges from 0 - 100.

**Progression Type**

**Continuous Rate**, Instant

Options for how the progress amount updates.

-
**Instant Rate:** Gains a single chunk of the Progress or Regress Rate at once.

-
**Continuous Rate:** Updates at the specific Progress or Regress Rate per second.

### Functions and Events

For more information on how events and functions work, see [Getting Started with Devices](https://dev.epicgames.com/documentation/fortnite/getting-started-with-devices-in-fortnite).

#### Functions

 Functions Description
**Begin Progressing When Receiving From**

Increases the current progress level by the **Progress Rate** user option.

**Begin Regressing When Receiving From**

Reduces the current progress level by the **Regress Rate** user option.

**Pause When Receiving From**

Pauses the device.

**Progress Fully**

Increases the device to its **Progress Target**.

**Regress Fully**

Reduces the **Progress Target** to 0.

#### Events
**

Events in UEFN are read-only. When you set a function on another device that binds to an event on this device, the events are set automatically but cannot be edited.

In Creative, you can link events to functions as well as functions to events.

 Events Description
On Progress Filled Completely**

Event that occurs when the device reaches its **Progress Target**.

O**n Progress Emptied Completely**

Event that occurs when the device regresses to 0.

**On Progress Changed**

Event that occurs when the current progress of the device changes.

**Progress Threshold Cross Event**

Event that occurs when the device hits one of the mesh thresholds, and a mesh is swapped in response.

 UEFN-Only Options

#### Visuals

Use the **Visuals** category to adjust the appearance of the mesh and materials at different thresholds. The default value is the jar mesh at different fill stages.

 Visual Options Value Description
**Threshold Mesh**

*Index*

Represents the list of meshes for the stages of progression.

To add meshes to the list, click the plus (**+**) icon.

**Threshold**

Minimum (Min)

Maximum (Max)

Sets the progress range (the bound) for the mesh to be active.

Use the following options to determine how the set min and max values are included in the range.

-
**Exclusive:** Excludes the set value.

-
**Inclusive (Default):** Includes the set value.

-
**Open:** Uses the whole range, from the set value to the **Progress Target**.

**

If two thresholds overlap, the device uses the first qualifying threshold in the list.

Static Mesh**

Choose a Static Mesh Asset

Sets the mesh for the threshold range. The mesh that the device will show while its progress value falls between that threshold.

**Transition VFX**

Choose a Niagara System

Simulates the visual effect (VFX) when the device transitions into the set static mesh.

**Transition Sound Cue**

Choose a Sound Cue Asset

Plays the sound when the device transitions into the set static mesh.

**Fill Material Index**

**2**, choose a number

Creates a dynamic material instance for the material in this slot, and writes to the **FillAmount** scalar material parameter.

This material parameter for the current fill is expressed as a ratio of Current Progress / Progress Target. For example, if your target progress is 100 vs 50, but you have a current progress of 25, then you'll get 1/4 full vs 1/2 full. To disable the functionality, set the value to -1.
**

You must use a ScalarParameter** node in the material, and rename it to **FillAmount**.

#### Audio

With **Continuous Rate** active, you can add audio to indicate the progress.

 Audio Type Description
**Progress Audio**

Plays audio when the device is progressing at a continuous rate.

**Regress Audio**

Plays audio when the device is regressing at a continuous rate.

**Finish Audio**

Plays audio when the device reaches its **Progress Target**.

The following general categories are included in the Details panel:

-
HLOD

-
Displacement

-
Rendering

-
Draw Distance

-
Data Layers

To learn more about the panel, see [User Interface Reference](https://dev.epicgames.com/documentation/fortnite/user-interface-reference-for-unreal-editor-for-fortnite).

### Verse API

You can use the Verse API for the Progress Based Mesh device to customize your further mechanics. In Verse, you can directly set the progress amount. When coupled with triggers and receivers, you can configure pre-determined progress and regression amounts.

For more information on using the device in Verse, see the progress_based_mesh_device API reference.

---

## Using Save Point Devices in Fortnite Creative

**כותרת מקורית:** Using Save Point Devices in Fortnite Creative  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/using-save-point-devices-in-fortnite-creative  
**מקור קלט:** `07D_מטרות_התקדמות_מדדים_וניקוד(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `using-save-point-devices-in-fortnite-creative`

###### Prerequisite topics

In order to understand and use the content on this page, make sure you are familiar with the following topics:

- [Getting Started with Devices](https://dev.epicgames.com/documentation/fortnite/getting-started-with-devices-in-fortnite)

The **Save Point** device provides a way for creators to add elimination tracking persistence, inventory and resource tracking across multiple game sessions, and more.

Think of it as saving a snapshot of where the player is at any given time.

For example:

-
In racing games, players can track their best lap times.

-
In adventure games, players can save their progress toward objectives.

-
In skillrun games, players can pick up where they left off instead of having to start over every time they leave the game and come back.

If players are on an island using Save Point devices when a new version of that island is published, those players can continue their session and their progress will be saved. However, if a player matchmakes into an older, non-current version of an island, a HUD message displays stating that the island is not current, their save data will not be loaded, and their save game will not be modified.

To find the Save Point device, see [Using Devices](https://dev.epicgames.com/documentation/fortnite/getting-started-with-devices-in-fortnite).

### Contextual Filtering

Some devices are affected by a feature called **contextual filtering**. This feature hides or displays options depending on the values selected for certain related options. This reduces clutter in the Customize panel and makes options easier to manage and navigate. To help identify them, values that trigger contextual filtering are in *italic*.

All options are listed, including those affected by contextual filtering; if they are hidden or displayed based on a specific option's value, there will be a note about it in the Description field for that option.

### Device Options

This device has some basic functionality, like autosaving and saving checkpoint data. Additionally, there are some advanced options, like saving a player's shield and health data.

You can configure this device with the following options.

Default values are **bold**. Values that trigger contextual filtering are *italic*.

**אפשרויות, ערכים ותיאורים:**

##### Enabled During Phase

- **Value / Values:** None, **Gameplay Only**
- **Description:** Determines whether the device is enabled during a specific [game phase](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary).

##### Auto Save

- **Value / Values:** **Yes**, No
- **Description:** Determines whether the player's data is automatically saved while they play.

##### Auto-Load

- **Value / Values:** **Yes**, No
- **Description:** Determines whether to autoload the player's data. If this is set to **Yes**, the **Auto-Load Behavior** option displays below. If it is set to **No** that option does not display.

##### Auto-Load Behavior

- **Value / Values:** **Initial Spawn**, Game Start, Round Start, Every Spawn
- **Description:** Determines when the player's saved data is loaded.

##### Save Health and Shields

- **Value / Values:** Yes, **No**
- **Description:** Determines whether the player's health and shield data is saved.

##### Save Loadout

- **Value / Values:** **Yes**, No
- **Description:** Determines whether the player's current loadout is saved.

##### Save Full Ammo Magazines

- **Value / Values:** **Yes**, No
- **Description:** Restores full ammo magazines on loading player data. If **No**, restores the exact amount of ammo the player had when saving.

##### Save Resources

- **Value / Values:** **Yes**, No
- **Description:** Determines whether the player's current resources are saved.

##### Save Gold

- **Value / Values:** **Yes**, No
- **Description:** Determines whether the player's current gold is saved.

##### Save Scoreboard Stats Behavior

- **Value / Values:** Round, Career, **Both**
- **Description:** This determines what kind of scoreboard stats are saved. Values are:

#### -
**Round**: Only the current round's scoreboard stats are saved between rounds.

- **Value / Values:** -
**Career**: Only the player's career scoreboard stats are saved.
- **Description:** -
**Both**: Both the current round's stats and the player's career stats are saved.

##### Save All Scoreboard Stats

- **Value / Values:** No, **Yes**, Only If Lower, Only If Higher
- **Description:** Determines whether the device saves all of the player's current stat data that appears on the scoreboard.

##### Save Score

- **Value / Values:** No, **Yes**, Only If Lower, Only If Higher
- **Description:** Determines whether the player's current score data is saved.

##### Save Round Wins

- **Value / Values:** No, **Yes**, Only If Lower, Only If Higher
- **Description:** Determines whether the player's current round wins are saved.

##### Save Eliminations

- **Value / Values:** No, **Yes**, Only If Lower, Only If Higher
- **Description:** Determines whether the player's current eliminations count is saved.

##### Save Assists

- **Value / Values:** No, **Yes**, Only If Lower, Only If Higher
- **Description:** Determines whether the player's current assists count is saved.

##### Save Collected Items

- **Value / Values:** **Yes**, Only If Lower, Only If Higher, No
- **Description:** Determines whether the player's collected items are saved.

##### Save Creature Eliminations

- **Value / Values:** **Yes**, Only If Lower, Only If Higher, No
- **Description:** Determines whether the player's current creature eliminations count is saved.

##### Save Checkpoint

- **Value / Values:** **Yes**, No
- **Description:** Determines whether the player's [checkpoint](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) data is saved. If set to **Yes**, the player will [respawn](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) at the last checkpoint they activated.

##### Save Player Location

- **Value / Values:** **Yes**, No
- **Description:** Determines whether the player's location is saved. If set to **Yes**, the player will respawn at the last position they saved.

##### Save Team

- **Value / Values:** Yes, **No**
- **Description:** Determines whether the player's team number is saved. If set to **Yes**, the player will load with that team assigned, [triggering](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) any related Team Settings & Inventory device.

##### Save Class

- **Value / Values:** **Yes**, No
- **Description:** Determines whether the player's [class number](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) is saved. If set to **Yes**, the player will load with that class assigned, triggering the related [Class Designer](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) device.

##### Allow Player to Clear Data

- **Value / Values:** Yes, **No**
- **Description:** Determines whether players can clear their progress data from the Game (Sidebar) menu.

### Direct Event Binding System

**Direct event binding** allows devices to communicate directly, which makes your workflow more intuitive, and gives you more freedom to focus on your design ideas.

Below are the functions and events for this device.

#### Functions

A [function](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) listens for an event on a device then performs an action.

-
For any function, click the **option**, then **Select Device** to access and select from the **Device** dropdown menu.

-
Once you've selected a device, click **Select Event** to bind the device to an event that will trigger the function for the device.

-
If more than one device or event triggers a function, press the **Add** button to add a line and repeat these steps.

**אפשרויות ותיאורים:**

##### Save Player When Receiving From

This function saves player data when an event occurs.

##### Load Player When Receiving From

This function loads player data when an event occurs.

##### Enable When Receiving From

This function enables the device when an event occurs.

##### Disable When Receiving From

This function disables the device when an event occurs.

##### Clear Data for Player When Receiving From

This function clears player data when an event occurs.

##### Clear Data for All Players When Receiving From

This function clears all player data when an event occurs.

##### Save All Players When Receiving From

This function saves data for all players when an event occurs.

##### Load All Players When Receiving From

This function loads data for all players when an event occurs.

#### Events

Direct event binding uses events as transmitters. An event tells another device to perform a function.

-
For any event option, click the **option**, then **Select Device** to access and select from the **Device** dropdown menu.

-
Once you've selected a device, click **Select Function** to bind this event to a function for that device.

-
If more than one function is triggered by the event, click the **Add** button to add a line and repeat these steps.

**אפשרויות ותיאורים:**

##### On Activation Send Event To

When the device is activated, it sends an event to the selected device, which triggers the selected function.

##### On Player Loaded Send Event To

When a player's save data is loaded, the device sends an event to the selected device, which triggers the selected function.

##### On Cleared Send Event To

When a player clears data, the device sends an event to the selected device, which triggers the selected function.

---

## Using Score Manager Devices in Fortnite Creative

**כותרת מקורית:** Using Score Manager Devices in Fortnite Creative  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/using-score-manager-devices-in-fortnite-creative  
**מקור קלט:** `07D_מטרות_התקדמות_מדדים_וניקוד(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `using-score-manager-devices-in-fortnite-creative`

With the **Score Manager** device, creators can manipulate scores using triggers. By using channel messages, the Score Manager can communicate with a variety of devices. Creators can use this to award scores in many ways, creating many varieties of gameplay.

For help on how to find the **Score Manager** device, see [Using Devices](https://dev.epicgames.com/documentation/fortnite/using-devices-in-fortnite).

If you're using multiple copies of a device on an island, it can be useful to [rename](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#rename-a-device) them. Choosing names that relate to a device's purpose makes it easier to remember what each one does, and easier to find a specific device when using the Event [Browser](https://dev.epicgames.com/documentation/fortnite/event-browser-in-fortnite-creative).

### Contextual Filtering

Some devices are affected by a feature called **contextual filtering**. This feature hides or displays options depending on the values selected for certain related options. This feature will reduce clutter in the Customize panel and make options easier to manage and navigate.

However, it may not be easy to recognize which options or values trigger contextual filtering. To help you identify them, in our device docs we use *italic* for any values that trigger contextual filtering. All options will be listed, including those affected by contextual filtering; if they are hidden or displayed based on a specific option's value, there will be a note about that in the Description field for that option.

### Device Options

In its default state, the Score Manager does nothing. It must be activated by receiving a signal from a specific channel.

You can configure this device with the following options.

Default values are bold. Values that trigger contextual filtering are *italic*.

**אפשרויות, ערכים ותיאורים:**

##### Score Value

- **Value / Values:** **1**, Pick or enter a number
- **Description:** When this device is triggered, award the selected amount of score to the player. Values range from -2 billion to +2 billion.

##### Score Award Type

- **Value / Values:** None, **Add**, Subtract, Set
- **Description:** Determines how score is awarded to players.

##### Activating Team

- **Value / Values:** **Any**, Pick or enter a team
- **Description:** Defines which team can activate this device.

##### Times Can Trigger

- **Value / Values:** **Infinite**, Pick a number
- **Description:** Determines how many times this device can trigger before it is disabled.

##### Increment Score on Awarding

- **Value / Values:** **On**, Off
- **Description:** Determines if the device uses the Score Increment to update the Score amount when the the device awards the player a score.

##### Score Change when Activated

- **Value / Values:** **0**, -200 to 200
- **Description:** After the first activation of this device, adjust the score awarded by the selected value for each activation.

##### Minimum Score

- **Value / Values:** **No Limit**, Pick or enter a number
- **Description:** Determines the minimum amount of score this device can award in a single instance. Values range from -2 billion to +2 billion.

##### Maximum Score

- **Value / Values:** **No Limit**, Pick or enter a number
- **Description:** Determines the maximum amount of score this device can award in a single instance. Values range from -2 billion to +2 billion.

##### Enabled During Phase

- **Value / Values:** None, **Always**, Pre-Game Only, Gameplay Only
- **Description:** Determines the phase in which the device is enabled.

##### Visible In Game

- **Value / Values:** **No**, Yes, Only Number
- **Description:** Determines whether or not the device is visible in the game.

##### Use Static Hologram

- **Value / Values:** On, **Off**
- **Description:** If this is set to **On**, the Score Hologram will stay in place instead of always facing the player.

##### Send Event On Score

- **Value / Values:** **999**, Pick or enter a number
- **Description:** When this device awards the specified score, send an event to devices linked to the **On Score Output event**.

##### Play Audio

- **Value / Values:** **On**, Off
- **Description:** Determines whether the device should play audio effects.

##### Display Score Update on HUD

- **Value / Values:** *On*, **Off**
- **Description:** Determines whether score updates are displayed as a HUD message. If you choose **On**, several additional options are displayed below this one in the Customize panel.

##### Reset HUD Message Score

- **Value / Values:** **Off**, On
- **Description:** When the device displays a score message on the HUD, this determines whether it starts at zero.

##### HUD Message

- **Value / Values:** **Score!**, Enter text
- **Description:** Determines what message is displayed on the HUD with the score. Use the default, or enter custom text. The text field has a limit of 150 characters.

##### HUD Message Score Color

- **Value / Values:** **#BFEBFFFF**, Pick a color
- **Description:** Determines the color of the score displayed on the HUD. Click the swatch to open the Color Picker. You can click to select a swatch, or enter a Hex code in the Search bar to find that color.

##### HUD Message Color

- **Value / Values:** **#00BAFFFF**, Pick a color
- **Description:** Determines the color of the text in the message you set in the **HUD Message** option. Click the swatch to open the Color Picker. You can click to select a swatch, or enter a Hex code in the Search bar to find that color.

##### **Display Score Update if Score is 0

- **Value / Values:** On, **Off**
- **Description:** Determines if the Score Update still displays if the output score is 0.

### Direct Event Binding

Following are the [direct event binding](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#direct-event-binding) options for this device.

#### Functions

A [function](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#function) listens for an event on a device then performs an action.

-
For any function, click the **option**, then **Select Device** to access and select from the **Device dropdown menu**.

-
Once you've selected a device, click **Select Event** to bind the device to an event that will trigger the function.

-
If more than one device or event triggers a function, click the **Add** button to add a line and repeat these steps.

**אפשרויות ותיאורים:**

##### Activate When Receiving From

Activates the device when an event occurs.

##### Enable When Receiving From

Enables the device when an event occurs.

##### Disable When Receiving From

Disables the device when an event occurs.

##### Reset When Receiving From

Resets the device when an event occurs.

##### Increment When Receiving From

Activate without sending score, and increment (increase) the score value when an event occurs.

##### Decrement When Receiving From

Activate without sending score, and decrement (decrease) the value when an event occurs.

##### Set To Player Score When Receiving From

Sets the score on the device to the score of the activating player when an event occurs.

#### Events

An [event](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#event) tells another device when to perform a function.

-
For any event, click the **option**, then **Select Device** to access and select from the **Device dropdown menu**.

-
Once you've selected a device, click **Select Function** to bind this event to a function for that device.

-
If more than one function is triggered by the event, click the **Add** button to add a line and repeat these steps.

**אפשרויות ותיאורים:**

##### On Max Triggers Transmit To

When this device reaches its maximum number of triggers as defined by the **Times Can Trigger** option, it sends an event to the selected device.

##### On Score Output Transmit To

When this device awards the score defined by the **Send Event on Score** option, it sends an event to the selected device.

### Gameplay Examples Using Score Manager Devices

- [
*

Dungeon Crawler Example

Use Capture Areas to create zones that teams must capture and hold to gain points.

](https://dev.epicgames.com/documentation/fortnite/dungeon-crawler-gameplay-example-in-fortnite-creative)

- [

Top Scorer In Class

Use the Class Designer and other devices to create player classes with different abilities.

](https://dev.epicgames.com/documentation/fortnite/top-scorer-in-class-in-fortnite-creative)

[**Event Browser**](https://dev.epicgames.com/edc/manage/assets/event-browser-in-fortnite-creative)

---

## Using Stat Counter Devices in Fortnite Creative

**כותרת מקורית:** Using Stat Counter Devices in Fortnite Creative  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/using-stat-counter-devices-in-fortnite-creative  
**מקור קלט:** `07D_מטרות_התקדמות_מדדים_וניקוד(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `using-stat-counter-devices-in-fortnite-creative`

Use the **Stat Counter** device to set statistic (stats) limits that can trigger events when met. This device can set and compare stats for individual players and across teams.

Pair this device with the [Stat Creator](https://dev.epicgames.com/documentation/fortnite/using-stat-creator-devices-in-fortnite-creative) to create games where players can harvest items to gain in-game XP and increase stat levels.

For help on how to find the Stat Counter device, see [Using Devices](https://dev.epicgames.com/documentation/fortnite/using-devices-in-fortnite).

If you're using multiple copies of a device on an island, it can be helpful to [rename](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#rename-a-device) them. You can choose names that relate to each device’s purpose, so it’s easier to remember what each one does.

### Contextual Filtering

Some devices are affected by a feature called **contextual filtering**. This feature hides or displays options depending on the values selected for certain related options. This feature will reduce clutter in the Customize panel and make options easier to manage and navigate.

However, it may not be easy to recognize which options or values trigger contextual filtering. To help you identify them, in our device docs, we use *italic* for any values that trigger contextual filtering. All options will be listed, including those affected by contextual filtering; if they are hidden or displayed based on a specific option’s value, a note about that will be in the Description field for that option.

### Device Options

This device has some basic functionality, like tracking set statistics. This device can also continuously track and compare the stat value over time.

You can configure this device with the following options.

Default values are **bold**. Values that trigger contextual filtering are *italic*.

### Basic Options

**אפשרויות, ערכים ותיאורים:**

##### Tracked Stat

- **Value / Values:** **Score**, Select a stat
- **Description:** Determines which statistic this device will track.

##### Enabled During Game

- **Value / Values:** **Yes**, No
- **Description:** Determines if the device will start when the game begins.

### All Options (Additional)

**אפשרויות, ערכים ותיאורים:**

##### Compare Type

- **Value / Values:** Fewer Than, Equal or Fewer, Not Equal To, Equal To, **Equal or More**, More Than
- **Description:** Determines how the tracked stat needs to be compared against the **Comparison Value**. This determines if either the success or fail events are activated.

##### Comparison Value

- **Value / Values:** **1**, Select or enter a value
- **Description:** Determines what value the tracked stat needs to be for comparison against **Compare Type**.

##### Broadcast Events on Stat Change

- **Value / Values:** True, **False**
- **Description:** If set to **Yes**, this will broadcast the OnValueChanged event whenever a valid player's tracked stat changes. It will also broadcast the OnCompareSuccess or OnCompareFailure events when the stat comparison result changes.

##### Compare Per Player

- **Value / Values:** **Yes**, No
- **Description:** If set to **Yes**, the device will track individual stats per player. If unset, this device will track the accumulated stat value of all valid players.

##### Value Override Type

- **Value / Values:** Add, Subtract, **Set**
- **Description:** Determines if this device sets, adds to, or subtracts from the stat value when calling the **OverrideValue** function.

##### Value Override

- **Value / Values:** **0**, Pick or enter a value
- **Description:** Determines the value of the **Value Override** option.

##### Visible in Game

- **Value / Values:** Yes, **When Valid**, No
- **Description:** Determines whether or not the device is visible during gameplay.

##### Value to Show

- **Value / Values:** **Comparison**, Value, Target, Override
- **Description:** Determines what number is shown on the device.

##### Show Icon

- **Value / Values:** **Yes**, No
- **Description:** Determines whether or not to show the device's stat icon.

##### Show Background

- **Value / Values:** **Yes**, No
- **Description:** Determines whether or not to show the device's background.

##### Number Length

- **Value / Values:** **2**, Pick or enter a number
- **Description:** Determines how many numbers show on the device's readout. If dynamic, the size will update based on the displayed value.

##### Selected Team

- **Value / Values:** **Any**, Pick or enter a team number
- **Description:** Determines which team will have their stats changed and compared by this device.

##### Invert Team Selection

- **Value / Values:** Yes, **No**
- **Description:** Determines if the device will be valid for all but the selected team.

##### Selected Class

- **Value / Values:** **Any**, Pick or enter a class number
- **Description:** Determines which class will have their stats changed and compared by this device.

##### Invert Class Selection

- **Value / Values:** Yes, **No**
- **Description:** Determines if the device will be valid for all but the selected class.

##### Registered Player Behavior

- **Value / Values:** **Add Registered**, Require Registered, Ignored Registered
- **Description:** Determines how players that are registered are tracked by the device. When set to **Add Registered**, players can either be registered or selected by the other requirements. When set to **Require Registered**, players must be both registered and selected by the device. When set to **Ignore Registered**, players must be selected by the other restrictions but are not registered.

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

##### Override Value

Overrides the instigator's value for their tracked stat based on the settings of ValueOverrideType and ValueOverride.

##### Compare Stat

Tests whether the instigating player succeeds or fails the comparison. This will always activate success or fail events.

##### Enable

Enables the device to immediately trigger any stat change events if a stat has changed and is set to compare through the **Stat Change** option.

##### Disable

Disables the device to not be visible or compare stats.

##### Register Player

Registers the instigating player to be added or removed from the counted players depending on the **Track Registered Players** setting.

##### Unregister Player

Removes the instigating player from the registered list. Registered players may be added or removed from the counted players depending on the **Track Registered Players** option.

##### Unregister All Players

Clears all players from the registered list. Registered players may be added or removed from the counted players depending on the **Track Registered Players** setting.

#### Events

An [event](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#event) tells another device when to perform a function.

-
For any event option, click the **option**, then **Select Device** to access and select from the **Device dropdown menu**.

-
Once you've selected a device, click **Select Function** to bind the timer to that device's function.

-
If more than one device is affected by the function, press the **Add** button and repeat.

**אפשרויות ותיאורים:**

##### On Compare Success

When the device attempts to compare, an event is sent if it passes the comparison requirements.

##### On Compare Failure

When the device attempts to compare, an event is sent if it fails the compare requirements.

##### On Value Changed

Transmits a signal on the selected channel when the stat value changes.

---

## Using Stat Creator Devices in Fortnite Creative

**כותרת מקורית:** Using Stat Creator Devices in Fortnite Creative  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/using-stat-creator-devices-in-fortnite-creative  
**מקור קלט:** `07D_מטרות_התקדמות_מדדים_וניקוד(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `using-stat-creator-devices-in-fortnite-creative`

Use the **Stat Creator** device to create custom statistics (stats) with a set value and level to drive your gameplay. These stats are in-game data that can fulfill win/lose conditions and even scoreboard requirements.

With this device, you can create your own in-game XP leveling systems. Pair this device with a [Stat Powerup](https://dev.epicgames.com/documentation/fortnite/using-stat-powerup-devices-in-fortnite-creative) to create a custom stat that continuously decreases in value such as "Heat" to create systems where players must seek shelter or a campfire to replenish.

Within the [Island Settings'](https://dev.epicgames.com/documentation/fortnite/understanding-island-settings-in-fortnite-creative) **Mode** tab, you can then navigate to **Victory Condition** > **Round Win Condition** to set your custom status as a win requirement. Navigate to the **Scoreboard Column** options within the **User Interface** tab to set your custom stat within the gameplay's scoreboard.

Through **Unreal Editor for Fortnite** (UEFN), you can even use widget blueprints to further customize your stat's UI.

For help on how to find the Stat Creator device, see [**Using Devices**](https://dev.epicgames.com/documentation/fortnite/using-devices-in-fortnite-creative).

If you're using multiple copies of a device on an island, it can be helpful to [rename](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#rename-a-device) them. You can choose names that relate to each device’s purpose, so it’s easier to remember what each one does.

### Contextual Filtering

Some devices are affected by a feature called **contextual filtering**. This feature hides or displays options depending on the values selected for certain related options. This feature will reduce clutter in the Customize panel and make options easier to manage and navigate.

However, it may not be easy to recognize which options or values trigger contextual filtering. To help you identify them, in our device docs we use *italic* for any values that trigger contextual filtering. All options will be listed, including those affected by contextual filtering; if they are hidden or displayed based on a specific option’s value, there will be a note about that in the Description field for that option.

### Device Options

This device has some basic functionality, such as setting the value's parameters and determining who the stat will apply to. Additionally, there are some advanced options like broadcasting events for all players and using persistence.

You can configure this device with the following options.

Default values are **bold**. Values that trigger contextual filtering are *italic*.

### Basic Options

**אפשרויות, ערכים ותיאורים:**

##### Stat Name

- **Value / Values:** **Stat**, Insert stat name
- **Description:** Displays the name of the stat.

##### Max Value

- **Value / Values:** **No Limit**, *Pick or enter a value*
- **Description:** Determines the stat value that is needed to surpass the first level. If set to **No Limit**, the first level will never be completed.

##### Max Level

- **Value / Values:** **1**, Pick or enter a value number
- **Description:** Determines the maximum level players can reach during the game. Starting at 1, players will progress through all proceeding levels and then complete the stat when reaching that level.

##### Per Level Points Multiplier

- **Value / Values:** **1.0x**, Pick or enter a multiplier value
- **Description:** Determines how many points are required to reach each level in the stat.

##### Can Lose Level from Point Loss

- **Value / Values:** Yes, **No**
- **Description:** If set to **No**, when points are removed from the stat it will never revert to the previous level.

##### Scope

- **Value / Values:** **Player**, Team, Match
- **Description:** Determines who the stat will apply to. If set to either **Team** or **Match**, all players in that scope will share the same stat value.

##### Selected Team

- **Value / Values:** **Any**, Pick or enter a team number
- **Description:** Determines which team can activate the device.

##### Invert Team Selection

- **Value / Values:** On, **Off**
- **Description:** If set to **On**, this device will apply to all but the selected team.

##### Selected Class

- **Value / Values:** No Class, **Any**, Pick or enter a class number
- **Description:** Determines which class can activate the device.

##### Invert Class Selection

- **Value / Values:** On, **Off**
- **Description:** If set to **On**, this device will apply to all but the selected class.

##### Stat Color

- **Value / Values:** **White**, Select a color
- **Description:** Determines the color of the stat, which is used for the UI and other effects.

##### Stat Bar Show on HUD

- **Value / Values:** **Yes**, Non-Zero, No, *For Duration*
- **Description:** Determines if the status bar is visible during the game. If set to **For Duration**, the UI will show after the player gains or loses points then hide after a duration set by **Stat Bar Duration**. If set to **Non-Zero**, the stat bar will only show when the player has a non-zero value in the stat.

##### Stat Bar Duration

- **Value / Values:** **5 Seconds**, Pick or enter a duration
- **Description:** Determines how long the stat bar is shown on the HUD after its value changes.

### All Options (Additional)

**אפשרויות, ערכים ותיאורים:**

##### Enabled Phase

- **Value / Values:** None, **Always**
- **Description:** Determines the game phases during which the device will be enabled.

##### User Widget

- **Value / Values:** **Default**, Compact, Tiny
- **Description:** Determines what UI to show for this stat.

##### Hud Priority

- **Value / Values:** **1**, Pick or enter a number
- **Description:** Determines the order in which this stat will appear on the HUD. Higher numbers show first on the list.

##### Stat Icon

- **Value / Values:** **None**, Pick or enter an icon name
- **Description:** Determines which icon to use with this statistic.

##### Broadcast Events for All Players

- **Value / Values:** On, **Off**
- **Description:** Determines if the level and value change events broadcast for all players or just the triggering player.

##### Use Persistence

- **Value / Values:** *On*, **Off**
- **Description:** Determines if this device should save or load any data from the backend.

##### Resolve Conflicts

- **Value / Values:** First Player, Highest, Lowest, Average, **Median**
- **Description:** Determines what value is chosen for the stat when loading multiple players that have the same scope.

##### Auto Save

- **Value / Values:** Yes, **No**
- **Description:** If set to **Yes**, when the player leaves or the round ends, player data is saved automatically. If not, it will need to be saved manually through a receiver.

##### Auto Load

- **Value / Values:** Yes, **No**
- **Description:** If set to **Yes**, when the round or game starts, all players will have any saved data they have loaded.

##### Intro Animation

- **Value / Values:** None, **Fade and Slide From Left**
- **Description:** Determines what animation plays for the Stat Creator widget when it appears.

##### Outro Animation

- **Value / Values:** None, **Fade**
- **Description:** Determines what animation plays for the Stat Creator widget when it is removed.

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

##### Enable When Receiving From

Enables the device when receiving a signal from the specified channel. If the player had any points stored when disabled, they will be restored when the device is enabled.

##### Disable When Receiving From

Disables the device when receiving a signal from a specified channel.

##### Save When Receiving From

Saves the stat to persistent inventory, allowing the stat to be carried over between games. If **Auto-Save** is off, this is the only way to save data to the persistent record.

##### Load When Receiving From

Loads stats from persistent inventory.

##### Reset Stat When Receiving From

Returns the stat to a 0 value when triggered.

##### Clear Player Persistence Data When Receiving From

Clears any saved data for the instigating player when receiving a signal from the selected channel.

##### Clear Player Persistence Data for All When Receiving From

Clears saved data for all players on the island when receiving a signal from the selected channel.

##### Increase Level When Receiving From

Increases stat to the next level and resets the value if the stat has levels.

##### Decrease Level When Receiving From

Decreases the stat to the previous level and resets the value if the stat has levels.

##### Load for All When Receiving From

Loads the previously saved stat values for all players.

#### Events

An [event](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#event) tells another device when to perform a function.

-
For any event option, click the **option**, then **Select Device** to access and select from the **Device dropdown menu**.

-
Once you've selected a device, click **Select Function** to bind the timer to that device's function.

-
If more than one device is affected by the function, press the **Add** button and repeat.

**אפשרויות ותיאורים:**

##### On Level Up Send Event To

Transmits a signal on the selected channel on player level up.

##### On Reached Maximum Send Event To

Transmits a signal on the selected channel when players reach max level.

##### On Level Down Send Event To

Transmits a signal on the selected channel when a player loses a level.

##### On Value Changed Send Event To

Transmits a signal on the selected channel whenever the stat value changes.

---

## Using Stat Powerup Devices in Fortnite Creative

**כותרת מקורית:** Using Stat Powerup Devices in Fortnite Creative  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/using-stat-powerup-devices-in-fortnite-creative  
**מקור קלט:** `07D_מטרות_התקדמות_מדדים_וניקוד(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `using-stat-powerup-devices-in-fortnite-creative`

Place **Stat Powerup** devices within your game to grant and adjust in-game statistics (stats). You can either use custom statistics created in the [Stat Creator](https://dev.epicgames.com/documentation/fortnite/using-stat-creator-devices-in-fortnite-creative) device or pre-made stats such as:

-
**Score**

-
**Collect Items**

-
**Objectives**

-
**AI Eliminations**

-
**Eliminations**

-
**Elimination Assists**

-
**Eliminated**

-
**Damage Dealt**

-
**Damage Taken**

-
**Spawns Left**

-
**Lap Time**

These powerups can either be manually picked up by players or activated through device triggers.

You can pair this device with the [**Stat Creator**](https://dev.epicgames.com/documentation/fortnite/using-stat-creator-devices-in-fortnite-creative) and [Timed Objective](https://dev.epicgames.com/documentation/fortnite/using-timed-objective-devices-in-fortnite-creative) to create a game where players compete to place the most bombs that are tracked through a custom stat such as "Bombs Planted".

For help on how to find the Stat Powerup device, see [**Using Devices**](https://dev.epicgames.com/documentation/fortnite/using-devices-in-fortnite-creative).

If you're using multiple copies of a device on an island, it can be helpful to [rename](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#rename-a-device) them. You can choose names that relate to each device’s purpose, so it’s easier to remember what each one does.

### Contextual Filtering

Some devices are affected by a feature called **contextual filtering**. This feature hides or displays options depending on the values selected for certain related options. This feature will reduce clutter in the Customize panel and make options easier to manage and navigate.

However, it may not be easy to recognize which options or values trigger contextual filtering. To help you identify them, in our device docs we use *italic* for any values that trigger contextual filtering. All options will be listed, including those affected by contextual filtering; if they are hidden or displayed based on a specific option’s value, there will be a note about that in the Description field for that option.

### Device Options

This device has some basic functionality, like adjusting the value of stats applied and their duration.

You can configure this device with the following options.

Default values are **bold**. Values that trigger contextual filtering are *italic*.

### Basic Options

**אפשרויות, ערכים ותיאורים:**

##### Stat To Apply

- **Value / Values:** **Score**, Select a stat
- **Description:** Determines which stat this powerup adds or removes value from.

##### Magnitude

- **Value / Values:** **1**, Pick or enter a value
- **Description:** Determines how much of the stat’s value will be added or removed.

##### Infinite Effect Duration

- **Value / Values:** Yes, ***No***
- **Description:** Determines if the effect will stay active infinitely or not. If set to **No**, an additional option to set a custom amount of time will appear.

##### Effect Duration

- **Value / Values:** **3 Seconds**, Pick or enter a duration
- **Description:** Determines the amount of time the applied effect will stay active.

##### Respawn

- **Value / Values:** ***Yes***, No
- **Description:** Determines if the powerup will respawn after being picked up.

##### Time To Respawn

- **Value / Values:** **15 Seconds**, Pick or enter an amount
- **Description:** Sets the amount of time this powerup will respawn after pick up.

##### Ambient Audio

- **Value / Values:** **On**, Off
- **Description:** Determines whether the powerup will play ambient audio when players are nearby.

### All Options (Additional)

**אפשרויות, ערכים ותיאורים:**

##### Disables Effect On Pickup

- **Value / Values:** Yes, **No**
- **Description:** If set to **Yes**, the powerup effect will be canceled when collected.

##### Pickup Radius

- **Value / Values:** **On Touch**, Pick or enter a radius
- **Description:** Sets the distance in meters the player needs to be from the powerup to collect it.

##### Spawn on Minigame Start

- **Value / Values:** **Yes**, No
- **Description:** Determines if the powerup is spawned when the minigame starts.

##### Pick Up Audio

- **Value / Values:** **On**, Off
- **Description:** Determines if audio is played when the powerup is collected.

##### Selected Class

- **Value / Values:** **Any**, Pick or enter a class number
- **Description:** Specifies which class can interact with this powerup.

##### Selected Team

- **Value / Values:** **Any**, Pick or enter a team number
- **Description:** Specifies which team can interact with this powerup.

##### Apply To

- **Value / Values:** **Player**, Player's Team, Player's Class, Same Class In Player's Team, All Players
- **Description:** Determines which players can see the powerup.

##### Who Can See This Powerup

- **Value / Values:** None, All, Only Players That Can Pick Up
- **Description:** Determines who can see the powerup when activated.

##### Persist on Elimination

- **Value / Values:** On, **Off**
- **Description:** Determines if the powerup will continue to apply when the player has been eliminated and on their next spawn.

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

##### Spawn When Receiving From

Immediately spawns the powerup when the event occurs.

##### Despawn When Receiving From

Immediately despawns the powerup when the event occurs. The powerup will not spawn again until triggered.

##### Pickup When Receiving From

Collects the powerup when the event occurs, allowing the effect to apply through other devices.

##### Clear When Receiving From

Clears the powerup's active effect when the event occurs.

#### Events

An [event](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#event) tells another device when to perform a function.

-
For any event option, click the **option**, then **Select Device** to access and select from the **Device dropdown menu**.

-
Once you've selected a device, click **Select Function** to bind the timer to that device's function.

-
If more than one device is affected by the function, press the **Add** button and repeat.

**אפשרויות ותיאורים:**

##### On Item Picked Up Send Event To

Sends an event to linked devices when the powerup is picked up.

---

## Using Timed Objective Devices in Fortnite Creative

**כותרת מקורית:** Using Timed Objective Devices in Fortnite Creative  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/using-timed-objective-devices-in-fortnite-creative  
**מקור קלט:** `07D_מטרות_התקדמות_מדדים_וניקוד(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `using-timed-objective-devices-in-fortnite-creative`

**
The Timed Objective device is for [game modes](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#game-mode) where players can start or stop timers to advance [gameplay](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#gameplay) [objectives](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#objective), such as Attack/Defend Bomb objectives.

For help on how to find the Timed Objective** device, see [Using Devices](https://dev.epicgames.com/documentation/fortnite/using-devices-in-fortnite).

If you're using multiple copies of a device on an island, it can be useful to rename them. Choosing names that relate to a device's purpose makes it easier to remember what each one does, and easier to find a specific device when using the [Event Browser](https://dev.epicgames.com/documentation/fortnite/event-browser-in-fortnite-creative).

### Device Options

When the device is placed, any player can [enable](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#enable) or disable it. It is in its holographic state until initially started, then will appear and count down. Any team can pause the timer and interact with it. The timer will appear on the HUD.

Default values are **bold**.

#### Basic Options

**אפשרויות, ערכים ותיאורים:**

##### Time

- **Value / Values:** **10 Seconds**, Pick a time
- **Description:** Sets the length of the timer for the objective.

##### Start Score

- **Value / Values:** **None**, Pick a score
- **Description:** Sets the amount of score awarded for successfully starting an unstarted timer.

##### Stop Score

- **Value / Values:** **None**, Pick a score
- **Description:** Sets the amount of score to be awarded for successfully stopping an active timer.

##### Completed Score

- **Value / Values:** **None**, Pick a score
- **Description:** Sets the amount of score to be awarded when the timer is complete.

#### All Options (Additional)

**אפשרויות, ערכים ותיאורים:**

##### Start When Round Starts

- **Value / Values:** **No**, Yes
- **Description:** Determines whether the timer should start automatically at the beginning of each round.

##### Timer Label Text

- **Value / Values:** Enter Text
- **Description:** Specifies custom text to be displayed along with the timer countdown. The text field has an 80 character limit.

##### Timer Label Text Style

- **Value / Values:** Default, **Bold**, Pick a style
- **Description:** Sets the style for the countdown display and custom text.

##### Hologram Until Activated

- **Value / Values:** No, **Yes**
- **Description:** Determines whether the objective device appears as a hologram until activated.

##### Visible During Game

- **Value / Values:** No, **Yes**
- **Description:** Determines whether the device is visible during the game.

##### Countdown Visible on HUD

- **Value / Values:** No, **Yes**
- **Description:** Determines whether the timer countdown is displayed on the player's HUD.

##### Completion Behavior

- **Value / Values:** **Disable**, Reset, Restart
- **Description:** Determines what the device should do when the timer completes.

#### -
**Disable**: The device is disabled and cannot be used again until reset.

- **Value / Values:** -
**Reset**: The timer is reset and the device can be used again immediately.
- **Description:** -
**Restart**: The timer is reset and the countdown begins again immediately.

##### Urgency Mode

- **Value / Values:** Disabled, **Enabled**
- **Description:** Determines whether the device will enter Urgency mode when the timer gets close to the end. Urgency mode changes the timer's audio and visual effects to reflect the short time remaining.

##### Urgency Mode Start Time

- **Value / Values:** **5**, Pick a time
- **Description:** Sets the remaining counter time at which the device will enter Urgency mode.

##### Start Team Filter

- **Value / Values:** None, **All**, Pick a team
- **Description:** Determines which team can start an unstarted timer.

##### Start Interact Text

- **Value / Values:** Insert Text
- **Description:** Defines custom text to be displayed as a prompt for a player who can start an unstarted timer. The text field has an 80 character limit.

##### Start Interact Time

- **Value / Values:** Instant, **3 Seconds**, Pick a time
- **Description:** Determines the length of interaction required to start an unstarted timer.

##### Stop Team Filter

- **Value / Values:** None, **All**, Pick a team
- **Description:** Determines which team can stop an active timer.

##### Stop Interact Text

- **Value / Values:** Insert Text
- **Description:** Defines custom text to be displayed as a prompt for a player who can stop an active timer. The text field has an 80 character limit.

##### Stop Interact Time

- **Value / Values:** Instant, **3 Seconds**, Pick a time
- **Description:** Determines the length of interaction required to stop an active timer.

##### Restart Team Filter

- **Value / Values:** None, **All**, Pick a team
- **Description:** Determines which team can restart a stopped timer.

##### Restart Interact Text

- **Value / Values:** Insert Text
- **Description:** Defines custom text to be displayed as a prompt for a player who can restart a stopped timer.

##### Restart Interact Time

- **Value / Values:** Instant, **3 Seconds**, Pick a time
- **Description:** Determines the length of interaction required to restart a stopped timer.

##### Restart Score

- **Value / Values:** **None**, Pick a score
- **Description:** Sets the amount of score to be awarded for successfully restarting a stopped timer.

##### Pausing Team Filter

- **Value / Values:** **None**, All, Pick a team
- **Description:** Determines which team can pause an active timer.

##### Pause Interact Text

- **Value / Values:** Insert Text
- **Description:** Defines custom text to be displayed as a prompt for a player who can pause an active timer. The text field has an 80 character limit.

##### Pause Interact Time

- **Value / Values:** Instant, **3 Seconds**, Pick a time
- **Description:** Determines the length of interaction required to pause an active timer.

##### Pause Score

- **Value / Values:** **None**, Pick a score
- **Description:** Sets the amount of score to be awarded for successfully pausing an active timer.

##### Resuming Team Filter

- **Value / Values:** **None**, All, Pick a team
- **Description:** Determines which team can resume a paused timer.

##### Resume Interact Text

- **Value / Values:** Insert Text
- **Description:** Defines custom text to be displayed as a prompt for a player who can resume a paused timer.

##### Resume Interact Time

- **Value / Values:** Instant, **3 Seconds**, Pick a time
- **Description:** Determines the length of interaction required to resume a paused timer.

##### Resume Score

- **Value / Values:** **None**, Pick a score
- **Description:** Sets the amount of score to be awarded for successfully resuming a paused timer.

##### Show Time On Maps

- **Value / Values:** **Off**, Both, Minimap, Overview Map
- **Description:** Determines whether the timer should be displayed on the Minimap or Overview Map.

##### Mesh Options

- **Value / Values:** **None**, Explosive Attachment
- **Description:** Selects any visual additions to the device.

##### Audio Effects

- **Value / Values:** Off, **On**
- **Description:** Determines whether the device will play audio effects during the game.

##### Activation Sound

- **Value / Values:** Off, **On**
- **Description:** Determines whether the device will play a sound when activated.

##### Activation Sound Distance

- **Value / Values:** Whole Map, **Nearby**
- **Description:** Determines whether the activation sound is localized or audible anywhere on the map.

##### Deactivation Sound

- **Value / Values:** Off, **On**
- **Description:** Determines whether the device will play a sound when deactivated.

##### Deactivation Sound Distance

- **Value / Values:** Whole Map, **Nearby**
- **Description:** Determines whether the deactivation sound is localized or audible anywhere on the map.

##### Completion Sound

- **Value / Values:** Off, **On**
- **Description:** Determines whether the device will play a sound when complete.

##### Completion Sound Distance

- **Value / Values:** Whole Map, **Nearby**
- **Description:** Determines whether the completion sound is localized or audible anywhere on the map.

##### Timer Sound

- **Value / Values:** Off, **On**
- **Description:** Determines whether the device will play a sound to represent the timer.

##### Timer Sound Distance

- **Value / Values:** Whole Map, **Nearby**
- **Description:** Determines whether the timer sound is localized or audible anywhere on the map.

##### Maintain Interaction While Looking Around

- **Value / Values:** **Off**, On
- **Description:** Allows players who are interacting with this device to look around without cancelling interaction.

##### If Instigating Player Is Not Present

- **Value / Values:** **Use Empty Instigator**, Pick A Random Player
- **Description:** This determines what player instigated the signal when the instigating player is no longer in the game.

### Direct Event Binding

Following are the direct event binding options for this device.

#### Functions

A [function](https://dev.epicgames.com/documentation/en-us/fortnite-creative/function) listens for an event on a device, and then performs an action.

-
For any function, click the option, then Select Device to access and select from the Device dropdown menu.

-
Once you've selected a device, click Select Event to bind the device to an event that will trigger the function for the device.

-
If more than one device or event triggers a function, click the Add button to add a line and repeat these steps.

**אפשרויות ותיאורים:**

##### Start When Receiving From

Starts the timer when an event occurs.

##### Stop When Receiving From

Stops the timer when an event occurs.

##### Resume When Receiving From

Resumes the timer when an event occurs.

##### Complete When Receiving From

Completes the timer when an event occurs.

##### Show When Receiving From

Makes the device visible when an event occurs.

##### Hide When Receiving From

Makes the device invisible when an event occurs.

##### Enable When Receiving From

Enables the device when an event occurs.

##### Disable When Receiving From

Disables the device when an event occurs.

##### Pause When Receiving From

Pauses the timer when an event occurs.

##### Restart When Receiving From

Restarts the device when an event occurs.

#### Events

An [event](https://dev.epicgames.com/documentation/en-us/fortnite-creative/event) tells another device when to perform a function.

-
For any function, click the option, then **Select Device** to access and select from the **Device **dropdown menu.

-
Once you've selected a device, click **Select Function **to bind this event to a function for that device.

-
If more than one function is triggered by the event, click the **Add **button to add a line and repeat these steps.

 Options Description
**On Paused Send Event To**

When the timer is paused, an event is sent to the selected device.

On **Stopped**

Send Event To

When the timer is stopped, an event is sent to the selected device.

On **Resumed**

Send Event To

When the timer is resumed, an event is sent to the selected device.

On **Completed**

Send Event To

When the timer has completed., an event is sent to the selected device.

On **Started**

Send Event To

When the timer is started, an event is sent to the selected device.

On **Restarted**

Send Event To

When the timer has restarted, an event is sent to the selected device.

### Design Examples

Here are some examples of how you can use the Timed Objective device.

-
[Door Open](https://dev.epicgames.com/documentation/fortnite/using-timed-objective-devices-in-fortnite-creative)

-
[Switch Delay](https://dev.epicgames.com/documentation/fortnite/using-timed-objective-devices-in-fortnite-creative)

#### Door Open

One of the most useful functions of the Timed Objective is using it to send signals after a preset period of time.

**Devices used**:

-
1 x **Timed Objective**

-
2 x [Prop Mover](https://dev.epicgames.com/documentation/fortnite/using-prop-mover-devices-in-fortnite-creative)

-
Create a simple enclosed arena. Use two props for the doors in a closed position.

-
Attach a **Prop Mover** device to each of the movable doors. Make sure to orient the movement arrow so each door opens in the appropriate direction. Customize them both to the following settings:

 Option Value Description
Distance

2 Meters

The doors will move 2 meters.

Speed

1 Meter/Second

The doors will move at 1 m/s.

Time From Start

Off

The Prop Movers will not automatically activate after an amount of time has elapsed from the start of the round.

On Prop Collision Behavior

Continue

Any contact with other props that the doors make while moving will be ignored.

Prop Damage On Collision

None

Props impacted by the doors will not take damage.

-
Place a **Timed Objective** device anywhere on the island. Customize it to the following settings:

 Option Value Description
Timer Label Text

Doors Open In...

This HUD message is shown during the timer countdown.

Urgency Mode Start Time

3

The countdown sounds become more noticeable with 3 seconds left.

-
Set the direct event bindings of the Timed Objective to the following:

 Function Device Event Description
On Completed Send Event To

DoorPropMover1, DoorPropMover2

Start

When the Timed Objective completes, the doors will begin moving.

Here’s an overview of how devices communicate in this Design Example:

 Device A Function Device B Event Explanation
**DoorPropMover1, DoorPropMover2**

Start

**TimedObjective**
(w:95)

On Completed Send Event To

When the Timed Objective completes, the doors will begin moving.

You now have the basic functionality for sending delayed signals from the Timed Objective device.

There are countless ways to take advantage of the Timed Objective device to delay signals anywhere from seconds to minutes. From causing events to take place at a predetermined time after the start of the game to starting the countdown from a separate signal, it’s an essential part of the Creative toolset that's easy to use and offers a lot of flexibility.

Use direct event binding to start your countdowns on a signal from another device, and make sure **Completion Behavior** is set to **Reset** or **Restart** if you want it to be usable more than once.

#### Switch Delay

Another form of gameplay you can explore is creating switches that will start an interruptible countdown after a brief interaction, allowing players to try to control a point long enough to end a round in their favor.

**Devices used**:

-
1 x **Timed Objective**

-
1 x [**Switch**](https://dev.epicgames.com/documentation/fortnite/using-switch-devices-in-fortnite-creative)

-
1 x [**End Game Device**](https://dev.epicgames.com/documentation/fortnite/using-end-game-devices-in-fortnite-creative)

-
Create a small arena with a place for a Switch device where it can be contested.

-
Place a **Switch** and customize it to the following settings:

 Option Value Description
Initial State

On

The Switch will begin in the on position.

Turn On Text

Activated Counter!

This text is shown when the device is in the on state.

Turn Off Text

Deactivated Counter!

This text is shown when the device is in the off state.

Device Model

Antique Lever

The Switch will appear as an Antique Lever in game.

Interact Time

3 Seconds

It will take 3 seconds of interaction to change the state of the Switch.

-
Place a **Timed Objective** device anywhere on the map and customize it to the following settings:

 Option Value Description
Time

15 Seconds

The timer will take 15 seconds to complete.

Timer Label Text

Team A wins in...

The HUD will display this text during the timer countdown.

Timer Sound Distance

Whole Map

The timer can be heard throughout the entire map regardless of player proximity.

-
Place an **End Game Device** anywhere on the island. Customize it to the following settings:

 Option Value Description
Custom Victory Callout

Team A wins via timeout!

If the timer concludes, then Team A is the victor and this message will be shown.

-
Set the direct event bindings of the Switch to the following:

 Function Device Event Description
On Turned On Send Event To

TimedObjective

Start

When the Switch is turned on, the Timed Objective will start.

On Turned Off Send Event To

TimedObjective

Stop

When the Switch is turned off, the Timed Objective will stop.

-
Set the direct event bindings of the Timed Objective to the following:

 Function Device Event Description
On Completed Send Event To

EndGameDevice

Activate

When the Timed Objective successfully completes, the End Game Device will end the game.

Here’s an overview of how devices communicate in this Design Example:

 Device A Function Device B Event Explanation
**TimedObjective**
(w:95)

Start

**Switch**

On Turned On Send Event To

When the Switch is turned on, the Timed Objective will start.

**TimedObjective**
(w:95)

Stop

**Switch**

On Turned Off Send Event To

When the Switch is turned off, the Timed Objective will stop.

**EndGameDevice**

Activate

**TimedObjective**
(w:95)

On Completed Send Event To

When the Timed Objective successfully completes, the End Game Device will end the game.

You now have the basic functionality to create an interruptible countdown with a Timed Objective device.

It is very common to use the **Start** function and **On Completed Send Event To** event when connecting a Timed Objective to other devices. The method shown here can be an alternative to point-building [domination](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#domination)-style games, where a point only needs to be held for 15 seconds without the player who's interacting getting eliminated.

There could be multiple places unlocked before the End Game Device is triggered, with high-speed gameplay based around more competition on the Switch than other devices.

---

## Using Tracker Devices in Fortnite Creative

**כותרת מקורית:** Using Tracker Devices in Fortnite Creative  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/using-tracker-devices-in-fortnite-creative  
**מקור קלט:** `07D_מטרות_התקדמות_מדדים_וניקוד(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `using-tracker-devices-in-fortnite-creative`

Use the **Tracker** device to create and track custom [objectives](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) that a player can complete, and send a signal to another device when the player completes a tracked objective.

You can track objectives set for individual players, a team, or multiple teams. For teams, you can also track persistence data for individual players from one session to the next. (For more on this, see [Tracking Persistence Data](https://dev.epicgames.com/documentation/fortnite/using-tracker-devices-in-fortnite-creative) below.

For help on how to find the Tracker device, see [Using Devices](https://dev.epicgames.com/documentation/fortnite/using-devices-in-fortnite).

You'll need a separate tracker for each objective you want to track.

If you're using multiple copies of a device on an island, it can be useful to [rename](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) them. Choosing names that relate to a device's purpose makes it easier to remember what each one does, and easier to find a specific device when using the [Event Browser](https://dev.epicgames.com/documentation/fortnite/event-browser-in-fortnite-creative).

### Contextual Filtering

Some devices are affected by a feature called contextual filtering. This feature hides or displays options depending on the values selected for certain related options. This feature will reduce clutter in the Customize panel and make options easier to manage and navigate.

However, it may not be easy to recognize which options or values trigger contextual filtering. To help you identify them, in our device docs we use *italic* for any values that trigger contextual filtering. All options will be listed, including those affected by contextual filtering; if they are hidden or displayed based on a specific option's value, there will be a note about that in the **Description** field for that option.

### Device Options

This device has some basic functionality, like which stat is tracked, and the value for that stat when the target is met. There are also some advanced options, like whether completion progress is shared among team members or tracked individually.

Default values are **bold**. Values that trigger contextual filtering are *italic*.

You can configure this device with the following options.

 Option Values Description
**Stat to Track**

**Eliminations**, Pick a stat to track

Determines which statistic the device will track for the **Tracker Value**.

Stats that can be tracked are:

-
**Events**

-
**Eliminations** (default)

-
**Eliminated**

-
**Score**

-
**Chest Opened**

-
**Llama Opened**

-
**Player Revived**

-
**Player Interrogated**

-
**Race Checkpoint Activated**

-
**Fish Fished**

-
**Weapon Fished**

-
**Prop Destroyed**

-
**Shield Potion Consumed**

-
**Distance Traveled on Foot**

-
**Distance Traveled in Vehicle**

-
**Distance Traveled in Air**

-
**Distance Traveled**

-
**Round Completed**

-
**Round Won**

-
**Game Completed**

-
**Game Won**

-
**Play Time Elapsed**

**Reset on First Spawn**

**No**, Yes

Determines whether the tracked stat will be reset when the player spawns in to a new game or round. If **Stat to Track** is set to **Rounds Completed**, **Rounds Won**, **Games Complete**, or **Games Won**, the device will not be reset regardless of the setting you select here.

**Target Value**

**10**, Pick a number

When the device counts to the selected value, the objective is complete. If you select **0**, the tracker will never complete.

**Starting Value**

**0**, Pick or enter a number

Determines the value the tracker is set to when it first begins tracking.

**Valid Team**

**Any**, Pick or enter a number

This tracker can be assigned to players on the selected team.

**Assign on Game Start**

**On**, Off

Determines whether this tracker is assigned to applicable players when the game starts.

**Assign When Joining in Progress**

**On**, Off

Determines whether a player will be assigned this tracker when they join a game already in progress.

**Sharing**

**Individual**, Team, All

Determines whether progress is tracked for individual players, for all members of a team, or whether all players contribute progress toward a single target value. Note that if you want to use the **Resolves Conflicts** option with persistence data (statistics carried forward from session to session) you will need to set this to **Team** or **All**, as **Resolves Conflicts** doesn't apply to individual players. See [Tracking Persistence Data](https://dev.epicgames.com/documentation/fortnite/using-tracker-devices-in-fortnite-creative) for more info.

**Target Team**

**Any**, Pick or enter a number

Determines which team is tracked when the **Stat to Track** option is set to **Eliminations** or **Eliminated**.

**Target Class**

**Any**, Pick or enter a number

Determines which class is tracked when the **Stat to Track** option is set to **Eliminations** or **Eliminated**.

**When Target Is Reached**

Do Nothing, End Round, **Complete Tracker**

Determines what happens when the target tracker value is reached.

**Winning Team**

Completing Team Wins, **Use Game Win Conditions**, Pick or enter a number

Determines which team wins the round when the tracker is completed. This option is only valid if the **When Target is Reached** option is set to **End Round**.

**Amount to Change on Event**

**1**, Pick or enter a number

Determines how much to increment (add) or decrement (subtract) the tracker value each time the **Increment Progress When Receiving From** or **Decrement Progress When Receiving From** option is triggered.

**Show on HUD**

No, Detailed, List, **Both**

Determines whether tracker progress is displayed on the player's HUD. If you choose **Detailed** or **Both**, a color-coded text box displays in the upper left of the player's HUD.

**Tracker Title**

Enter text

Assigns a title to the tracker, which is displayed if **Show on HUD** is enabled. The text field has a 32-character limit.

**Description Text**

Enter text

Assigns a description to the tracker, which is displayed below the title if the **Show on HUD** option is enabled. The text field has a 64-character limit.

**Show Progress**

**Total**, Remaining, Off

Determines whether **Tracker Progress** is displayed after the **Tracker Description** if the **Show on HUD** option is enabled. If you choose **Total**, the tracker will count up to the target value. If you choose **Remaining**, the tracker will count down from the target value.

**HUD Widget**

**Default**, Slim, Tiny

Determines which widget is used for the HUD.

**Tracker Completion Ceremony**

**Yes**, No

Determines whether or not the completion of this tracker will be accompanied by a ceremony.

**Quest Icon**

**None**, Pick an icon

Sets the icon that shows on the quest box if the **Shown on HUD** option is set to show tracked stats. Click the icon to open the Icon Library picker, and choose an icon by scrolling through the Icon Library, or type a word into the search box to search for a specific icon. Select an icon, then click the checkmark. See the [Icon List table](https://dev.epicgames.com/documentation/fortnite/using-tracker-devices-in-fortnite-creative) below for available icons.

**Color**

**#FFFFFF**, Pick a color

Sets the color of the icon and the quest box. Click the color swatch to open the color picker. Each color swatch has its hex code next to the swatch. You can also type a hex code into the search bar to find a specific color. Select a color, then click the checkmark.

**Use Persistence**

**Off**, *On*

Determines whether this device should load data from earlier game sessions. If you set this to **On**, more options will show. Also see [Tracking Persistence Data](https://dev.epicgames.com/documentation/fortnite/using-tracker-devices-in-fortnite-creative) below.

**Auto Save**

Yes, **No**

This only displays if **Use Persistence** is set to **On**. Determines if the device saves its data automatically.

**Auto Load**

Initial Spawn, **Off**

This only displays if **Use Persistence** is set to **On**. Determines whether the device data and player's progress is automatically loaded. If this is set to **Initial Spawn**, data will only be loaded when the player initially spawns. If this is set to **Off**, data is never auto-loaded, and the developer needs to activate this with an event.

**Resolves Conflicts**

**Highest**, Lowest, First Player, Average, Median

This option only displays if **Use Persistence** is set to **On**. Conflict resolution is how the game treats persistence data when players join a new session. When a tracker affects more than one player at the same time, the setting selected here will determine how the tracked value is applied. Note that this option only has an effect on the game if **Sharing** is set to **Team** or **All**. It has no effect if **Sharing** is set to **Individual**.

This option determines what number the tracker should start with at the beginning of a session.

-
**Highest**: Applies the highest value in the group to each player.

-
**Lowest**: Applies the lowest value in the group to each player.

-
**First Player**: Uses the value from the first player loaded into that session and applies it to each player in the group.

-
**Average**: Takes the average value across all tracked players in the current session.

-
**Median**: Takes the value in the middle of all sorted values for this session.

**Resolves Conflict After Tracker Active**

**Yes**, No

This option only displays if **Use Persistence** is set to **On**. This option determines whether the value of the tracked stat is recalculated based on the persistence value of new players.

### Tracking Persistence Data

You can set the Tracker device to collect persistence data, meaning stats tracked across multiple sessions, with multiple players or teams.

Persistence is based on player data for a specific island, and will track multiple players for a single island.

For example, if you have a group quest where players have to collectively tame 200 wolves, but the group only manages to tame 100 before the session ends, a player can return the next day and continue taming the wolves. However, the player may be playing with a different group entirely, and that's where conflict resolution becomes important.

If the **Resolves Conflict** option is set to **Average**, in the new group, you might have one player with a persistent tracked value of 50, another with a value of 100, and a third player new to the game who starts with 0. In this case the starting value for each player would be 50+100+0/3, or **50** if you've selected **Average**.

The same tracked values set for **Median** would be **50**, based on the median (middle) value: 0 - **50** - 100.

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

##### Remove From All When Receiving From

This function removes the tracker from all valid players when an event occurs.

##### Complete When Receiving From

Immediately completes the tracker when when an event occurs.

##### Reset Progress When Receiving From

Resets the progress for the triggering player (and any players sharing progress) when an event occurs.

##### Increment Progress When Receiving From

Increases the tracker's v+alue when an event occurs.

##### Remove When Receiving From

Removes the tracker from the triggering player, and any players sharing the event.

##### Assign When Receiving From

Assigns the tracker to the [instigating](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) player (and any players sharing progress) when an event occurs.

##### Assign to All When Receiving From

Assigns the tracker to all valid players when an event occurs.

##### Increase Target Value When Receiving From

Increases the value of the target when an event occurs.

##### Decrease Target Value When Receiving From

Decreases from the target value when an event occurs.

##### Decrement Progress When Receiving From

Subtracts from the target value when an event occurs.

##### Save When Receiving From

Saves the device data and player's personal progress when an event occurs.

##### Load for Player When Receiving From

Loads instigating player's data when an event occurs .

##### Load for All When Receiving From

Loads all player data when an event occurs.

##### Clear Persistence When Receiving From

Clears instigating player's data when an event occurs.

##### Save for All When Receiving From

Saves player data for all players when an event occurs.

##### Clear for All When Receiving From

Clears data for all players when an event occurs.

#### Events

An [event](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) tells another device when to perform a function.

-
For any event option, click the **option**, then **Select Device** to access and select from the **Device dropdown menu**.

-
Once you've selected a device, click **Select Function** to bind the timer to a function for that device.

-
If more than one device is affected by the function, press the **Add** button and repeat.

**אפשרויות ותיאורים:**

##### When Complete Send Event To

When the tracker completes, it sends an event to the selected device, which triggers the selected function.

##### On Saved Send Event To

When the tracker saves data and players progress, it sends an event to the selected device, which triggers the selected function..

##### On Loaded Send Event To

When the tracker loads data and players progress, it sends an event to the selected device, which triggers the selected function.

##### On Cleared Send Event To

When device clears persistent data, it sends an event to the selected device, which triggers the selected function.

### Using the Tracker Device in Verse

You can use the code below to control a Tracker device in [Verse](https://dev.epicgames.com/documentation/en-us/uefn/learn-programming-with-verse-in-unreal-editor-for-fortnite). This code shows how to use events and functions in the Tracker device API. Modify it to fit the needs of your experience.

using { /Fortnite.com/Devices }
using { /Verse.org/Simulation }
using { /Verse.org/Random }
using { /UnrealEngine.com/Temporary/Diagnostics }

## A Verse-authored creative device that can be placed in a level
tracker_device_verse_example := class(creative_device):

 # Reference to the Switch Device in the level.
 # In the Details panel for this Verse device,

Expand code Copy full snippet(61 lines long)

To use this code in your UEFN experience, follow these steps.

-
Drag a Tracker device onto your island.

-
Create a new Verse device named **tracker_device_verse_example**. See [Create Your Own Device Using Verse](https://dev.epicgames.com/documentation/en-us/uefn/create-your-own-device-in-verse#creatinganewdevicewithverse) for steps.

-
In Visual Studio Code, open **tracker_device_verse_example.verse** in Visual Studio Code and paste the code above.

-
Compile your code and drag your Verse-authored device onto your island. See [Adding Your Verse Device to Your Level](https://dev.epicgames.com/documentation/en-us/uefn/create-your-own-device-in-verse#addingyourversedevicetoyourlevel) for steps.

-
Add a reference for the Tracker device on your island to your Verse device. See [Adding a Verse Reference to a Creative Device in Your Level](https://dev.epicgames.com/documentation/en-us/uefn/customize-device-properties-in-verse#addingaversereferencetoacreativedeviceinyourlevel) for steps.

-
Save your project and click **Launch Session** to playtest.

#### Tracker Device Verse API

See the [tracker_device API Reference](https://dev.epicgames.com/documentation/en-us/uefn/verse-api/fortnitedotcom/devices/tracker_device) for more information on using the Tracker device in Verse.

---

## Using Vending Machine Devices in Fortnite Creative

**כותרת מקורית:** Using Vending Machine Devices in Fortnite Creative  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/using-vending-machine-devices-in-fortnite-creative  
**מקור קלט:** `07D_מטרות_התקדמות_מדדים_וניקוד(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `using-vending-machine-devices-in-fortnite-creative`

The **Vending Machine** is a device that can hold and [spawn](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#spawning) [items](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#item), with an optional [cost](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) for each item. The Vending Machine can hold up to three items, and players can cycle between these by hitting the machine with their pickaxe.

The Vending Machine is one of several devices in Creative that spawns items — in this case, spawning them in front of the device when the player pays the cost. If the item was spawned by a player interacting directly with the device (not remotely), the item will be added to the player's inventory. To add an item to the Vending Machine, drop it in front of the device while in [Create mode](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#create-mode).

To find the Vending Machine device, go to the Creative inventory and select the Devices tab. From there you can search or browse for the device. For more information on finding devices see [Using Devices](https://dev.epicgames.com/documentation/fortnite/using-devices-in-fortnite).

### Adding Items to the Device

-
Stand in front of the Vending Machine.

-
Press the **Tab** key to open the Creative inventory. Click the tab for the type of item you want to [register](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#register) to the device. Locate the item and select it.

-
Click **Equip** at the bottom of the screen. This equips the item to your [Equipment Bar](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#equipment-bar).

-
Repeat the first three steps until you have equipped the three items you want to put in the Vending Machine.

-
While still in the Creative inventory, drag an item from your Equipment Bar into a blank area on the screen. This drops the item, and if you are in front of the device it will add that item to the device.

-
Repeat the previous step for the other two items. You should see images of the three items cycling on the front display of the Vending Machine.

### Device Options

When placed, the Vending Machine is inactive. When an item is dropped onto it in Create mode, a preview of that item will appear on the screen. When the game starts, a player can interact with the device and it will spawn the item. By default, there is no cost for the item.

You can register up to three items to the Vending Machine, and will show an error message if you try to add more.

You can configure this device with the following options.

Default values are **bold**.

**אפשרויות, ערכים ותיאורים:**

##### First Item Resource Type

- **Value / Values:** **Wood**, Stone, Metal, Gold
- **Description:** Determines what type of resource the first item is purchased with.

##### Cost of First Item

- **Value / Values:** **No Cost**, Pick a cost
- **Description:** Determines the amount of resources (defined in the **First Item Resource Type** option) the first item costs.

##### Second Item Resource Type

- **Value / Values:** Wood, **Stone**, Metal, Gold
- **Description:** Determines what type of resource the second item is purchased with.

##### Cost of Second Item

- **Value / Values:** **No Cost**, Pick an amount
- **Description:** Determines the amount of resources (defined in the **Second Item Resource Type** option) the second item costs.

##### Third Item Resource Type

- **Value / Values:** Wood, Stone, **Metal**, Gold
- **Description:** Determines what type of resource the third item is purchased with.

##### Cost of Third Item

- **Value / Values:** **No Cost**, Pick an amount
- **Description:** Determines the amount of resources (defined in the **Third Item Resource Type** option) the third item costs.

##### Initial Weapon Ammo

- **Value / Values:** **Don't Override**, select a number from 1 to 999
- **Description:** Sets the amount of ammunition loaded in the weapon when granted, limited by the weapon's magazine size.

##### Spare Weapon Ammo

- **Value / Values:** **Default**, select a number from 1 to 999
- **Description:** Sets how much spare ammunition is added to the player's inventory when a weapon is granted. **Default** provides ammo based on the ammo type used by the weapon.

##### Enabled at Game Start

- **Value / Values:** **Yes**, No
- **Description:** Determines whether or not the Vending Machine is enabled at start of the game.

##### Interaction Time

- **Value / Values:** **Instant**, Pick an amount of seconds
- **Description:** Determines how long the player needs to hold down the Interact control to purchase an item from the Vending Machine.

##### Model

- **Value / Values:** **Default**, Western, Modern, Screen Only
- **Description:** Determines the visual style of the Vending Machine.

##### Selected Team

- **Value / Values:** **Any**, pick a number
- **Description:** Determines which team can use the Vending Machine.

##### Invert Team Selection

- **Value / Values:** **Off**, On
- **Description:** When set to **On**, all teams except the **Selected Team** can use this device.

##### Selected Class

- **Value / Values:** No Class, **Any**, pick a number
- **Description:** Determines which class can use the Vending Machine.

##### Invert Class Selection

- **Value / Values:** **Off**, On
- **Description:** When set to **On**, all classes except the **Selected Class** can use this device.

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

##### Cycle to Next Item When Receiving From

Cycles through the registered items to the next item in the Vending Machine when an event occurs.

##### Spawn Item When Receiving From

Spawns an item when an event occurs.

#### Events

An [event](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#event) tells another device when to perform a function.

-
For any event option, click the **option**, then **Select Device** to access and select from the **Device dropdown menu**.

-
Once you've selected a device, click **Select Function** to bind the timer to a function for that device.

-
If more than one device is affected by the function, press the **Add** button and repeat.

**אפשרויות ותיאורים:**

##### On Item Spawned Send Event To

When an item spawns, it sends an event to the selected device, which triggers the selected function.

### Design Examples

Here are some examples of how you can use the Vending Machine device.

-
You can resize the Vending Machines.

-
You can use resources to purchase items.

-
You can Enable or Disable Vending Machines.

-
You can place multiple items in each Vending Machine.

#### Resizing Vending Machines

If you resize the Vending Machines, you can fit many Vending Machines into a smaller area, such as an equipment store.

You can also connect the size of the Vending Machine to the value of the items, then stack smaller machines with less valuable items, and put more expensive items in larger machines.

*Click image to enlarge.*

**Designer's Tip**

If you are going to stack machines, or place them near each other, make sure that they are already filled with items. Trying to drop items into machines that are close to each other is difficult, because you might end up adding it to the wrong one.

#### Using Resources To Purchase Items

As a developer, you can adjust the cost of the items in a Vending Machine and use any kind of resource as a currency. For each item you can set Wood, stone, metal or gold as the currency used to pay for that item. For example, the first item can cost 50 wood, the second item can cost 100 stone, and the third item can cost 200 gold.

This gives you some interesting ways to control the resources on your island, and determines how valuable every type of resource is.

#### Enable or Disable Vending Machines

The Vending Machine can be disabled until a channel is activated. This effectively locks the machine until a criteria is met, or until the player performs a specific action. This is useful if you want to limit the player's access to items.

-
Place a Vending Machine device and customize the following options as shown below.

**Enabled At Game Start**: No

-
**Enable When Receiving From**: Channel 1

-
**Disable When Receiving From**: Channel 2

-
By using other devices to send the appropriate signals, you can enable or disable the device from being used certain times during your game.

**Designer's Tip**

You can have Vending Machines become available when a player reaches a certain level, when they press a certain button, or even when they defeat a specific type of creature.

#### Multiple Items in Each Vending Machine

Each Vending Machine can sell up to 3 different items.

-
To put three items into the machine, drop the items in order that you want them to be displayed.

-
Next open the Customize panel and enter a price for each item using the **Cost of First Item**, **Cost of Second Item** and **Cost of Third Item** options. The price values range from **No Cost** to 999 of any resource. The type of resource used to buy an item is set in the **Resource Type** option for each item.

[
*](https://dev.epicgames.com/community/api/documentation/image/82ce21bf-f32c-4dad-9b2b-dc5a3ffa23f5?resizing_type=fit)

A player can cycle through each item in the Vending Machine by waiting for a few seconds until the next item is shown, or by using their pickaxe to hit the machine. Each hit will show the next item that can be purchased.

**Designer's Tip**

You can include a text message for the player, using a HUD Message or Billboard device to remind them that they can hit the Vending Machine to cycle through all the available items that it can sell.

---

## Shove Gameplay Item in Fortnite

**כותרת מקורית:** Shove Gameplay Item in Fortnite  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/shove-gameplay-item-in-fortnite  
**מקור קלט:** `08_Items_משאבים_ופריטי_משימה(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `shove-gameplay-item-in-fortnite`

*

*Learn to use this **Beta** feature, but use caution when shipping with it.

**
The Shove **gameplay item grants a player the unique ability to push another player, and for physics-enabled islands, a prop a short distance.

The shoving action is done with bare hands by players (there is no external indication of whether or not a player has the item equipped). This hidden design can create an element of suspense on your island.

You can use this item in many ways to create interesting gameplay options:

-
Players can push others off high places, causing fall damage.

-
Players can push a team member or other ally out of the way of a hazard, vehicle, or attack.

-
Players can push physics-enabled props on a trigger to activate an event.

To learn more about enabling physics, see [Getting Started with Physics](https://dev.epicgames.com/documentation/fortnite/getting-started-with-physics).

Add this item to your island to help create intense situations, for example, a player not knowing if others in the game will use the item to help or harm.

 Player using Shove to push another player off a cliff

### Finding the Shove Item in Creative

To find the Shove item in Creative, follow these steps:

-
Open the Creative Menu by pressing the **M** key on PC, or using the control that opens the Creative Menu. Click **Content** to open the inventory.

-
Click **Items** in the **Categories** panel on the left. To find the Shove item, you can type "shove" in the search bar, or just the first few letters of the word.
**
[
](https://dev.epicgames.com/community/api/documentation/image/e86aba1e-0941-4a23-ba97-2a45f0858923?resizing_type=fit) Find the Shove item in the Creative Content browser

-
Select the Shove** item, and click **Equip** at the bottom of the screen. Alternatively, you can drag it to the Equipment bar.

To grant the Shove item to players, you need to attach it to a device such as the **Item Spawner**. See the **Registering Items in Creative** section to learn how.

### Finding the Shove Item in UEFN

To find the Shove item in UEFN and add it to your level, follow these steps:

-
Open your project in UEFN.

-
In the Content Browser, select the **Fortnite** Folder. In the search bar, type "shove", or just the first few letters of the word.
**
[
](https://dev.epicgames.com/community/api/documentation/image/42201521-2a5f-41de-9df0-b66d5461d449?resizing_type=fit) Find the Shove item in the UEFN Content Browser

-
Select the Shove** item, and drag it into your level.

To grant the Shove item to players, you need to attach it to a device such as the **Item Spawner**. See the **Adding Shove to the Item List in UEFN** section to learn how.

### Registering Items in Creative

To grant items to a player, you can use several devices that grant players items. Some examples of devices that can grant items to players, or offer them in exchange for currency, are listed below.

-
[Class Designer](https://dev.epicgames.com/documentation/fortnite/using-class-designer-devices-in-fortnite-creative)

-
[Conditional Button](https://dev.epicgames.com/documentation/fortnite/using-conditional-button-devices-in-fortnite-creative)

-
[Elimination Manager](https://dev.epicgames.com/documentation/fortnite/using-elimination-manager-devices-in-fortnite-creative)

-
[Item Granter](https://dev.epicgames.com/documentation/fortnite/using-item-granter-devices-in-fortnite-creative)

-
[Item Spawner](https://dev.epicgames.com/documentation/fortnite/using-item-spawner-devices-in-fortnite-creative)

-
**Team Settings & Inventory

-
[Vending Machine](https://dev.epicgames.com/documentation/fortnite/using-vending-machine-devices-in-fortnite-creative)

You must register items to attach them to the device. To register an item for this kind of device, follow the steps below.

-
In the Content** tab of the menu screen, find the equipment and items you want to register with a device and equip them.

-
In Create mode, stand directly beside the device that will register the item.

-
Press the **Tab** key to open the player inventory screen.

-
Click and drag the item with your mouse until a backpack icon appears.

 Registering the Shove item with the Item Spawner

The compatible device will automatically register the dropped item.

### Adding Shove to the Item List in UEFN

To grant the items to your players, you must attach the item to a device that grants items to players, or offers them to players in exchange for currency. For example, the steps below show you how to add the Shove item to an **Item Spawner** device.

-
In the Content Browser, expand the **Fortnite** folder and select the **Devices** folder.

-
In the search bar, type "spawner" to reduce the number of devices shown.

-
Scroll down to find the **Item Spawner** device, and drag it into your level.

-
Select the Item Spawner in your viewport or in the Outliner. In the **Details** panel, locate the **Item List** option under **User Options**.
**
[
*](https://dev.epicgames.com/community/api/documentation/image/46b2f432-408c-4e52-b209-623ea60e915c?resizing_type=fit) Locate the Item List option in the Details panel

-
Click the + (plus)** icon to add an array element.
**
[
](https://dev.epicgames.com/community/api/documentation/image/927b6943-2bf8-42b7-adde-9f8f9aac924f?resizing_type=fit) Click the plus sign to add an array element

-
Click the dropdown for Pickup to Spawn**, and type "shove" into the search bar. Select the **Shove** item.

[
](https://dev.epicgames.com/community/api/documentation/image/f54d2172-2018-4cc4-9a56-028b0ffc1144?resizing_type=fit) Click the dropdown and select the Shove item

Now the Shove item is attached to the Item Spawner, and it will spawn the item in the game.

---

## Using Crafting Items in Fortnite Creative

**כותרת מקורית:** Using Crafting Items in Fortnite Creative  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/using-crafting-items-in-fortnite-creative  
**מקור קלט:** `08_Items_משאבים_ופריטי_משימה(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `using-crafting-items-in-fortnite-creative`

Offer **crafting** items to players throughout gameplay as an island resource that can be collected and exchanged. Players cannot directly consume these items, but can collect them to simulate [crafting](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#crafting) by exchanging them for other usable items.

Crafting items are:

-
**Animal Bones**

-
**Stink Sac**

-
**Mechanical Parts**

-
**Cube Monster Parts**

Though more items are considered crafting items, only these items will show on the top row of the **Resources** bar as shown in [Managing Consumables](https://dev.epicgames.com/documentation/fortnite/using-crafting-items-in-fortnite-creative).

These items could be required along with another to unlock requirements for [devices](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#device) like the [**Conditional Button**](https://dev.epicgames.com/documentation/fortnite/using-conditional-button-devices-in-fortnite-creative).

*Use the devices like Conditional Button and Item Granter to create the system of crafting.*

You could pair **Animal Bones** with [****](https://dev.epicgames.com/documentation/fortnite/using-mineral-ore-crafting-items-in-fortnite-creative)**[Rough Ore](https://dev.epicgames.com/documentation/en-us/fortnite-creative/using-mineral-ore-crafting-items-in-fortnite-creative)** as requirements needed to craft weapons like the **Primal Pistol**.

To do so, you will need to set the Conditional Button's setting **Key Items Required** to **2** and pair the device with an [**Item Granter**](https://dev.epicgames.com/documentation/fortnite/using-item-granter-devices-in-fortnite-creative) to grant the usable item.

You can also blend items with [props](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#prop) of similar [themes](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) from the **Galleries** and **Prefabs** tab.

*Click image to enlarge.*

For example, you can blend Cube Monster Parts with props from the **Crashed Abductor Gallery** to fully immerse players onto your island.

To create the process of crafting, you will need to either [spawn](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#spawning) or [grant](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#grant) items onto the map for players to collect with the **Item Spawner** or **Item Granter**.

Players can collect these items to exchange for usable items through devices like Conditional Button, which consumes equipped items. They can also use these items to craft other items that will build up to a larger item.

Visit our [video tutorials](https://mediaspace.unrealengine.com/playlist/dedicated/208434573/1_gxu6mwv5/1_qfnz9w5c) to learn more about working with items and for tips to enhance gameplay.

### Finding and Placing Items

*Click image to enlarge.*

-
From **Build** mode, press the **Tab** key, then click **CREATIVE** on the top navigation bar to select the CREATIVE inventory screen if not already displayed.

-
Click the **CONSUMABLES** tab.

-
On this screen, scroll to find and select the item, use the **Search** box to look up the item by name, or check the list of relevant **Categories** specific to the item you’re looking for to filter the view.

-
Click the item, then click either **EQUIP** or **ADD TO CHEST**.

Clicking **Equip** will add the item to your [Resources bar](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#resources-bar). (When you're back in Create mode, you can view items in your Resources bar by pressing the **Tab** key and selecting **Play**.)

*Click image to enlarge.*

You may want to offer an item bundle to players through a [chest](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#chest) or [llama](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#llama). Selecting **Add To Chest** will add the item to the [Chest tab](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary). Each time you click it, the item count will increase by one, shown in a yellow box on the **Chest** tab.

From the **Chest** tab, you can select either **Create Chest** or **Create Llama** to store the items in a Chest or a Llama for use [in-game](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#ingame).

You can add up to fifteen items to the **Chest** tab. When it’s full, the **Add To Chest** tab will disappear. To add more items, you first have to remove items from the **Chest** tab.

### Managing Items

You can manage these items when you are in [Play inventory](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#play-inventory). To access the **Play** inventory screen, press **Tab** and click **Play** in the top navigation bar. In the PLAY inventory, you can create or split item stacks, or remove them entirely from your Resources bar.

*Click image to enlarge.*

Instead of dropping these items on the ground, it's best to grant them to players by using item-granting devices like the Item Spawner.

You cannot reposition or copy items with the phone tool. To delete an item from your inventory in Create mode, you will have to select either *Respawn* or *Back To Hub* from the *Menu*. When you do this, your inventory clears.

### Crafting Items

 Item Usage

**Animal Bones**

Can be gathered from bone-themed props or wildlife to craft items like the **Pimal Pistol**.

**Mechanical Parts**

Can be gathered from mechanical-themed props or vehicles to craft items like the **Clinger**.

**Stink Sac**

Can be gathered from wildlife or trash-themed props to craft items like the **Stink Bomb**.

**Cube Monster Parts**

Can be gathered fas alien-themed items from **Galleries** like the **Kevin Cube** or **Zero Point** to craft items like the **Sideways Rifle**.

### Registering Items

[
*](https://dev.epicgames.com/community/api/documentation/image/896c3b8f-3c8f-462b-b1e8-25c44a43acd2?resizing_type=fit)

*Click image to enlarge.*

You can drop items directly onto devices that can either hold or grant items. Above shows the Conditional Button, which holds two crafting items and an Item Granter that holds one usable item.

This pair of devices can be set up for players to exchange Animal Bones and Rough Ore for a Primal Pistol. To do so, these items must first be [registered](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#register) to the devices that will hold the information.

*Click image to enlarge.*

To register an item for this kind of device, follow the steps below. (You can also watch a [video tutorial](https://mediaspace.unrealengine.com/media/RegisteringCraftingConsumablesinFortniteCreative/1_zpmj3v0g) that shows you how to register items, for [crafting](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#crafting) or other [in-game](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#ingame) use.)

To register an item for this kind of device, follow these steps.

-
In the CREATIVE inventory, find the equipment and items you want to register with a device and equip them.

-
In Create mode, stand directly beside the device that will register the item.

-
Press the **Tab** key to open the **PLAY** inventory screen.

-
Click the item, then press either **Z** or **X** to split or drop the item. You can also drag the item to the side until a [backpack icon](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#backpack-icon) appears.

The compatible device will automatically register the dropped item.

Compatible devices that can hold items are:

-
**Vending Machine**

-
**Team Settings & Inventory**

-
**Class Designer**

-
**Capture Item Spawner**

-
**Capture Area**

-
**Item Granter**

-
**Item Spawner**

-
**Conditional Button**

-
**Elimination Manager**

-
**Item Remover**

Use these devices to set up your own system for granting and spawning items onto your island.

---

## Using Crystal Crafting Items in Fortnite Creative

**כותרת מקורית:** Using Crystal Crafting Items in Fortnite Creative  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/using-crystal-crafting-items-in-fortnite-creative  
**מקור קלט:** `08_Items_משאבים_ופריטי_משימה(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `using-crystal-crafting-items-in-fortnite-creative`

Players can use **Crystal items** as [crafting](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#crafting) materials for items that can use crystals as an ingredient. You can set this [item](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) to be required with another item to unlock requirements for devices like the [**Conditional Button**](https://dev.epicgames.com/documentation/fortnite/using-conditional-button-devices-in-fortnite-creative).

Crystal items are:

-
**Quartz Crystal**

-
**Rainbow Crystal**

-
**Shadowshard Crystal**

-
**Sunbeam Crystal**

*Use the devices like Conditional Button and Item Spawner to create the system of crafting.*

You could pair Crystal items with [Blast Powder items](https://dev.epicgames.com/documentation/en-us/fortnite-creative/using-power-crafting-items-in-fortnite-creative) as materials needed to craft weapons or another item like the **Boogie Bomb**.

To do so, you will need to set the Conditional Button's setting **Key Items Required** to **2** and pair the device with an [**Item Granter**](https://dev.epicgames.com/documentation/fortnite/using-item-granter-devices-in-fortnite-creative) to grant the usable item.

You can also blend items with [props](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#prop) of similar [themes](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) from the **Galleries** and **Prefabs** tab.

*This Galleries prop can be found in the Volcanic Rock Gallery.*

For example, you can blend crystal items with rocks from the **Galleries** tab to fully immerse players onto your island.

To create the process of crafting, you will need to either spawn items onto your map with the [**Item Spawner**](https://dev.epicgames.com/documentation/fortnite/using-item-spawner-devices-in-fortnite-creative) or grant them to players with [**Item Granter**](https://dev.epicgames.com/documentation/fortnite/using-item-granter-devices-in-fortnite-creative).

Players can collect these items to exchange for usable items through devices like Conditional Button, which consumes equipped items. They can also use these items to craft other items that will build up to a larger item.

Visit our [video tutorials](https://mediaspace.unrealengine.com/playlist/dedicated/208434573/1_gxu6mwv5/1_qfnz9w5c) to learn more about working with items and for tips to enhance gameplay.

### Finding and Placing Items

*Click image to enlarge.*

-
From [Build mode](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#create-mode), press the **Tab** key, then click **CREATIVE** on the [top navigation bar](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) to select the [CREATIVE inventory](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) screen if not already displayed.

-
Click the **CONSUMABLES** tab.

-
Scroll to find and select the item, use the **Search** box to look up the item by name, or check the list of relevant **Categories** specific to the item you're looking for to filter the view.

-
Click the item, then click either **EQUIP** or **ADD TO CHEST**.

Clicking EQUIP will add the item to your [Equipment bar](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#equipment-bar). (When you're back in Create mode, you can view any items you've [equipped](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#equip) by pressing the **F** key.)

From the CHEST tab, you can select either CREATE CHEST or CREATE LLAMA to store the items in a Chest or a Llama for use [in-game](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#ingame).

Clicking EQUIP will add the item to your [Resources bar](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#resources-bar). (When you're back in Create mode, you can view items in your Resources bar by pressing the **Tab** key and selecting **Play**)

You may want to offer an item bundle to players through a [chest](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#chest) or [llama](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#llama). Selecting **Add To Chest** will add the item to the [Chest tab](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary). Each time you click it, the item count will increase by one, shown in a yellow box on the **Chest** tab.

From the **Chest** tab, you can select either **Create Chest** or **Create Llama** to store the items in a Chest or a Llama for use [in-game](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#ingame).

You can add up to fifteen items to the **Chest** tab. When it’s full, the **Add To Chest** tab will disappear. To add more items, you first have to remove items from the **Chest** tab.

### Managing Items

You can manage these items when you are in [Play inventory](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#play-inventory). To access the **Play** inventory screen, press **Tab** and click **Play** in the top navigation bar. In the PLAY inventory, you can create or split item stacks, or remove them entirely from your Equipment bar.

*Click image to enlarge.*

Instead of dropping these items on the ground, it's best to grant them to players by using item-granting devices like the Item Spawner.

You cannot reposition or copy items with the phone tool. To delete an item from your inventory in Create mode, you will have to select either *Respawn* or *Back To Hub* from the *Menu*. When you do this, your inventory clears.

### Crystal Items

 Item Usage

**Quartz Crystal**

Can be used as a required crafting ingredient for weapons or items like the **Raygun**. This item can also be required as a piece to craft a larger item.

**Shadowshard Crystals**

Can be used as a required ingredient for weapons or items like the **Boogie Bomb**. This item can also be required as a piece to craft a larger item.

**Shadowshard Crystals**

Can be used as a required ingredient for weapons or items like the **Rift-To-Go**. This item can also be required as a piece to craft a larger item.

**Sunbeam Crystal**

Can be used as a required ingredient for weapons or items like the **Jetpack**. This item can also be required as a piece to craft a larger item.

### Registering Crafting Items to a Device

[
*](https://dev.epicgames.com/community/api/documentation/image/a43d943b-143c-4a98-b028-dccfe6873501?resizing_type=fit)

*Click image to enlarge.*

You can drop items directly onto devices that can either hold or grant items. Above shows the Conditional Button, which holds two crafting items and an Item Granter that holds one usable item.

This pair of devices can be set up for players to exchange Blast Powder and Rainbow Crystals for a Boogie Bomb. To do so, these items must first be [registered](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#register) to the devices that will hold the information.

*Click image to enlarge.*

To register items to a device, you must stand directly on or immediately beside the device.

To register an item for this kind of device, follow the steps below. (You can also watch a [video tutorial](https://mediaspace.unrealengine.com/media/RegisteringCraftingConsumablesinFortniteCreative/1_zpmj3v0g) that shows you how to register items, for [crafting](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#crafting) or other [in-game](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#ingame) use.)

-
In the CREATIVE inventory, find the equipment and items you want to register with a device and equip them.

-
In Create mode, stand directly beside the device that will register the item.

-
Press the **Tab** key to open the **PLAY** inventory screen.

-
Click the item, then press either **Z** or **X** to split or drop the item. You can also drag the item to the side until a [backpack icon](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#backpack-icon) appears.

The compatible device will automatically register the dropped item.

Compatible devices that can hold items are:

-
**Vending Machine**

-
**Team Settings & Inventory**

-
**Class Designer**

-
**Capture Item Spawner**

-
**Item Granter**

-
**Item Spawner**

-
**Conditional Button**

-
**Elimination Manager**

-
**Item Remover**

Use these devices to set up your own system for granting and spawning items onto your island.

---

## Using Dino Egg Items in Fortnite Creative

**כותרת מקורית:** Using Dino Egg Items in Fortnite Creative  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/using-dino-egg-items-in-fortnite-creative  
**מקור קלט:** `08_Items_משאבים_ופריטי_משימה(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `using-dino-egg-items-in-fortnite-creative`

Use **Dino Egg** [items](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) as [crafting](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#crafting) materials that can build up to other items. These items could be required along with another item to unlock requirements for [devices](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#device) like the [**Conditional Button**](https://dev.epicgames.com/documentation/fortnite/using-conditional-button-devices-in-fortnite-creative).

A full description of these Dino Egg items is in the [table](https://dev.epicgames.com/documentation/fortnite/using-dino-egg-items-in-fortnite-creative#primal-items) below.

*Use devices like Conditional Button and Item Spawner to create a system of crafting.*

You could pair items like [****](https://dev.epicgames.com/documentation/fortnite/using-healing-items-in-fortnite-creative)**[Bandages](https://dev.epicgames.com/documentation/en-us/fortnite-creative/using-healing-items-in-fortnite-creative)** and **White Dino Eggs** as materials needed to craft weapons or other items like [****](https://dev.epicgames.com/documentation/fortnite/using-egg-items-in-fortnite-creative)**[Heal Eggs](https://dev.epicgames.com/documentation/en-us/fortnite-creative/using-egg-items-in-fortnite-creative)**.

To do this, you would need to set the Conditional Button setting **Key Items Required** to **2** and pair the device with an [**Item Granter**](https://dev.epicgames.com/documentation/fortnite/using-item-granter-devices-in-fortnite-creative) or [**Item Spawner**](https://dev.epicgames.com/documentation/fortnite/using-item-spawner-devices-in-fortnite-creative) to grant the usable item.

You can also blend items with [props](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#prop) of similar [themes](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#island-theme) from the **Galleries** and **Prefabs** categories.

*This Galleries prop can be found in Dinosaur Prop Gallery.*

For example, you can blend food with fridges and stoves for immersive gameplay.

To create the process of crafting, you will need to either [spawn](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#spawning) the item onto your map with the Item Spawner or [grant](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#grant) items to players through the Item Granter.

Players can collect these items to exchange for usable items through devices like Conditional Button, which consumes equipped items. They can also use these items to craft other items that will build up to a larger item.

See this [video tutorial](https://www.youtube.com/watch) to learn more about working with items, and for tips on how you can enhance gameplay.

### Finding and Placing Items

*Click image to enlarge.*

-
From **Create mode**, press the **Tab** key and click **Creative** to select the [Creative inventory](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) screen.

-
Click the **Items** tab.

-
On this screen, scroll to find and select the item, use the **Search** box to look up the item by name, or check the list of relevant **Categories** specific to the item you're looking for to filter the view.

-
Click the item, then either choose **Equip** or **Add To Chest**.

Clicking **Equip** will add the item to your [Resources bar](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#resources-bar). When you're back in Create mode, you can view items in your Resources bar by pressing the **Tab** key and selecting **Play**.

You may want to create an item bundle to players through a [chest](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#chest) or [llama](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#llama). Selecting Add To Chest will add the item to the [Chest tab](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary). Each time you click it, the item count will increase by one, shown in a yellow box on the Chest tab.

You can add up to fifteen items to the Chest tab. When it’s full, the Add To Chest tab will disappear. To add more items, you first have to remove items from the Chest tab.

From the Chest tab, you can select either Create Chest or Create Llama to store the items in a Chest or a Llama for use [in-game](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#ingame).

### Managing Items

You can manage these items when you are in [Play inventory](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#play-inventory). To access the **Play** inventory screen, press **Tab** and click **Play** in the top navigation bar. In the **Play** inventory screen, you can split item stacks or remove them entirely from the Resources bar.

Instead of dropping these items on the ground, it's best to grant them to players by using item-granting devices like the Item Spawner.

You cannot reposition or copy items with the phone tool. To delete an item from your inventory in Create mode, you will have to select either *Respawn* or *Back To Hub* from the *Menu*. When you do this, your inventory clears.

### Primal Items

 Item Usage

**Yellow Eruption Dino Egg**

Themed to be harvested from dinosaurs.

**White Speckled Dino Egg**

Themed to be harvested from dinosaurs.

**White Shimmering Dino Egg**

Themed to be harvested from dinosaurs.

**White Marbled Dino Egg**

Themed to be harvested from dinosaurs.

**White Dino Egg**

Themed to be harvested from dinosaurs.

**Red Shimmering Dino Egg**

Themed to be harvested from dinosaurs.

**Red Flecked Dino Egg**

Themed to be harvested from dinosaurs.

**Red Eruption Dino Egg**

Themed to be harvested from dinosaurs.

**Pink Marbled Dino Egg**

Themed to be harvested from dinosaurs.

**Green Marbled Dino Egg**

Themed to be harvested from dinosaurs.

**Green Flecked Dino Egg**

Themed to be harvested from dinosaurs.

**Green Dino Egg**

Themed to be harvested from dinosaurs.

**Gray Eruption Dino Egg**

Themed to be harvested from dinosaurs.

**Brown Speckled Dino Egg**

Themed to be harvested from dinosaurs.

**Brown Dino Egg**

Themed to be harvested from dinosaurs.

**Blue Speckled Dino Egg**

Themed to be harvested from dinosaurs.

**Blue Shimmering Dino Egg**

Themed to be harvested from dinosaurs.

**Blue Flecked Dino Egg**

Themed to be harvested from dinosaurs.

### Registering Crafting Items to a Device

[
*](https://dev.epicgames.com/community/api/documentation/image/8a0ae15f-54b8-45b3-9936-b48609e7cc1d?resizing_type=fit)

You can drop items directly onto devices that can either hold or grant items. Above shows the Conditional Button, which holds two crafting items and an Item Spawner that holds one usable item.

This pair of devices can be set up for players to exchange Wheat and Roasted Chicken for Meat. To do so, these items must first be [registered](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#register) to the devices that will hold the information.

To register items to a device, you must stand directly on or immediately beside the device.

To register an item for this kind of device, follow these steps.

-
In the Creative inventory, find the equipment and items you want to register with a device and equip them.

-
In Create mode, stand directly beside the device that will register the item.

-
Press the **Tab** key to open the **Play** inventory screen.

-
Click the item, then press either **Z** or **X** to split or drop the item. You can also drag the item to the side until a [backpack icon](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#backpack-icon) appears.

The compatible device will automatically register the dropped item.

Compatible devices that can hold items are:

-
**Vending Machine**

-
**Team Settings & Inventory**

-
**Class Designer**

-
**Capture Item Spawner**

-
**Item Granter**

-
**Item Spawner**

-
**Conditional Button**

-
**Elimination Manager**

-
**Item Remover**

-
**Item Placer**

Use these devices to set up your own system for granting and spawning items onto your island.

---

## Using Disguise Items in Fortnite Creative

**כותרת מקורית:** Using Disguise Items in Fortnite Creative  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/using-disguise-items-in-fortnite-creative  
**מקור קלט:** `08_Items_משאבים_ופריטי_משימה(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `using-disguise-items-in-fortnite-creative`

Offer **Disguise** [items](https://dev.epicgames.com/documentation/fortnite/fortnite-creative-glossary#items) for players to conceal themselves and blend in with the environment. Both the **Creepin Cardboard** and the **Sneaky Snowman** can replenish themselves when used so that players can decorate their surroundings with matching props to blend in.

Disguise items include:

**Creepin’ Cardboard**

**Sneaky Snowman**

**Bush**

**Big Bush Bomb**

### Finding and Placing Items

Click the image to enlarge.

From [**Create** mode](https://dev.epicgames.com/documentation/fortnite/fortnite-creative-glossary#create-mode), press the **Tab** key, then click **CREATIVE** on the [top navigation bar](https://dev.epicgames.com/documentation/fortnite/fortnite-creative-glossary#topnavigationbar) to select the [CREATIVE inventory](https://dev.epicgames.com/documentation/fortnite/fortnite-creative-glossary#creativeinventory) screen if not already displayed.

Click the **CONSUMABLES** tab.

Scroll to find and select the item, use the **Search** box to look up the item by name, or check the list of relevant **Categories** specific to the item you're looking for to filter the view.

Click the item, then click either **Equip** or **Add To Chest**.

Clicking **Equip** will add the item to your [Equipment bar](https://dev.epicgames.com/documentation/fortnite/fortnite-creative-glossary#equipmentbar). When you're back in Create mode, you can view any items you've [equipped](https://dev.epicgames.com/documentation/fortnite/fortnite-creative-glossary#equip) by pressing the **F** key. You can select equipped items by either scrolling your middle mouse button or by pressing its corresponding number on your keyboard.

From the [**Chest**](https://dev.epicgames.com/documentation/fortnite/fortnite-creative-glossary#chesttab) tab, you can select either **Create Chest** or **Create Llama** to store the items in a [chest](https://dev.epicgames.com/documentation/fortnite/fortnite-creative-glossary#chest) or a [llama](https://dev.epicgames.com/documentation/fortnite/fortnite-creative-glossary#llama) for use [in-game](https://dev.epicgames.com/documentation/fortnite/fortnite-creative-glossary#in-game).

Click the image to enlarge.

Chests and llamas are a great way to offer item bundles to players. Selecting **Add To Chest** will add the item to the **Chest** tab. Each time you click **Add To Chest**, the item count will increase by one, shown as a yellow box on the Chest tab.

You can add up to fifteen items to the Chest tab. When it’s full, the **Add To Chest** button will disappear. You must remove items from the **Chest** tab to add more.

There are many ways to offer these items to players. Use any devices under the [Registering Items](https://dev.epicgames.com/documentation/fortnite/using-disguise-consumables-in-fortnite-creative#registeringitems) section to offer or require these items during gameplay.

### Managing Items

You can manage these items in the [**Play** inventory](https://dev.epicgames.com/documentation/fortnite/fortnite-creative-glossary#play-inventory). To access the **Play** inventory screen, press **Tab** and click **Play** in the top navigation bar. Here, you can swap item positions or drop them from your Equipment bar.

You cannot reposition or copy items with the phone tool. To delete an item from your inventory in Create mode, you will have to select either *Respawn* or *Back To Hub* from the *Menu*. When you do this, your inventory clears.

### Using Disguise Items

Players can use Creepin’ Cardboard and Sneaky Snowman by holding the right mouse button. Use the [aiming arc](https://dev.epicgames.com/documentation/fortnite/fortnite-creative-glossary#aiming-arc) to position and throw the item and press the interact button to enter. The Bush can be entered by pressing the interact button.

 Item
 Usage

 **Creepin’ Cardboard**

Can be thrown and entered for a player to disguise themselves as a prop. A player can still move freely and build while hiding inside this prop. To fully hide, a player must crouch while in disguise. While hiding, a player can also throw multiple copies of this prop to blend in with their surroundings. Enemy players can destroy this prop when inflicting damage. When thrown, this item will regenerate after 30 seconds. Players can equip this item a stack of one, which comes with 5 uses.

 **Sneaky Snowman**

Can be thrown and entered for players to disguise themselves as props. A player can still move freely and build while hiding inside this prop. To fully hide, a player must crouch while in disguise. While hiding, a player can also throw multiple copies of this prop to blend in with their surroundings. Enemy players can destroy this prop when inflicting damage. When destroyed, this prop will turn into a throwable snowball that deals 80 points of damage while freezing the contacting player’s feet, causing them to slide uncontrollably. This item will regenerate its uses after 30 seconds when thrown. Players can equip this item in stacks of one, which comes with 5 uses.

 **Bush**

Can be consumed to apply a bush over the player. This bush will appear transparent to the player wearing it, allowing them to move and build freely. To fully hide, the player must crouch while in disguise. The Bush can only take damage once before it is destroyed. This item can be equipped in stacks of two.

 **Big Bush Bomb**

Can be thrown to deploy a large bush for players to hide in. This item can be equipped in stacks of four.

### Registering Items

You can drop items directly onto devices that can either hold or [grant](https://dev.epicgames.com/documentation/fortnite/fortnite-creative-glossary#grant) items. You must [register](https://dev.epicgames.com/documentation/fortnite/fortnite-creative-glossary#register) these items to save in the device's memory.

To register items to a device, stand directly on or immediately beside the device.

To register an item for this kind of device, follow the steps below. (You can also watch a [video tutorial](https://mediaspace.unrealengine.com/media/RegisteringCraftingConsumablesinFortniteCreative/1_zpmj3v0g) that shows you how to register items, for [crafting](https://dev.epicgames.com/documentation/fortnite/fortnite-creative-glossary#crafting) or other [in-game](https://dev.epicgames.com/documentation/fortnite/fortnite-creative-glossary#in-game) use.)

In the CREATIVE inventory, find the equipment and items you want to register with a device and equip them.

In Create mode, stand directly beside the device registering the item.

Press the **Tab** key to open the **PLAY** inventory screen.

Click the item, then press either **Z** or **X** to split or drop the item. You can also drag the item to the side until a [backpack icon](https://dev.epicgames.com/documentation/fortnite/fortnite-creative-glossary#backpack-icon) appears.

The compatible device will automatically register the dropped item. Compatible devices that can hold items include:

**Vending Machine**

**Team Settings & Inventory**

**Class Designer**

**Capture Item Spawner**

**Capture Area**

**Item Granter**

**Item Spawner**

**Conditional Button**

**Elimination Manager**

**Item Remover**

Use these devices to set up a system for granting and spawning items onto your island.

### Using Items for Crafting

You can pair items with each other and with weapons to create the process of [crafting](https://dev.epicgames.com/documentation/fortnite/fortnite-creative-glossary#crafting), where players exchange one item or group of items for another.

To do this, choose from the list of compatible devices above like the [**Conditional Button**](https://dev.epicgames.com/documentation/fortnite/using-conditional-button-devices-in-fortnite-creative) and [**Item Spawner**](https://dev.epicgames.com/documentation/fortnite/using-item-spawner-devices-in-fortnite-creative) to set up the crafting process.

For example, you can require [**Flower Petals**](https://dev.epicgames.com/documentation/404) and [**Fibrous Herbs**](https://dev.epicgames.com/documentation/404) as items needed to craft a **Bush**.

Visit our [video tutorials](https://mediaspace.unrealengine.com/playlist/dedicated/208434573/1_gxu6mwv5/1_qfnz9w5c) to learn more about working with items and for tips to enhance gameplay.

---

## Using Gold Items in Fortnite Creative

**כותרת מקורית:** Using Gold Items in Fortnite Creative  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/using-gold-items-in-fortnite-creative  
**מקור קלט:** `08_Items_משאבים_ופריטי_משימה(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `using-gold-items-in-fortnite-creative`

You can [register](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#register) **Gold** items as required [currency](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#currency) for players to use on your island. The set requirements will show on a HUD message near the device.

You can use this item as required currency for devices like:

-
**Conditional Button**

-
**Item Spawner**

-
**Vending Machine**

While [in-game](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#ingame), you can offer gold throughout the world for players to collect by through devices like the **Item Spawner** or **Item Granter**.

Through the [My Island - Settings menu](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary), you can adjust multiple settings for gold allocation on your island. You can change settings like **Show Gold Resource Count** to determine if gold will show on the player's HUD.

*Click image to enlarge.*

You can also grant players with Gold by using the **Round Settings** device and altering the **Gold Given Per Round** settings.

*Click image to enlarge.*

### Finding and Placing Items

*Click image to enlarge.*

-
From **Create mode**, press the **Tab** key and click **CREATIVE** to select the **Creative inventory screen**.

-
Click the **CONSUMABLES** tab.

-
On this screen, scroll to find and select the item, use the **Search** box to look up the item by name, or check the list of relevant **Categories** specific to the item you’re looking for to filter the view.

-
Click the item, then click either **EQUIP** or **ADD TO CHEST**.

Clicking **EQUIP** will add the item to your [Resources bar](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#resources-bar). (When you're back in Create mode, you can view items in your Resources bar by pressing the **Tab** key and selecting **Play**)

You may want to offer an item bundle to players through a [chest](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#chest) or [llama](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#llama). Selecting **ADD TO CHEST** will add the item to the [CHEST tab](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary).

*Click image to enlarge.*

Each time you click **ADD TO CHEST**, the item count will increase by one, shown in a yellow box on the **CHEST** tab.

You can add up to fifteen items to the **CHEST** tab. When it’s full, the **ADD TO CHEST** tab will disappear. To add more items, you first have to remove items from the **CHEST** tab.

From the **CHEST** tab, you can select either **CREATE CHEST** or **CREATE LLAMA** to store the items in a Chest or a Llama for use [in-game](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#ingame).

### Managing Items

You can manage these items when you are in [Play inventory](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#play-inventory). To access the **Play** inventory screen, press **Tab** and click **Play** in the top navigation bar. In the Play inventory screen, you can create or split item stacks, or remove them entirely from the Resources bar.

*Click image to enlarge.*

Instead of dropping these items on the ground, it's best to grant them to players by using item-granting devices like the Item Spawner.

You cannot reposition or copy items with the phone tool. To delete an item from your inventory in Create mode, you will have to select either *Respawn* or *Back To Hub* from the *Menu*. When you do this, your inventory clears.

### Registering Items

Some devices can hold or grant items. To [register](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#register) an item for this kind of device, follow these steps.

-
In CREATIVE inventory, find the equipment and items you want to register with a device and equip them.

-
In Create mode, stand directly beside the device that will register the item.

-
Press the **Tab** key to open the **PLAY inventory** screen.

-
Click the item, then press either **Z** or **X** to split or drop the item. You can also drag the item to the side until a [backpack icon](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#backpack-icon) appears.

The compatible device will automatically register the dropped item.

---

## Using Items in Fortnite Creative

**כותרת מקורית:** Using Items in Fortnite Creative  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/using-items-in-fortnite-creative  
**מקור קלט:** `08_Items_משאבים_ופריטי_משימה(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `using-items-in-fortnite-creative`

*

Items include things that can be consumed by players, devices, or weapons. There are also items that can be used as crafting materials. Crafting materials are items that can be exchanged for other usable items, or that can be used as a crafting piece for a larger item.

You can find a wide range of uses for these items. Find out more about the [items](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) available in Fortnite Creative and how you can use them!

 You can find items in [Content Browser](https://dev.epicgames.com/documentation/fortnite/exploring-the-content-browser-menu-in-fortnite-creative), in the [Items Category](https://dev.epicgames.com/documentation/fortnite/items-category) .

- [

Ammo Items

Use ammo items to restock weapons during gameplay.

](https://dev.epicgames.com/documentation/fortnite/using-ammo-items-in-fortnite-creative)
- [

Attack Items

Offer players creative ways to eliminate enemies.

](https://dev.epicgames.com/documentation/fortnite/using-attack-items-in-fortnite-creative)
- [

Crafting Items

Use crafting items as resources for players to collect and exchange during gameplay.

](https://dev.epicgames.com/documentation/fortnite/using-crafting-items-in-fortnite-creative)
- [

Crystal Crafting Items

Offer these items for players to collect during gameplay.

](https://dev.epicgames.com/documentation/fortnite/using-crystal-crafting-items-in-fortnite-creative)
- [

Dino Egg Crafting Items

Use these crafting items to create a theme that's dino-mite!

](https://dev.epicgames.com/documentation/fortnite/using-dino-egg-items-in-fortnite-creative)
- [

Disguise Items

Help players hide who they truly are with Disguise items.

](https://dev.epicgames.com/documentation/fortnite/using-disguise-items-in-fortnite-creative)
- [

Egg Items

Use Egg items to spring life to your island.

](https://dev.epicgames.com/documentation/fortnite/using-egg-items-in-fortnite-creative)
- [

Explosive Items

Offer these ranged attack items for an explosive gameplay.

](https://dev.epicgames.com/documentation/fortnite/using-explosive-items-in-fortnite-creative)
- [

Fish Items

Revive players and offer status buffs with these fishy items.

](https://dev.epicgames.com/documentation/fortnite/using-fish-items-in-fortnite-creative)
- [

Fishing Items

Get your fish on by using items that can reel in items from fishing zones.

](https://dev.epicgames.com/documentation/fortnite/using-fishing-items-in-fortnite-creative)
- [

Flopper Items

Offer these flopping items to aid players with status buffs during combat gameplay.

](https://dev.epicgames.com/documentation/fortnite/using-flopper-items-in-fortnite-creative)
- [

Food Crafting Items

Use these food items to collect and exchange for crafting.

](https://dev.epicgames.com/documentation/fortnite/using-food-crafting-items-in-fortnite-creative)
- [

Gold Items

Use Gold items to set currency requirements that will unlock devices and items.

](https://dev.epicgames.com/documentation/fortnite/using-gold-items-in-fortnite-creative)
- [

Grenade Items

Throw these items for an explosive variation of damage and status buffs.

](https://dev.epicgames.com/documentation/fortnite/using-grenade-items-in-fortnite-creative)
- [

Halloween Candy Items

Use the Halloween Candy items to offer players a temporary status boost.

](https://dev.epicgames.com/documentation/fortnite/using-halloween-candy-items-in-fortnite-creative)
- [

Healing Items

Use these items to replenish health during gameplay.

](https://dev.epicgames.com/documentation/fortnite/using-healing-items-in-fortnite-creative)
- [

Ice Cream Items

Serve these sweet treats for players to restore health and gain status buffs as they cool off.

](https://dev.epicgames.com/documentation/fortnite/using-ice-cream-items-in-fortnite-creative)
- [

Mechanical Crafting Items

Offer mechanical-themed crafting items on your island.

](https://dev.epicgames.com/documentation/fortnite/using-mechanical-crafting-items-in-fortnite-creative)
- [

Mineral Ore Crafting Items

Offer these items for players to collect and craft weapons and more.

](https://dev.epicgames.com/documentation/fortnite/using-mineral-ore-crafting-items-in-fortnite-creative)
- [

Mineral Powder Items

Offer powder-themed crafting items for players throughout gameplay.

](https://dev.epicgames.com/documentation/fortnite/using-mineral-powder-items-in-fortnite-creative)
- [

Produce Items

Refuel your player's energy by using these food-themed items.

](https://dev.epicgames.com/documentation/fortnite/using-produce-items-in-fortnite-creative)
- [

Nature Items

Gather nature-themed items like bacon or herbs as an island resource.

](https://dev.epicgames.com/documentation/fortnite/using-nature-items-in-fortnite-creative)
- [

Objective Items

Make your gameplay missions possible by using items that trigger objectives.

](https://dev.epicgames.com/documentation/fortnite/using-objective-items-in-fortnite-creative)
- [

Portable Items

Portable aids that can be thrown or equipped to assist combat gameplay.

](https://dev.epicgames.com/documentation/fortnite/using-portable-items-in-fortnite-creative)
- [

Power Crafting Items

Players can use these power supplies to keep their items charged!

](https://dev.epicgames.com/documentation/fortnite/using-power-crafting-items-in-fortnite-creative)
- [

Primal Crafting Items

Show off your wild side by using Primal items.

](https://dev.epicgames.com/documentation/fortnite/using-primal-crafting-items-in-fortnite-creative)
- [

Ranged Weapon Items

Go the distance by throwing these items that can aid in ranged attacks.

](https://dev.epicgames.com/documentation/fortnite/using-ranged-weapon-items-in-fortnite-creative)
- [

Restorative Items

Regenerate damaged health and shields with these cool items.

](https://dev.epicgames.com/documentation/fortnite/using-restorative-items-in-fortnite-creative)
- [

Shield Items

Give players a boost for protection in combat play.

](https://dev.epicgames.com/documentation/fortnite/using-shield-items-in-fortnite-creative)
- [

Shove Gameplay Item

Add the Shove item to give a unique action to players, that they can use to help or harm!

](https://dev.epicgames.com/documentation/fortnite/shove-gameplay-item-in-fortnite)
- [

Slap Items

Slap unlimited Energy into your life with these items.

](https://dev.epicgames.com/documentation/fortnite/using-slap-items-in-fortnite-creative)
- [

Trap Items

Use Trap items to offer aid in combat and building gameplay.

](https://dev.epicgames.com/documentation/fortnite/using-trap-items-in-fortnite-creative)
- [

Travel Items

Move in style with items that will get you from one place to another.

](https://dev.epicgames.com/documentation/fortnite/using-travel-items-in-fortnite-creative)
- [

Twine Crafting Items

Place twine items as a crafting resource for your island.

](https://dev.epicgames.com/documentation/fortnite/using-twine-crafting-items-in-fortnite-creative)
- [

Vehicle Mod Items

Trick out your vehicles with mod items.

](https://dev.epicgames.com/documentation/fortnite/using-vehicle-mod-items-in-fortnite-creative)
- [

Wild Edible Crafting Items

Edible items found in nature to collect and exchange for crafting.

](https://dev.epicgames.com/documentation/fortnite/using-wild-edible-crafting-items-in-fortnite-creative)
- [

World Resource Items

World Resources Items can be used as building materials or currency.

](https://dev.epicgames.com/documentation/fortnite/using-world-resource-items-in-fortnite-creative)

---

## Using Nature Items in Fortnite Creative

**כותרת מקורית:** Using Nature Items in Fortnite Creative  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/using-nature-items-in-fortnite-creative  
**מקור קלט:** `08_Items_משאבים_ופריטי_משימה(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `using-nature-items-in-fortnite-creative`

Use **Nature** [items](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) as [crafting](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#crafting) materials for items that can use ingredients. These items could also be required to unlock requirements for [devices](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#device) like the [**Conditional Button**](https://dev.epicgames.com/documentation/fortnite/using-conditional-button-devices-in-fortnite-creative).

You could pair **Adhesive Resin** with [mechanical items](https://dev.epicgames.com/documentation/fortnite/using-mechanical-crafting-items-in-fortnite-creative) as materials needed to craft usable items or weapons like the **Makeshift Revolver**.

Mechanical items are:

-
**Fibrous Herbs**

-
**Flower Petals**

-
**Planks**

-
**Bacon**

-
**Adhesive Resin**

-
**Duct Tape**

You can also blend items with [props](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#prop) of similar [themes](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary). Grant crafting items with a pair of devices like **Button** and **Item Granter** to blend them with similar props from the **Galleries** tab. For example, you can blend nature items with foliage and nature props from the **Galleries** tab to fully immerse players onto your island.

To create the process of crafting, you will need to either [spawn](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#spawning) or [grant](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#grant) items onto the map for players to collect with the **Item Spawner** or **Item Granter**.

The players can collect these items to exchange for usable items through item consuming devices like Conditional Button. They can also use these items to craft other items that will build up to a larger item.

Visit our [video tutorials](https://mediaspace.unrealengine.com/playlist/dedicated/208434573/1_gxu6mwv5/1_qfnz9w5c) to learn more about working with items and for tips to enhance gameplay.

### Finding and Placing Items

*Click image to enlarge.*

-
From **Build** mode, press the **Tab** key, then click **CREATIVE** on the [top navigation bar](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) to select the CREATIVE inventory screen if not already displayed.

-
Click the **CONSUMABLES** tab.

-
On this screen, scroll to find and select the item, use the **Search** box to look up the item by name, or check the list of relevant **Categories** specific to the item you're looking for to filter the view.

-
Click the item, then click either **EQUIP** or **ADD TO CHEST**.

Clicking EQUIP will add the item to your [Resources bar](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#resources-bar). (When you're back in Create mode, you can view items in your Resources bar by pressing the **Tab** key and selecting **Play**)

You may want to offer an item bundle to players through a [chest](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#chest) or [llama](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#llama). Selecting ADD TO CHEST will add the item to the [CHEST tab](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary). Each time you click ADD TO CHEST, the item count will increase by one, shown in a yellow box on the CHEST tab.

*Click image to enlarge.*

You can add up to fifteen items to the CHEST tab. When it’s full, the ADD TO CHEST tab will disappear. To add more items, you first have to remove items from the CHEST tab.

From the CHEST tab, you can select either CREATE CHEST or CREATE LLAMA to store the items in a Chest or a Llama for use [in-game](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#ingame).

### Managing Items

You can manage these items when you are in [Play inventory](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#play-inventory). To access the **Play** inventory screen, press **Tab** and click **Play** in the top navigation bar. In the **Play** inventory, you can create or split item stacks, or remove them entirely from your Resources bar.

*Click image to enlarge.*

Instead of dropping these items on the ground, it's best to grant them to players by using item-granting devices like the Item Spawner.

You cannot reposition or copy items with the phone tool. To delete an item from your inventory in Create mode, you will have to select either *Respawn* or *Back To Hub* from the *Menu*. When you do this, your inventory clears.

### Nature Items

 Item Use

**Fibrous Herbs**

Cab be used as a crafing ingredient for folige items like **Bush**.

**Flower Petals**

Can be used as a crafing ingredient for foliage items like **Cabbage**.

**Planks**

Can be used as a crafting ingredient for items like **Junk Rift**. .

**Bacon**

Can be used as a crafting ingredient for items like food items.

**Adhesive Resin**

Can be used as a crafting ingredient for weapons and other items like **Duct Tape**.

**Duct Tape**

Can be used as a crafting ingredient for weapons, traps, and other items.

### Registering Crafting Items to a Device

Some devices can hold or grant items. To [register](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#register) an item for this kind of device, follow these steps.

-
In the CREATIVE inventory, find the equipment and items you want to register with a device and equip them.

-
Stand directly beside the device that will register the item.

-
Press the **Tab** key to open the **PLAY** inventory screen.

-
Click the item, then press either **Z** or **X** to split or drop the item. You can also drag the item to the side until a [backpack icon](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#backpack-icon) appears.

The compatible device will automatically register the dropped item.

---

## Using Objective Items in Fortnite Creative

**כותרת מקורית:** Using Objective Items in Fortnite Creative  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/using-objective-items-in-fortnite-creative  
**מקור קלט:** `08_Items_משאבים_ופריטי_משימה(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `using-objective-items-in-fortnite-creative`

**Objective** [items](https://dev.epicgames.com/documentation/fortnite/fortnite-creative-glossary#items) can be used to grant players access to areas and unlock requirements for [in-game](https://dev.epicgames.com/documentation/fortnite/fortnite-creative-glossary#in-game) [objectives](https://dev.epicgames.com/documentation/fortnite/fortnite-creative-glossary#objective).

Objective items include:

**Jewel**

**Flag**

**Catty Corner Keycard**

**Fortilla Keycard**

**Grotto Keycard**

**Rig Keycard**

**Shark Keycard**

**Authority Keycard**

**Key**

Create objectives for players to unlock once by equipping these items.

You can create game modes like capture the flag and [jewel thief](https://dev.epicgames.com/documentation/fortnite/fortnite-creative-glossary#jewel-thief) by pairing the [**Item Spawner**](https://dev.epicgames.com/documentation/fortnite/using-item-spawner-devices-in-fortnite-creative) and [**Capture Area**](https://dev.epicgames.com/documentation/fortnite/using-capture-area-devices-in-fortnite) with these items.

You can also use the [**Conditional Button**](https://dev.epicgames.com/documentation/fortnite/using-conditional-button-devices-in-fortnite-creative) and require players to unlock doors with Objective items.

### Finding and Placing Items

Click image to enlarge.

From [**Build** mode](https://dev.epicgames.com/documentation/fortnite/fortnite-creative-glossary#create-mode), press the **Tab** key, then click **CREATIVE** on the [top navigation bar](https://dev.epicgames.com/documentation/fortnite/fortnite-creative-glossary#topnavigationbar) to select the [CREATIVE inventory](https://dev.epicgames.com/documentation/fortnite/fortnite-creative-glossary#creativeinventory) screen if not already displayed.

Click the **CONSUMABLES** tab.

Scroll to find and select the item, use the **Search** box to look up the item by name, or check the list of relevant **Categories** specific to the item you're looking for to filter the view.

Click the item, then click either **Equip** or **Add To Chest**.

Clicking **Equip** will add the item to your [Equipment bar](https://dev.epicgames.com/documentation/fortnite/fortnite-creative-glossary#equipmentbar).

When you're back in [Create mode](https://dev.epicgames.com/documentation/fortnite/fortnite-creative-glossary#create-mode), you can view any items you've [equipped](https://dev.epicgames.com/documentation/fortnite/fortnite-creative-glossary#equip) by pressing the **F** key. You can select equipped items by either scrolling your middle mouse button or by pressing its corresponding number on your keyboard.

From the [**Chest**](https://dev.epicgames.com/documentation/fortnite/fortnite-creative-glossary#chesttab) tab, you can select either **Create Chest** or **Create Llama** to store the items in a [chest](https://dev.epicgames.com/documentation/fortnite/fortnite-creative-glossary#chest) or a [llama](https://dev.epicgames.com/documentation/fortnite/fortnite-creative-glossary#llama) for use [in-game](https://dev.epicgames.com/documentation/fortnite/fortnite-creative-glossary#in-game).

Click image to enlarge.

Chests and llamas are a great way to offer item bundles to players. Selecting **Add To Chest** will add the item to the [**Chest** tab](https://dev.epicgames.com/documentation/fortnite/fortnite-creative-glossary#chesttab). Each time you click **Add To Chest**, the item count will increase by one, shown as a yellow box on the Chest tab.

You can add up to fifteen items to the **Chest** tab. When it’s full, the **Add To Chest** tab will disappear. To add more items, you first have to remove items from the **Chest** tab.

There are many ways for you to offer these items to players. Use any of the devices under the [Registering Items](https://dev.epicgames.com/documentation/fortnite/using-objective-consumables-in-fortnite-creative#registeringitems) section to either offer or require these items during gameplay.

### Managing Items

You can manage these items when you are in [**Play** inventory](https://dev.epicgames.com/documentation/fortnite/fortnite-creative-glossary#play-inventory). To access the **Play** inventory screen, press **Tab** and click **Play** in the top navigation bar. Here, you can swap item positions or drop them from your Equipment bar.

You cannot reposition or copy items with the phone tool. To delete an item from your inventory in Create mode, you will have to select either *Respawn* or *Back To Hub* from the *Menu*. When you do this, your inventory clears.

### Using Objective Items

Use these items to fulfill objective requirements.

 Item
 Usage

 **Jewel**
 Can be used in capture objectives. Players with this item equipped will have a Jewel backpack. Equips one at a time.

 **Flag**
 Can be used in capture objectives. This item can also be used as a melee weapon. Equips one at a time.

 **Catty Corner Keycard**
 Themed to unlock areas for the Catty Corner area. Equips one at a time.

 **Fortilla Keycard**
 Themed to unlock areas for the Fortilla area. Equips one at a time

 **Grotto Keycard**
 Themed to unlock areas for the Grotto area. Equips one at a time.

 **Rig Keycard**
 Themed to unlock areas for the Rig area. Equips one at a time.

 **Shark Keycard**
 Themed to unlock areas for the Shark area. Equips one at a time.

 **Authority Keycard**
 Themed to unlock areas for the Authority area. Equips one at a time.

 **Key**
 Themed as a key to unlock items like the Conditional Button.

### Registering Items

You can drop items directly onto devices that can either hold or [grant](https://dev.epicgames.com/documentation/fortnite/fortnite-creative-glossary#grant) items. You must [register](https://dev.epicgames.com/documentation/fortnite/fortnite-creative-glossary#register) these items to save in the device's memory.

To register items to a device, stand directly on or immediately beside the device.

To register an item for this kind of device, follow these steps. You can also watch a [video tutorial](https://mediaspace.unrealengine.com/media/RegisteringCraftingConsumablesinFortniteCreative/1_zpmj3v0g) that shows you how to register items, both crafting and usable.

In the CREATIVE inventory, find the equipment and items you want to register with a device and equip them.

In Create mode, stand directly beside the device that will register the item.

Press the **Tab** key to open the **PLAY** inventory screen.

Click the item, then press either **Z** or **X** to split or drop the item. You can also drag the item to the side until a [backpack icon](https://dev.epicgames.com/documentation/fortnite/fortnite-creative-glossary#backpack-icon) appears.

The compatible device will automatically register the dropped item. Compatible devices that can hold items include:

**Vending Machine**

**Team Settings & Inventory**

**Class Designer**

**Capture Item Spawner**

**Capture Area**

**Item Granter**

**Item Spawner**

**Conditional Button**

**Elimination Manager**

**Item Remover**

Use these devices to set up your own system for granting and spawning items onto your island.

### Using Items for Crafting

You can pair items with each other and with weapons to create the process of [crafting](https://dev.epicgames.com/documentation/fortnite/fortnite-creative-glossary#crafting), where players exchange items for another.

To do so, you can choose from the list of compatible devices above like the [**Conditional Button**](https://dev.epicgames.com/documentation/fortnite/using-conditional-button-devices-in-fortnite-creative) and [**Item Spawner**](https://dev.epicgames.com/documentation/fortnite/using-item-spawner-devices-in-fortnite-creative) to set up the crafting process.

For example, you can require [**Rainbow Crystals**](https://dev.epicgames.com/documentation/404) and [**Malachite Ore**](https://dev.epicgames.com/documentation/404) as items needed to craft **Jewels**.

Visit our [video tutorials](https://mediaspace.unrealengine.com/playlist/dedicated/208434573/1_gxu6mwv5/1_qfnz9w5c) to learn more about working with items and for tips to enhance gameplay.

---

## Using Travel Items in Fortnite Creative

**כותרת מקורית:** Using Travel Items in Fortnite Creative  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/using-travel-items-in-fortnite-creative  
**מקור קלט:** `08_Items_משאבים_ופריטי_משימה(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `using-travel-items-in-fortnite-creative`

**Travel [items](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary)** can move players across the map in various ways. Players can equip these items to traverse the map faster or escape combat.

Travel items include:

-
**Crash Pad**

-
**Inflate-A-Bull**

-
**Balloons**

-
**Gliders**

-
**Jules’ Glider Gun**

-
**Skye’s Grapper**

-
**Grappler**

-
**Jetpack**

### Finding and Placing Items

*Click image to enlarge.*

-
From [Build mode](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#create-mode), press the **Tab** key, then click **CREATIVE** on the [top navigation bar](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) to select the [CREATIVE inventory](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) screen if not already displayed.

-
Click the **CONSUMABLES** tab.

-
Scroll to find and select the item, use the **Search** box to look up the item by name, or check the list of relevant **Categories** specific to the item you're looking for to filter the view.

-
Click the item, then click either **Equip** or **Add To Chest**.

Clicking **Equip** will add the item to your [Equipment bar](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary).

When you're back in [Create mode](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#create-mode), you can view any items you've [equipped](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) by pressing the **F** key. You can select equipped items by either scrolling your middle mouse button or by pressing its corresponding number on your keyboard.

From the [Chest](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) tab, you can select either **Create Chest** or **Create Llama** to store the items in a [chest](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#chest) or a [llama](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#llama) for use [in-game](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#ingame).

*Click image to enlarge.*

Chests and llamas are a great way to offer item bundles to players. Selecting **Add To Chest** will add the item to the **Chest** tab. Each time you click **Add To Chest**, the item count will increase by one, shown as a yellow box on the Chest tab.

You can add up to fifteen items to the **Chest** tab. When it’s full, the **Add To Chest** tab will disappear. To add more items, you first have to remove items from the **Chest** tab.

There are many ways for you to offer these items to players. Use the devices under the [Registering Items](https://dev.epicgames.com/documentation/fortnite/using-travel-items-in-fortnite-creative#registering-items) section to either offer or require these items during gameplay.

### Managing Items

You can manage these items when you are in [Play inventory](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#play-inventory). To access the **Play** inventory screen, press **Tab** and click **Play** in the top navigation bar. Here, you can swap item positions or drop them from your Equipment bar.

You cannot reposition or copy items with the phone tool. To delete an item from your inventory in Create mode, you will have to select either *Respawn* or *Back To Hub* from the *Menu*. When you do this, your inventory clears.

### Using Travel Items

Use these items as an aid to travel across the map.

 Item Usage

**Crash Pad**

Like the [**Crash Pad**](https://dev.epicgames.com/documentation/fortnite/using-crash-pad-devices-in-fortnite-creative) device, players can bounce and launch themselves to a desired direction with no fall damage. Vehicles and projectiles like grenades and rockets will also bounce when touching this item. Crash Pads can be equipped in stacks of six and deflates after 60 seconds.

**Inflate-A-Bull**

Players can traverse the map in an inflatable cow suit. This item is a deployable backpack that allows players to moo, bounce, and roll with speed. This item will permanently deflate after two minutes or temporarily when attacked. Can be equipped one item at a time.

**Balloon**

Players can glide in various directions while jumping. This item is equipped in stacks of ten and can be individually detached when needed.

**Gliders**

With the setting **Glider Redeploy** as **Off** in the **My Island - Settings** tab, players can use this item to glide when falling from high altitudes. Gliders can be equipped in stacks of ten and will take on the appearance of Gliders equipped from their **Locker**.

**Jules’ Glider Gun**

Similar to the **Grappler**, this item launches a plunger that pulls players to their location of choice. When being pulled to high altitudes, an **Ohm Glider** will automatically deploy, allowing players to travel further and take no fall damage. This item has infinite uses.

**Skye’s Grappler**

This item launches a plunger that pulls players to their location of choice. Unlike **Jules’ Grappler Gun**, this item can cause fall damage since it does not automatically deploy a glider. Successfully connecting a shot with a surface allows players to reset their fall distance. This item has infinite uses and a slightly delayed cooldown.

**Grappler**

This item launches a plunger that pulls players to a desired location. Successfully connecting a shot with a surface allows players to reset their fall distance. This item equips in stacks of ten.

**Jetpack**

Through short bursts, blasts players into the air with the potential to cause fall damage if overheated. Players can gauge their **Jetpack’s** meter from the multicolored bars on their backpack. Can be equipped one at a time.

**Grapple Glider**

Launches a plunger that pulls players to a desired location and automatically deploys an equipped glider to negate fall damage. This item can be used up to 10 times.

### Registering Items

You can drop items directly onto devices that can either hold or grant items. You must [register](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#register) these items to save in the device's memory.

To register items to a device, you must stand directly on or immediately beside the device.

To register an item for this kind of device, follow these steps. You can also watch a [video tutorial](https://mediaspace.unrealengine.com/media/RegisteringCraftingConsumablesinFortniteCreative/1_zpmj3v0g) that shows you how to register items, both crafting and usable.

-
In the CREATIVE inventory, find the equipment and items you want to register with a device and equip them.

-
In Create mode, stand directly beside the device that will register the item.

-
Press the **Tab** key to open the **PLAY** inventory screen.

-
Click the item, then press either **Z** or **X** to split or drop the item. You can also drag the item to the side until a [backpack icon](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#backpack-icon) appears.

The compatible device will automatically register the dropped item. Compatible devices that can hold items include:

-
**Vending Machine**

-
**Team Settings & Inventory**

-
**Class Designer**

-
**Capture Item Spawner**

-
**Item Granter**

-
**Item Spawner**

-
**Conditional Button**

-
**Elimination Manager**

-
**Item Remover**

Use these devices to set up your own system for granting and spawning items onto your island.

### Using Items for Crafting

You can pair items with each other and weapons to create the process of crafting, where players exchange items for another.

To do so, you can choose from the list of compatible devices above like the [**Conditional Button**](https://dev.epicgames.com/documentation/fortnite/using-conditional-button-devices-in-fortnite-creative) and [**Item Spawner**](https://dev.epicgames.com/documentation/fortnite/using-item-spawner-devices-in-fortnite-creative) to set up the crafting process.

For example, you can require **Balloons** and [****](https://www.epicgames.com/fortnite/en-US/creative/docs/using-mechanical-consumables-in-fortnite-creative)**[Sturdy Mechanical Parts](https://dev.epicgames.com/documentation/fortnite/using-mechanical-crafting-items-in-fortnite-creative)** as items needed to craft a **Jetpack**.

Visit our [video tutorials](https://mediaspace.unrealengine.com/playlist/dedicated/208434573/1_gxu6mwv5/1_qfnz9w5c) to learn more about working with items and for tips to enhance gameplay.

---

## Using World Resource Items in Fortnite Creative

**כותרת מקורית:** Using World Resource Items in Fortnite Creative  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/using-world-resource-items-in-fortnite-creative  
**מקור קלט:** `08_Items_משאבים_ופריטי_משימה(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `using-world-resource-items-in-fortnite-creative`

You can use **world resource** [items](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) as building materials or as currency for devices like the Conditional Button.

World Resource items are:

-
**Wood**

-
**Stone**

-
**Metal**

While [in-game](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#ingame), you can offer these resources throughout the world for players to gather by using devices like the **Item Spawner** or **Item Granter**.

Through the [My Island - Settings menu](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary), you can adjust multiple settings that can alter resource allocations for your island. You can also change settings like **Infinite Resources** to determine whether resouces will be unlimited or not.

These world resources can be used as building materials for game modes like Zone Wars.

You could also require these resources as a currency for devices like the Item Spawner and [Vending Machine](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#vending-machine). The set requirements will show on a HUD message near the device.

### Finding and Placing World Resource Items

*Click image to enlarge.*

-
From [Build mode](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#create-mode), press the **Tab** key, then click **CREATIVE** on the [top navigation bar](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) to select the [CREATIVE inventory](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) screen if not already displayed.

-
Click the **CONSUMABLES** tab.

-
On this screen, scroll to find and select the item, use the **Search** box to look up the item by name, or check the list of relevant **Categories** specific to the item you're looking for to filter the view.

-
Click the item, then click either **EQUIP** or **ADD TO CHEST**.

Clicking EQUIP will add the item to your [Resources bar](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#resources-bar). (When you're back in Create mode, you can view items in your Resources bar by pressing the **Tab** key and selecting **Play**)

You may want to offer an item bundle to players through a [chest](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#chest) or [llama](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#llama). Selecting ADD TO CHEST will add the item to the [CHEST tab](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary).

Each time you click ADD TO CHEST, the item count will increase by one, shown in a yellow box on the CHEST tab.

You can add up to fifteen items to the CHEST tab. When it’s full, the ADD TO CHEST tab will disappear. To add more items, you first have to remove items from the CHEST tab.

### Managing Items

You can manage these items when you are in [Play inventory](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#play-inventory). To access the **Play** inventory screen, press **Tab** and click **Play** in the top navigation bar. In the **Play** inventory screen, you can create or split item stacks, or remove them entirely from the Resources bar.

*Click image to enlarge.*

Instead of dropping these items on the ground, it's best to grant them to players by using item-granting devices like the Item Spawner.

You cannot reposition or copy items with the phone tool. To delete an item from your inventory in Create mode, you will have to select either *Respawn* or *Back To Hub* from the *Menu*. When you do this, your inventory clears.

### Registering Items

Some devices can hold or grant items. To [register](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#register) an item for this kind of device, follow these steps.

-
In CREATIVE inventory, find the equipment and items you want to register with a device and equip them.

-
In Create mode, stand directly beside the device that will register the item.

-
Press the **Tab** key to open the **PLAY inventory** screen.

-
Click the item, then press either **Z** or **X** to split or drop the item. You can also drag the item to the side until a [backpack icon](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#backpack-icon) appears.

The compatible device will automatically register the dropped item.
