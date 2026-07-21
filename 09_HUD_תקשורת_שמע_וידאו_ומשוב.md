# HUD, תקשורת, שמע, וידאו ומשוב

> **מטרת הקובץ:** לרכז את דרכי הצגת המידע לשחקן באמצעות HUD, הודעות, סימוני עולם, דיאלוגים, שמע ווידאו.  
> **מתי להשתמש בו:** כאשר צריך להסביר מטרה, לתת משוב, להציג מידע או לעצב תקשורת חזותית וקולית.  
> **לא כלול:** תאורת עולם, VFX סביבתיים ו־AI.  
> **מקורות עיקריים:** `07E_HUD_תקשורת_שמע_וידאו_ומשוב(1).md`

## תוכן עניינים

- [Using Audio Mixer Devices in Fortnite Creative](#using-audio-mixer-devices-in-fortnite-creative)
- [Using Audio Player Devices in Fortnite Creative](#using-audio-player-devices-in-fortnite-creative)
- [Using Beacon Devices in Fortnite Creative](#using-beacon-devices-in-fortnite-creative)
- [Using Billboard Devices in Fortnite Creative](#using-billboard-devices-in-fortnite-creative)
- [Using HoloScreen Devices in Fortnite Creative](#using-holoscreen-devices-in-fortnite-creative)
- [Using HUD Controller Devices in Fortnite Creative](#using-hud-controller-devices-in-fortnite-creative)
- [Using HUD Message Devices in Fortnite Creative](#using-hud-message-devices-in-fortnite-creative)
- [Using Map Indicator Devices in Fortnite Creative](#using-map-indicator-devices-in-fortnite-creative)
- [Using Message Feed Devices in Fortnite Creative](#using-message-feed-devices-in-fortnite-creative)
- [Using Pop-up Dialog Devices in Fortnite Creative](#using-pop-up-dialog-devices-in-fortnite-creative)
- [Using Video Player Devices in Fortnite Creative](#using-video-player-devices-in-fortnite-creative)

---
## Using Audio Mixer Devices in Fortnite Creative

**כותרת מקורית:** Using Audio Mixer Devices in Fortnite Creative  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/using-audio-mixer-devices-in-fortnite-creative  
**מקור קלט:** `07E_HUD_תקשורת_שמע_וידאו_ומשוב(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `using-audio-mixer-devices-in-fortnite-creative`

**
You can use the **Audio Mixer** device to adjust the volume for groups of sounds. This gives you dynamic and automatic control of a game’s volume mix, much like a professional mixing console would.

With the Audio Mixer, you can adjust the volume level of sounds that are already in Fortnite (such as weapons, character footsteps, and vehicles). If you work on your island as a [project](https://dev.epicgames.com/documentation/en-us/uefn/unreal-editor-for-fortnite-glossary#project) in Unreal Editor for Fortnite (UEFN), you can create custom sound waves and sound cues that can be controlled with the Audio Mixer as well. See [Audio Mixer Device page](https://dev.epicgames.com/documentation/en-us/uefn/audio-mixer-in-unreal-editor-for-fortnite) in the UEFN documentation for more information about using the device in UEFN.

To find the Audio Mixer** device, see [Using Devices](https://dev.epicgames.com/documentation/en-us/fortnite-creative/using-devices-in-fortnite-creative).

### Control Bus

In UEFN, the [**control bus**](https://dev.epicgames.com/documentation/en-us/uefn/unreal-editor-for-fortnite-glossary#control-bus) is a way to control certain parameters for one or more sounds. There are several control buses set up to control the volume of the sounds that occur in Fortnite by default. If you don't have a [control bus mix](https://dev.epicgames.com/documentation/en-us/uefn/unreal-editor-for-fortnite-glossary#control-bus-mix) set up, or you aren't using UEFN to work on your island, you can choose a default control bus using the **Bus** option in the Audio Mixer device options. The following table lists the default control buses available.

If you want to control the volume of multiple buses in Creative, you'll need to place an Audio Mixer device for each bus you want to control.

 Control Bus Name Description
**Music**

Used to set the volume of music (this includes emote music).

**SFX**

Used to set the volume of all sound effects.

**Ambience**

Used to set the volume of ambient sounds.

**Explosions**

Used to set the volume of explosion sounds.

**Footsteps**

Used to set the volume of character footsteps.

**Gadgets**

Used to set the volume of sounds associated with Creative gadgets and devices.

**Impacts**

Used to set the volume of impact sounds.

**Vehicles**

Used to set the volume of vehicle sounds (except for engine sounds).

**Vehicle Engines**

Used to set the volume of vehicle engines.

**Weapons**

Used to set the volume of weapons.

If you have a control bus mix set on the Audio Mixer device in UEFN, the **Bus** setting on the device in Creative becomes deactivated. While editing the island in Creative, you will still see the Bus option and you can select a bus, but this will not actually have an effect.

### Registering Players

You can [register](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) and unregister players to the Audio Mixer device, which allows you to choose who should hear the mix that the Audio Mixer controls. Registering or unregistering players is done using direct event binding. See the **Direct Event Binding** section for more information.

### Device Options

In the device's **Customize** panel, you can find a limited group of options in the **Basic Options** tab. If you want to see all available options, click the **All Options** tab. This section lists and describes all available device options.

Default values are **bold**.

**אפשרויות, ערכים ותיאורים:**

##### Bus

- **Value / Values:** Select one of the following default control buses:
- **Description:** -
Music

#### -
SFX

- **Value / Values:** -
Ambience
- **Description:** -
Explosions

#### -
Footsteps

- **Value / Values:** -
Gadgets
- **Description:** -
Impacts

#### -
Vehicles

- **Value / Values:** -
Vehicle Engines
- **Description:** -
Weapons

#### -
Jam

- **Value / Values:** -
Patchwork
- **Description:** Each control bus controls a different group of sounds in Fortnite. See the **Control Bus** section above for more information.

##### Fader Value

- **Value / Values:** **1.0**, Pick a value
- **Description:** This sets the volume of the default control bus selected in the **Bus** option. There are ten values, from **0** (completely silent) to the default of **1.0** (full volume).

##### Can Be Heard By

- **Value / Values:** None, Registered Players, Non-Registered Players, **Everyone**
- **Description:** This determines what group of people will be affected by the settings of this Audio Mixer. You can use functions to register or unregister players.

##### Activate in Edit Mode

- **Value / Values:** On, **Off**
- **Description:** When set to **On**, the device will automatically activate when you are editing your island.

##### Activate at Game Start

- **Value / Values:** On, **Off**
- **Description:** When set to **On**, the device will automatically activate when the game starts.

### Direct Event Binding

**Direct event binding** allows devices to communicate directly, which makes your workflow more intuitive, and gives you more freedom to focus on your design ideas.

Below are the functions and events for this device.

#### Functions

A [**function**](https://dev.epicgames.com/documentation/en-us/fortnite-creative/fortnite-creative-glossary#function) listens for an event on a device then performs an action.

-
For any function, click the option, then Select Device to access and select from the Device dropdown menu.

-
Once you've selected a device, click Select Event and select the event that triggers this function.

-
If more than one device or event triggers a function, press the Add button to add a line and repeat these steps.

**אפשרויות ותיאורים:**

##### Activate Mix When Receiving From

When an event occurs, this function activates the mix controlled by this device.

##### Deactivate Mix When Receiving From

When an event occurs, this function deactivates the mix controlled by this device.

##### Register Player When Receiving From

When an event occurs, this function registers the triggering player to this device.

##### Unregister Player When Receiving From

When an event occurs, this function unregisters the triggering player from this device.

##### Unregister All Players When Receiving From

When an event occurs, this function unregisters all players from this device.

#### Events

This device has no events.

---

## Using Audio Player Devices in Fortnite Creative

**כותרת מקורית:** Using Audio Player Devices in Fortnite Creative  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/using-audio-player-devices-in-fortnite-creative  
**מקור קלט:** `07E_HUD_תקשורת_שמע_וידאו_ומשוב(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `using-audio-player-devices-in-fortnite-creative`

Use the Audio Player device to play special sound effects during your game. Choose from a large number of one-time sound effects.

If you are using UEFN, you can also create custom audio and map it to this device. See [Audio Player Device](https://dev.epicgames.com/documentation/en-us/uefn/using-audio-player-devices-in-unreal-editor-for-fortnite) for more information.

### Contextual Filtering

Some devices are affected by a feature called **contextual filtering**. This feature hides or displays options depending on the values selected for certain related options. This reduces clutter in the Customize panel and makes options easier to manage and navigate. To help identify them, values that trigger contextual filtering are in *italic*.

All options are listed, including those affected by contextual filtering; if they are hidden or displayed based on a specific option's value, there will be a note about it in the Description field for that option.

### Device Options

text here

**אפשרויות, ערכים ותיאורים:**

##### Enabled During Phase

- **Value / Values:** Always, None, Pre-Game Only, Gameplay Only, Create Only
- **Description:** Determines which phases in which the device is enabled.

##### Restart Audio when Activated

- **Value / Values:** On, **Off**
- **Description:** Determines whether the audio will restart when it is triggered to play. If this is set to **Off**, activations will be ignored if audio is already playing.

##### Audio

- **Value / Values:** Pick an audio cue or sound effect
- **Description:** This is the cue or sound effect that plays when the device is activated.

##### Volume

- **Value / Values:** **1.0**, Select a Volume
- **Description:** Sets the volume for the audio. This is a linear setting, so 0.5 is half as loud and 2.0 is twice as loud as the source audio volume.

##### Visible in Game

- **Value / Values:** On, Off
- **Description:** Determines whether the device will be visible during the game.

##### Play on Hit

- **Value / Values:** On, Off
- **Description:** Determines whether the audio will play when the device is hit by the player.

##### Can be Heard By

- **Value / Values:** **Everyone**, Instigator Only, Registered Players Only, Non-Registered Players Only
- **Description:** Determines who will be able to hear audio from this device.

##### Play Location

- **Value / Values:** **Device**, Local Player, Registered Players, Instigating Players
- **Description:** Determines if the audio should be played from the device location, or the location of a player.

##### Playback Speed

- **Value / Values:** **1.0**, Select a Play Rate
- **Description:** Raises or lowers the pitch of the audio by changing the playback speed. 2.0 is twice as fast, 0.5 is half-speed as the source audio volume.

##### Fade In Duration

- **Value / Values:** **0.0**, Select a Duration
- **Description:** The time it takes the sound to reach full volume in seconds when the device is triggered to play.

##### Fade Out Duration

- **Value / Values:** **0.0**, Select a Duration
- **Description:** The time it takes the sound to reach full volume in seconds when the device is triggered to stop.

##### Mesh

- **Value / Values:** **Speaker**, Loudspeaker
- **Description:** Determines the visual appearance of the device's mesh.

##### Enable Spatialization

- **Value / Values:** ***On***, Off
- **Description:** Enables audio panning based on position relative to the listener. If this is set to **Off**, the **Stereo Spread** option is not displayed.

##### Stereo Spread

- **Value / Values:** **0.0**, Pick an amount
- **Description:** This option only displays if the **Enable Spatialization** option is set to **On**. This setting sets the distance between the virtual left and right speakers, with the play location at the center of the spread.

##### Enable Volume Attenuation

- **Value / Values:** *On*, Off
- **Description:** Enables volume changes based on the device's proximity to the listener. Source audio will become quieter the further the listener is from the location of the sound. If this is set to **Off**, several attenuation options are not displayed.

##### Attenuation Function

- **Value / Values:** **Linear**, Logarithmic
- **Description:** Defines the mapping function between the value of the **Attenuation Min** **Distance** option and the value of the **Attenuation Falloff** **Distance** option.

##### Attenuation Min Distance

- **Value / Values:** **4.0**, Set a Distance
- **Description:** The range in which the audio will remain at the value set in the **Volume** setting.

##### Attenuation Falloff Distance

- **Value / Values:** **32.0**, Set a Distance
- **Description:** The range from the **Attenuation Min Distance** over which the sound will go from the value set in the **Volume** option to silent.

##### Enable Attenuation Visuals

- **Value / Values:** On, Off
- **Description:** If this is set to **On**, there are visual effects.

##### Sync Player Audio

- **Value / Values:** On, **Off**
- **Description:** Determines whether the audio played is synchronized for all player devices. This is best used when you are playing a longer audio piece, such as music or dialogue.

##### Auto Play - Create

- **Value / Values:** On, **Off**
- **Description:** If this is set to **On**, the chosen audio will automatically play during Create Mode.

##### Auto Play - Waiting For Players

- **Value / Values:** On, **Off**
- **Description:** If this is set to **On**, the chosen audio will automatically play during the Waiting For Players phase.

##### Auto Play - Countdown

- **Value / Values:** On, **Off**
- **Description:** If this is set to **On**, the chosen audio will automatically play during the Countdown phase.

##### Auto Play - Gameplay

- **Value / Values:** On, **Off**
- **Description:** If this is set to **On**, the chosen audio will automatically play during the game.

##### Auto Play - Round End

- **Value / Values:** On, **Off**
- **Description:** If this is set to **On**, the chosen audio will automatically play when a round ends.

##### Auto Play - Game End

- **Value / Values:** On, **Off**
- **Description:** If this is set to **On**, the chosen audio will automatically play when the

### Direct Event Binding

 Following are the direct event binding options for this device.

#### Functions

A [function](https://dev.epicgames.com/documentation/fortnite/function) listens for an event on a device, and then performs an action.

-
For any function, click the option, then Select Device to access and select from the Device dropdown menu.

-
Once you've selected a device, click Select Event to bind the device to an event that will trigger the function for the device.

-
If more than one device or event triggers a function, click the Add button to add a line and repeat these steps.

**אפשרויות ותיאורים:**

##### **Play **When Receiving From

Plays the selected audio when an event occurs.

##### Stop When Receiving From

Stops the audio when an event occurs.

##### **Enable **When Receiving From

Enables the device when an event occurs.

##### **Disable **When Receiving From

Disables the device when an event occurs.

##### **Register Player **When Receiving From

When an event occurs, the player is registered as a target for the audio player.

##### **Unregister ****Player **When Receiving From

When an event occurs, the player is unregistered as a target for the audio player.

##### **Unregister ****All ****Players **When Receiving From

When an event occurs, all players are unregistered as targets for the audio player.

#### Events

This device has no events.

---

## Using Beacon Devices in Fortnite Creative

**כותרת מקורית:** Using Beacon Devices in Fortnite Creative  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/using-beacon-devices-in-fortnite-creative  
**מקור קלט:** `07E_HUD_תקשורת_שמע_וידאו_ומשוב(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `using-beacon-devices-in-fortnite-creative`

**
The **beacon** provides several types of beacons that can use different particle effects in different colors. They can all be used to mark a location in the world, either with the particle effect or a HUD marker.

In **Beacon** mode, the beacon will show one of several particle effects in one of several colors. In **Badge** mode, it will show a HUD Marker with multiple customization options for the color and text shown. The text shown can be different based on the team relationship with the local client.

To find the Beacon** device, see [Using Devices](https://dev.epicgames.com/documentation/fortnite/using-devices-in-fortnite).

If you're using multiple copies of a device on an island, it can be helpful to [rename](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) them. Choosing names that relate to a device's purpose makes it easier to remember what each one does, and easier to find a specific device when using the [Event Browser](https://dev.epicgames.com/documentation/fortnite/event-browser-in-fortnite-creative).

### Contextual Filtering

Some devices are affected by a feature called **contextual filtering**. This feature hides or displays options depending on the values selected for certain related options. This reduces clutter in the Customize panel and makes options easier to manage and navigate. To help identify them, values that trigger contextual filtering are in *italic*.

All options are listed, including those affected by contextual filtering; if they are hidden or displayed based on a specific option's value, there will be a note about it in the Description field for that option.

### Device Options

The device can either show a beacon in the world view, a badge in the HUD, or both. It can be configured with a variety of particle effects and text, depending on the team of players viewing it.

In its default state the beacon shows one of several particle effects, depending on which beacon is chosen.

You can configure this device with the following options.

Default values are **bold**. Values that trigger contextual filtering are *italic*.

**אפשרויות, ערכים ותיאורים:**

##### Beacon To Show

- **Value / Values:** ***Particle***, *Badge*, *Both*
- **Description:** Determines if the beacon displays its particle effect, the HUD Marker (Badge) or both.

##### Beacon Particle Style

- **Value / Values:** Arrow, **Light Beam**, Flare
- **Description:** This only displays if the **Beacon to Show** option is set to **Particle** or **Both**. Determines what visual effect would be shown to players.

##### Badge UI Style

- **Value / Values:** **Default**, Backless
- **Description:** This option only displays if the **Beacon to Show** option is set to **Badge** or **Both**. Determines the visual style for the badge.

##### Friendly Team

- **Value / Values:** Any, Hostiles, **Neutral**, Pick or enter a team
- **Description:** This determines which team, if any, sees the badge as friendly.

##### Friendly Class

- **Value / Values:** No Class, **Any**, Pick or enter a class
- **Description:** Determines which class sees the beacon as friendly. If you choose **No Class** only players with no assigned class are seen as friendly.

##### Invert Class Selection

- **Value / Values:** On, **Off**
- **Description:** If this is set to **On**, all classes except the one selected in **Friendly Class** are seen as friendly.

##### Team Visibility

- **Value / Values:** None, **Any**, Hostile, Friendlies, Neutral, Pick or enter a team
- **Description:** Determines which team can see the beacon.

##### Beacon Color

- **Value / Values:** ***Direct Color***, Team Color, Team Relationship Color
- **Description:** Determines the beacon color. If you choose **Direct Color**, the **Custom Beacon Color** option displays below this one.

##### Custom Beacon Color

- **Value / Values:** **White**, Pick a color swatch
- **Description:** This option only displays if the **Beacon Color** option is set to **Direct Color**. Determines the color of the beacon. Click the swatch to open the Color Picker. Select a color, then click the checkmark to close the Color Picker.

##### Enabled on Phase

- **Value / Values:** None, **Always**, Pre-Game Only, Gameplay Only
- **Description:** Determines the game phase during which the device will be enabled.

##### Badge Uses Beacon Color

- **Value / Values:** On, **Off**
- **Description:** If set, the badge will inherit color from the beacon rather than using the Team Relationship color.

##### Icon Identifier

- **Value / Values:** **None**, Pick an icon
- **Description:** This only displays when the **Beacon to Show** option is set to **Badge** or **Both**. Assigns an icon to the badge, making it identifiable. Click to open the Icon Picker. Select an icon, then click the checkmark to close the Icon Picker.

##### Hide HUD Icon At

- **Value / Values:** **20M**, Pick or enter a distance
- **Description:** If the beacon shows a HUD marker, only show the HUD marker to players who are closer than this distance from the device. This only displays when the **Beacon to Show** option is set to **Badge** or **Both**.

##### Display Distance Text

- **Value / Values:** On, ***Off***
- **Description:** If the beacon shows a HUD marker, this determines whether the HUD also shows the distance between the player and the beacon. This only displays when the **Beacon to Show** option is set to **Badge** or **Both**.

##### Friendly Icon Text

- **Value / Values:** Enter text (30 character limit)
- **Description:** Specifies the text displayed on the badge for friendly players. This only displays when the **Beacon to Show** option is set to **Badge** or **Both**.

##### Neutral Icon Text

- **Value / Values:** Enter text (30 character limit)
- **Description:** Specifies the text displayed on the badge for neutral players. This only displays when the **Beacon to Show** option is set to **Badge** or **Both**.

##### Hostile Icon Text

- **Value / Values:** Enter text (30 character limit)
- **Description:** Specifies the text displayed on the badge for hostile players. This only displays when the **Beacon to Show** option is set to **Badge** or **Both**.

##### Text Font Style

- **Value / Values:** Subtle, **Bold**
- **Description:** Defines the font for any custom text displayed by this beacon. This only displays when the **Beacon to Show** option is set to **Badge** or **Both**.

##### HUD Text Size

- **Value / Values:** **1.0X**, Pick or enter a multiplier
- **Description:** Determines the size of the text displayed on the badge. This only displays when the **Beacon to Show** option is set to **Badge** or **Both**.

##### Requires Line of Sight

- **Value / Values:** **On**, Off
- **Description:** This determines whether direct line of sight is required to see the badge. This only displays when the **Beacon to Show** option is set to **Badge** or **Both**.

##### Clamp to Screen

- **Value / Values:** On, **Off**
- **Description:** When showing the HUD marker, this sets the badge to always appear on the screen. If the beacon is far away, the badge will display on the side of the HUD that matches the direction the player needs to go. This only displays when the **Beacon to Show** option is set to **Badge** or **Both**.

##### Show Offscreen Arrow

- **Value / Values:** On, **Off**
- **Description:** Sets to show an arrow pointing in the offscreen direction when the actual rendering position is offscreen and shows as a HUD element. This only displays when the **Beacon to Show** option is set to **Badge** or **Both**.

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

##### Disable When Receiving From

This function disables the device when an event occurs.

##### Add Player to Show List When Receiving From

This function adds the instigating player to the Show List when an event occurs.

##### Remove Player from Show List When Receiving From

This function removes the instigating player from the Show List when an event occurs.

##### Remove All Players from Show List When Receiving From

This function removes all players from the Show List when an event occurs.

#### Events

This device has no events.

### Gameplay Examples Using Beacons

-
[Random Sentry Fight](https://dev.epicgames.com/documentation/fortnite/random-sentry-fight-in-fortnite-creative)

-
[Search and Destroy Bomb](https://dev.epicgames.com/documentation/fortnite/search-and-destroy-bomb-in-fortnite-creative)

---

## Using Billboard Devices in Fortnite Creative

**כותרת מקורית:** Using Billboard Devices in Fortnite Creative  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/using-billboard-devices-in-fortnite-creative  
**מקור קלט:** `07E_HUD_תקשורת_שמע_וידאו_ומשוב(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `using-billboard-devices-in-fortnite-creative`

You can use **Billboard** devices to display short messages to players in your game. These are useful for things like [onboarding](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) players or providing [in-game](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) instructions.

Each message can be up to 150 characters long. You can also use multiple billboards throughout your island.

In addition to controlling the content, you can control the text size, font, justification, and text effects. You can also choose the color of the text and the background.

For help on how to find the **Billboard** device, see [Using Devices](https://dev.epicgames.com/documentation/fortnite/using-devices-in-fortnite). If you are using this in UEFN, you can find the device in the **Fortnite > Devices** folder.

If you're using multiple copies of a device on an island, it can be useful to [rename](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) them. Choosing names that relate to a device's purpose makes it easier to remember what each one does, and easier to find a specific device when using the [Event Browser](https://dev.epicgames.com/documentation/fortnite/event-browser-in-fortnite-creative).

### Device Options

This device has some basic functionality, like what text is displayed, the text size, and which font the text is using. There are also advanced options, like how far away players can read the billboard's text. In its [default](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) state, a Billboard device shows sample text, with invisible borders and a clear background.

You can configure this device with the following options.

Default values are **bold**.

 Option Value Description
**Text**

Enter text

Type the message that you want to display on the billboard. While it is possible to enter up to 512 characters, how much of the text will display is influenced by both text size and the font used.

**Show Border**

On, **Off**

Controls whether the billboard's border is visible.

If you set the **Show Border** option to **Off**, the collision properties of the device will also be turned off. That means players will be able to walk through the billboard. If you want the billboard to be solid, set the **Show Border** option to **On**.

**Display Mode**

**One Sided**, Two Sided

Controls whether the text shows on one side only or on both sides of the billboard.

**Background Color**

**Clear**, Pick a color

Sets the background color. Click to open a color picker, then scroll to select a color or use the search box to filter colors.

**Text Justification**

**Left**, Center, Right

Controls the alignment of the text.

**Text Size**

**12 (Medium)**, Pick a size

This sets the size of the text on the billboard. Use the arrows to pick a text size, or click in the field to type in a text size.

**View Distance**

Pick a distance, **Infinite**

Set how far away in-game the text will be visible. This is measured in [tiles](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary).

**Text Color**

**Alto Gray**, Pick a color

Sets the color of the text. Click to open a color picker, then scroll to select a color or use the search box to filter colors.

**Enabled During Phase**

None, **Always**, Pre-Game Only, Gameplay Only, Create Only

Controls when the billboard can be viewed. [Pre-game Only](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) can only be used with [published](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) islands.

**Text Font**

Roboto, Burbank, **Notosans**

The font used.

**Outline**

**None**, Light, Thick

Sets the thickness of a black outline around the text on the billboard.

**Shadow**

**None**, Lower Left, Lower Right, Upper Left, Upper Right

This adds a drop shadow to the text in the direction you choose.

### Direct Event Binding

Following are the [direct event binding](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) options for this device.

#### Functions

A [function](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) listens for an event on a device then performs an action.

-
For any function option, click the **option**, then **Select Device** to access and select from the **Device** dropdown menu.

-
Once you've selected a device, click **Select Event** to bind the timer to an event that will trigger the function for the device.

-
If more than one device should be affected by a function, press the **Add** button and repeat.

**אפשרויות ותיאורים:**

##### Set Text Hidden When Receiving From

Sets the text as hidden when an event occurs.

##### Set Text Visible When Receiving From

Sets the text as visible when an event occurs.

##### Update Display When Receiving Text Data When Receiving From

Sets the billboard to display text that has been updated from another source when an event occurs.

#### Events

An [event](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) tells another device when to perform a function.

No events are currently used with this device.

### Gameplay Example Using Billboards

-
[Color Switch Challenge](https://dev.epicgames.com/documentation/fortnite/color-switch-challenge-gameplay-example-in-fortnite-creative)

---

## Using HoloScreen Devices in Fortnite Creative

**כותרת מקורית:** Using HoloScreen Devices in Fortnite Creative  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/using-holoscreen-devices-in-fortnite-creative  
**מקור קלט:** `07E_HUD_תקשורת_שמע_וידאו_ומשוב(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `using-holoscreen-devices-in-fortnite-creative`

The **Holoscreen** device projects an image that you can customize with various visuals. These include:

-
A timer (standing still, or rotating)

-
Various posters and ads for Fortnite-related activities

*An example of a Holoscreen image.*

You can use multiple Holoscreens on your island.

To select the device for customization, point your phone at the device, not at the holoscreen.

For help finding the Holoscreen device, see [Using Devices](https://dev.epicgames.com/documentation/fortnite/using-devices-in-fortnite).

### Device Options

The [default](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#default) image is a clock, but other images can be selected. You can also change dimensions and appearance.

This device does not communicate with other devices.

You can configure this device with the following options.

Default values are **bold**.

**אפשרויות, ערכים ותיאורים:**

##### Bend

- **Value / Values:** **None**, Small, Medium, Large, XLarge, XXLarge
- **Description:** This determines the curve (bend) for the holoscreen.

##### Distance

- **Value / Values:** **1.0**, Select a distance
- **Description:** The distance the holoscreen is from the projector.

##### Projector Visible In Game

- **Value / Values:** **No**, Yes
- **Description:** Determines whether the projector will be visible to players during the game.

##### Holo Screen Image

- **Value / Values:** Clock, Clock Rotate, Select an option
- **Description:** Other options include advertising and signage for various [in-game](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#ingame) Fortnite businesses.

##### Width

- **Value / Values:** 1.0, Pick a width
- **Description:** The width of the holoscreen, measured in grids.

##### Height

- **Value / Values:** 1.0, Pick a height
- **Description:** The height of the holoscreen.

---

## Using HUD Controller Devices in Fortnite Creative

**כותרת מקורית:** Using HUD Controller Devices in Fortnite Creative  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/using-hud-controller-devices-in-fortnite-creative  
**מקור קלט:** `07E_HUD_תקשורת_שמע_וידאו_ומשוב(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `using-hud-controller-devices-in-fortnite-creative`

**
You can use the **HUD Controller** device to show or hide parts of the player's **[HUD](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary)**, or turn off the HUD completely. You can also use this with other devices like the HUD Message** device, the **Map Indicator** device, and the **Message Feed** device to determine exactly how much information players have during your game, as well as how and when they get that information.
**

There are several ways you can change what information shows in the HUD: change it in the User Settings,** use a **Team Settings & Inventory** device, use the **HUD Controller** device, or change it in the [Island Settings](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary). The priority order for changes to the HUD is as follows:

-
**User Settings** (press **Esc** to open the **Game Menu**, then click **Settings**) take priority over the other settings.

-
Team Settings & Inventory device takes priority over the HUD Controller and Island Settings.

-
HUD Controller takes priority over Island Settings.

-
The [Island Settings](https://dev.epicgames.com/documentation/fortnite/user-interface-settings-in-fortnite-creative) are lowest in priority. If you want to use the Island ssettings to determine what information is shown in the HUD, make sure that the HUD Controller options are set to **Do Not Override**.

There are two exceptions to the above priority hierarchy:

-
If the Island Settings or any device options are set to make parts of the HUD hidden, a player cannot turn them on in User Settings. This is so all players have access to the same HUD information in the game.

-
If the Island Settings or any device options are set to make parts of the HUD visible, a player can choose to turn them off in User Settings. This gives players the option to turn off parts of the HUD they don't need or want without affecting the experience of other players.

For help on how to find the **HUD Controller** device, see [Using Devices](https://dev.epicgames.com/documentation/fortnite/using-devices-in-fortnite).

If you're using multiple copies of a device on an island, it can be useful to [rename](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) them. Choosing names that relate to a device's purpose makes it easier to remember what each one does, and easier to find a specific device when using the [Event Browser](https://dev.epicgames.com/documentation/fortnite/event-browser-in-fortnite-creative).

### Contextual Filtering

Some devices are affected by a feature called **contextual filtering**. This feature hides or displays options depending on the values selected for certain related options. This reduces clutter in the Customize panel and makes options easier to manage and navigate. To help identify them, values that trigger contextual filtering are in *italic*.

All options are listed, including those affected by contextual filtering; if they are hidden or displayed based on a specific option's value, there will be a note about it in the Description field for that option.

### Device Options

This device has some basic functionality, like showing or hiding the [minimap](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary), and showing or hiding player resources. Additionally, there are some advanced options, like showing or hiding health, shields, or experience.

You can configure this device with the following options.
**

Default values are **bold**.

 Option Value Description
**Show HUD**

**Do Not Override**, Yes, No

Selecting **No** hides the HUD completely. If you want a HUD displayed, you can show or hide individual elements by customizing the options below.

**Show Minimap**

**Do Not Override**, Yes, No

Determines whether the minimap is displayed.

**Show HUD Info Box**

**Do Not Override**, Yes, No

Determines whether the HUD Info Box is displayed.

**Show Storm Timer**

**Do Not Override**, Yes, No

Determines whether the storm timer is displayed.

**Show Player Count**

**Do Not Override**, Yes, No

Determines whether the HUD displays the number of players currently in the game.

**Show Elimination Counter**

**Do Not Override**, Yes, No

Determines whether the HUD displays the number of players who have been eliminated.

**Show Round Timer**

**Do Not Override**, Yes, No

Determines whether to display the Round Timer.

**Show Round Details**

**Do Not Override**, Yes, No

Determines whether the Round Details are displayed.

**Show Build Menu**

**Do Not Override**, Yes, No

Determines whether the Build menu is displayed.

**Show Player Inventory**

**Do Not Override**, Yes, No

Determines whether the player's inventory is displayed.

**Show Team Info**

**Do Not Override**, Yes, No

Determines whether the Team Info HUD is displayed.

**Show Damage Numbers**

**Do Not Override**, Yes, No

Determines if Damage Numbers appear.

**Show Health**

**Do Not Override**, Yes, No

Determines whether the player's health bar is displayed.

**Show Health Numbers**

**Do Not Override**, Yes, No

Determines whether the player's health numbers are shown.

**Show Shields**

**Do Not Override**, Yes, No

Determines whether or not the player's shield bar is displayed.

**Show Shield Numbers**

**Do Not Override**, Yes, No

Determines if the player's shield numbers are visible.

**Show Battle Pass UI**

**Do Not Override**, Show All, Level Only, Experience Bar Only, Don’t Display

Determines what degree of the Battle Pass Experience UI is visible.

**Show Crafting Resources**

**Do Not Override**, Yes, No

Determines if crafting resources are visible on the HUD.

**Show Wood Resource**

**Do Not Override**, Yes, No

Determines whether or not the player's stock of wood is displayed.

**Show Stone Resource**

**Do Not Override**, Yes, No

Determines whether or not the player's stock of stone is displayed.

**Show Metal Resource**

**Do Not Override**, Yes, No

Determines whether or not the player's stock of metal is displayed.

**Show Gold Resource**

**Do Not Override**, Yes, No

Determines whether or not the player's stock of gold is displayed.

**Display Reticle**

**Do Not Override**, Always Show Reticles, Only Show Pickaxe Reticle, Only Show Weapon Reticles, Never Show Reticles

Determines what kinds of reticles, if any, are displayed.

Show Reticle Status**

Do Not Override, Yes, No

Determines if the reticle status is visible.

When the option is set to Yes, the status for the reticle, such as, No Ammo, appears.

**Show Pickup Stream**

**Do Not Override**, Yes, No

Determines whether or not the item pickup stream is displayed.

**Show Equipped Item Info**

**Do Not Override**, Yes, No

Determines whether or not information about the equipped item is displayed.

**Show Backpack Key**

**Do Not Override**, Yes, No

Determines if the backpack key is visibile.

**Show Sprint Bar**

**Do Not Override**, Yes, No

Determines if the player's sprint bar is visible.

**Show Player Action Alert**

**Do Not Override**, Yes, No

Determines whether player action alerts are displayed. This includes message for when a player is eliminated, when a player is down, and so on.

**Show Contextual Controls**

**Do Not Override**, Yes, No

Determines if a list of contextual controls are shown onscreen. This usually appears on the left side of the screen, when a particular device, vehicle, etc. has its own set of keybinds for controls.

**Show Interaction Prompts**

**Do Not Override**, Yes, No

Determines if interaction prompts are visible.

**Show Map Scoreboard Prompt**

**Do Not Override**, Yes, No

Determines if the Map/Scoreboard prompt is displayed.

**Show Storm Notifications**

**Do Not Override**, Yes, No

Determines if storm notifications are visible.

**Show Visual Sound Effect Indicators**

**Do Not Override**, *Custom*, No

If this is set to **No**, all visual-sound effects are disabled. When set to *Custom*, additional Show Indicator options become available in the options list.

**Enabled During Phase**

None, **All**, Pre-Game Only, Gameplay Only

Determines the game phases during which the device will be enabled. Pre-Game includes all phases prior to the game starting.

**Affected Team**

**Any**, Pick a team

Determines which team is affected by this device's changes to the HUD.

**Invert Affected Team**

Yes, **No**

If this is set to **Yes**, the device affects all teams except the one selected in the **Affected Team** option.

**Affected Class**

No Class, **Any**, Pick a class

Determines which class is affected by this device's changes to the HUD.

**Invert Affected Class**

Yes, **No**

If this is set to **Yes**, the device affects all classes except the one selected in the **Affected Class** option.

**Priority**

Lowest, Very Low, Low, **Normal**, High, Very High, Highest

Establishes a priority for this device. If several devices make different changes to the HUD, devices with a higher priority will override devices with a lower priority. If several devices have the same priority, only the first relevant device from a priority group will be considered.

**Modify Active Speakers Layout**

*On*, **Off**

If this is set to **On**, you can modify the location for the Active Speakers UI elements using the four additional options that display below this one.

**Modify Text Chat Layout**

*On*, **Off**

If this is set to On, you can modify the location for the Text Chat UI element using the four additional options that display below this one.

Text Chat can only be repositioned within the bounds of the screen.

**Alignment**

For Active Speakers Layout:

Middle Right, Pick a position

-
For Text Chat Layout: **Top Left**, Pick a position

This option only displays if the **Modify Active Speakers Layout** or **Modify Text Chat Layout** options are set to **On**. This determines the location on the screen for the Active Speakers UI or Text Chat UI elements. Click the arrow to open the Alignment Picker. Select a location, then click the checkmark to close the Alignment Picker.

**Anchor**

-
For Active Speakers Layout: Top Right, Pick a position

-
For Text Chat Layout: **Top Left**, Pick a position

This option only displays if the Modify Active Speakers Layout or Modify Text Chat Layout options are set to On. This option determines whether the Active Speakers UI or Text Chat UI is anchored to a position on the screen. Click the arrow to open the Anchor Picker. Select a location, then click the checkmark to close the Anchor Picker.

**X Offset**

**0.0**, Pick or enter a number

This option only displays if the **Modify Active Speakers Layout** or **Modify Text Chat Layout** options are set to **On**. Instead of using the **Alignment** or **Anchor **options, you can use this to precisely position the Active Speakers UI or Text Chat UI at a specific horizontal location.

**Y Offset**

**0.0**, Pick or enter a number

This option only displays if the

Modify Active Speakers Layout or Modify Text Chat Layout options are set to On. Instead of using the **Alignment** or **Anchor** options, you can use this to precisely position the Active Speakers UI or Text Chat UI at a specific horizontal location.

**Show HUD Messages**

Do Not Override, Yes, No

Determines whether HUD Messages display in the HUD or not.

**Show Vehicle Health**

Do Not Override, Yes, No

Determines whether vehicle health is displayed.

**Show Vehicle HUD**

Do Not Override, Yes, No

Determines whether to show the vehicle HUD when a player is driving a vehicle.

You can turn off visual sound effects in **Island Settings** by setting the **Visual Sound Effects** option to **Off**.
Additionally you can disable visual-sound efect indicators using Verse. Refer to the [Verse API](https://dev.epicgames.com/documentation/en-us/uefn/verse-api/fortnitedotcom/ui) for more information.

#### Additional UEFN Options

There are some UEFN-only settings for this device:

**אפשרויות, ערכים ותיאורים:**

##### Modify Minimap Layout

- **Value / Values:** False, *True *
- **Description:** This option only displays if you have the **Show Minima****p** option set to **Yes**. If you click the checkbox for this option, the **Alignment**, **Anchor**, **X Offse**t, and **Y Offset** options display. This gives you a way to modify the default Minimap layout.

##### Modify Player Inventory

- **Value / Values:** **False**, *True*
- **Description:** This option only displays if you have the Show Player Inventory option set to Yes. If you click the checkbox for this option, the Alignment, Anchor, X Offset, and Y Offset options display. This gives you a way to modify the layout of the player inventory.

##### Modify Health Layout

- **Value / Values:** **False**, True
- **Description:** This option only displays if you have the **Show Health** option set to **Yes**. If you click the checkbox for this option, the **Alignment**, **Anchor**, **X Offset**, and **Y Offset** options display. This gives you a way to modify the layout of the Health Widget.

##### Modify Equipped Items

- **Value / Values:** Select a widget
- **Description:** This option only displays if you have the Show Equipped Item Info option set to Yes. If you click the checkbox for this option, the **Alignment**, **Anchor**, **X Offset**, and **Y Offset** options display. This gives you a way to modify the layout of equipped item information.

##### Player Info Widget Override

- **Value / Values:** Select a widget
- **Description:** Provides a way to add a new player info widget to alter the HUD display from the default Fortnite look.

##### Equipped Item Info Widget Override

- **Value / Values:** Select a widget
- **Description:** Provides a way to add a custom widget Blueprint to alter the Fortnite HUD display for equipped item information.

##### Custom Quickbar Slot Widget Override

- **Value / Values:** Select a widget
- **Description:** Provides a way to add a custom widget for Quickbar slots.

##### Custom Quickbar Keybinding Layout

- **Value / Values:** **Bottom**, Top, Left, Right
- **Description:** Adjusts the layout of the keybindings in relation to the Quickbar slots when using a custom Quickbar widget.

##### Custom Quickbar Orientation

- **Value / Values:** **Horizontal**, Vertical
- **Description:** Decides whether to stack the Quickbar slots horizontally or vertically.

##### Modify Custom Quickbar Layout

- **Value / Values:** **False**, *True*
- **Description:** If you set this to **True**, the **Alignment**, **Anchor**, **X Offset** and **Y Offset** options display. This gives you a way to modify the layout of your custom Quickbar widget.

##### ******Custom Quickbar Paddin**g

- **Value / Values:** **0.0**, Pick an amount
- **Description:** This determines how much padding space is between the Quickbar slots on your custom Quickbar widget.

### Event Binding

Following are the [direct event binding](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) options for this device.

#### Functions

A [function](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) listens for an event on a device then performs an action.

-
For any function, click the **option**, then **Select Device** to access and select from the **Device dropdown menu**.

-
Once you've selected a device, click **Select Event** to bind the device to an event that will trigger the function.

-
If more than one device or event triggers a function, click the **Add** button to add a line and repeat these steps.

**אפשרויות ותיאורים:**

##### Enable When Receiving From

This function enables the device when an event occurs.

##### Disable When Receiving From

This function disables the device when an event occurs.

##### Update Affected Team When Receiving From

When an event occurs, this function changes the team selected in the **Affected Team** option to the instigator's team.

##### Update Affected Class When Receiving From

When an event occurs, this function changes the class selected in the **Affected Class** option to the instigator's class.

##### Reset Affected Team When Receiving From

When an event occurs, this function changes the **Affected Team** option to its original setting.

##### Reset Affected Class When Receiving From

When an event occurs, this function changes the **Affected Class** option to its original setting.

#### Events

This device has no events.

---

## Using HUD Message Devices in Fortnite Creative

**כותרת מקורית:** Using HUD Message Devices in Fortnite Creative  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/using-hud-message-devices-in-fortnite-creative  
**מקור קלט:** `07E_HUD_תקשורת_שמע_וידאו_ומשוב(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `using-hud-message-devices-in-fortnite-creative`

The **HUD Message** device displays messages to all players or specific ones, either through a trigger from another device or through a timer from the start of a [round](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary).

If you're using multiple copies of a device on an island, it can be helpful to [rename](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary) them. Choosing names that relate to a device's purpose makes it easier to remember what each one does, and easier to find a specific device when using the [Event Browser](https://dev.epicgames.com/documentation/fortnite/event-browser-in-fortnite-creative).

### Contextual Filtering

Some devices are affected by a feature called contextual filtering. This feature hides or displays options depending on the values selected for certain related options. This feature will reduce clutter in the Customize panel and make options easier to manage and navigate.

However, it may not be easy to recognize which options or values trigger contextual filtering. To help you identify them, in our device docs we use *italic* for any values that trigger contextual filtering. All options will be listed, including those affected by contextual filtering; if they are hidden or displayed based on a specific option's value, there will be a note about that in the **Description** field for that option.

### Device Options

You can configure this device with the following options.
**

Default values are **bold**. Values that trigger contextual filtering are *italic*.

**אפשרויות, ערכים ותיאורים:**

##### Message

- **Value / Values:** Enter text and format text
- **Description:** Click the **Format Styles** tab to choose a style for your text. A list of styles available is on the right. Each individual word must be clicked to select, then clicked again to de-select it. When you want to apply a style, click every word you want to have that style. If you want some words to have one style, and other words to have a different style, make sure you de-select previously selected words before selecting new words for the next style.

##### Show on Round Start

- **Value / Values:** **Off**, *On*
- **Description:** Determines if the message automatically appears at the start of a round. If you set this to **On**, another option displays below this one.

##### Time From Round Start

- **Value / Values:** Off, **10 seconds**, Pick an amount of time
- **Description:** This only displays if the **Show on Round Start** option is set to **On**. Displays the message based on the length of time after the round starts.

##### Background Opacity

- **Value / Values:** **0%**, Pick or enter a percentage
- **Description:** Determines the opacity of the message's background. By default, the background is transparent.

##### Background Color

- **Value / Values:** 2600CEFF**, Pick a color swatch
- **Description:** If you have set a background opacity in the **Background Opacity** option, this determines the color of the background. Click the color swatch to open the Color Picker. Each color swatch has its Hex Code next to the swatch. You can also type a Hex Code into the Search bar to find a specific color. Select a color, then click the checkmark.
**

##### Message Recipient**

- **Value / Values:** All, [Friendlies](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary), [Enemies](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary), Triggering Player, Pick or enter a team number
- **Description:** Determines which players receive the HUD message.

##### Show for Duration

- **Value / Values:** *Timed*, Permanent
- **Description:** Determines whether the device shows the message for a specific period of time. If you choose Timed, the Display Time option displays below this one.

##### Display Time

- **Value / Values:** 5 seconds, Permanent, Pick an amount of time
- **Description:** This option only displays if the Show for Duration option is set to Timed. Determines how long the message id displayed.

##### Play Sound

- **Value / Values:** Message - Important, Pick a sound
- **Description:** Determines which sound should accompany the message when it is displayed.

##### Placement

- **Value / Values:** Bottom Center, Top Center, Center Right, *Custom*
- **Description:** Choose where in the HUD the message displays. If you choose Custom, several additional options are displayed below this one.

##### Screen Anchor

- **Value / Values:** Top Left, Top Center, Top Right, Center Left, Center, Center Right, Bottom Left, Bottom Center, Bottom Right
- **Description:** This option is only displayed if you have the Placement option is set to Custom. Determines where on the screen the message is anchored, as well as the alignment of the message itself.

##### Placement Horizontal

- **Value / Values:** **0**, Pick a positive or negative number
- **Description:** This option is only displayed if you have the Placement option is set to Custom. Determines how far away, in pixels, the message is from the anchor point set in the Screen Anchor option. Positive numbers move it to the right, negative numbers move it to the left.

##### Placement Vertical

- **Value / Values:** **0**, Pick a positive or negative number
- **Description:** This option is only displayed if you have the Placement option is set to Custom. Determines how far away, in pixels, the message is from the anchor point set in the Screen Anchor option. Positive numbers move it upward, negative numbers move it downward.

##### HUD Widget

- **Value / Values:** Basic, Critical
- **Description:** Determines the visuals of the HUD message.

##### Layer

- **Value / Values:** **0**, Pick a layer number
- **Description:** Determines what layer the message displays on. Only one message at a time will display on a layer, and any other messages set to that layer will be queued. Setting messages to different layers causes multiple messages to be displayed simultaneously.

##### Priority

- **Value / Values:** **5**, Display Immediately, Pick or enter a priority number
- **Description:** Determines the priority for this message. Messages with a lower number (such as 1) are a higher priority, and will move any displayed message on the same layer to a queue. If you choose Display Immediately the message will display immediately and ignore any other messages.

##### Allow Multiple in Queue

- **Value / Values:** **Off**, On
- **Description:** By default, a message will only be queued if the device doesn't already have a message in the queue, or a message already displayed. If you choose On, you can have multiple messages queued on this device.

##### Show Behavior If Showing

- **Value / Values:** **Reset Display Time**, Replay, Ignore
- **Description:** Determines what happens if the device is directed to display a message when that message is already displayed.

##### Queue Timeout

- **Value / Values:** **Don't Queue**, Pick an amount of time
- **Description:** If a message is queued because a higher priority message is being displayed, this determines how long the message remains in the queue.

##### Queue Message for Join In Progress Players

- **Value / Values:** **On**, Off
- **Description:** Determines if this message is queued and then displayed to players that join the game while it is in-progress. This takes into account the value set for the Queue Timeout option.

##### Re-Evaluate Messages On Show

- **Value / Values:** **Off**, On
- **Description:** When a message is ready to be displayed, this determines if it is checked to make sure it is still relevant. This is useful if players can change class or team during the game, or otherwise become ineligible to see a message.

##### Intro Animation

- **Value / Values:** **None**, Zoom, Fade and Zoom, Fade, Reverse Zoom, Bounce, Slow Zoom, Slow Fade and Zoom, Slow Fade, Slow Reverse Zoom, Slide From Top, Slide From Bottom, Slide From Left, Slide From Right
- **Description:** Determines how the HUD Message is animated as it displays.

##### Outro Animation

- **Value / Values:** **None**, Zoom, Fade and Zoom, Fade, Reverse Zoom, Bounce, Slow Zoom, Slow Fade and Zoom, Slow Fade, Slow Reverse Zoom, Slide From Top, Slide From Bottom, Slide From Left, Slide From Right
- **Description:** Determines how the HUD Message is animated as it is removed.

##### Text Style Set

- **Value / Values:** Off, On
- **Description:** Determines the style set for the text. Select a text style from the dropdown menu.

##### Override Default Text Style

- **Value / Values:** **On**, Off
- **Description:** Provides a way to expose options to manually override the text when no styling is added. You will need to save your changes before any changes you make are applied to the preview.

##### Text Color

- **Value / Values:** **White**, Pick a color swatch
- **Description:** This option is only displayed if Override Default Text Style is set to On. Determines the color of the text in the HUD Message. Click the swatch to open the Color Picker. This is similar to the Color Picker for Background Color, but has names for colors rather than Hex Codes. Select a color, then click the checkmark to close the Color Picker.

##### Text Justification

- **Value / Values:** Left, Center, Right, Invariant Left, Invariant Right
- **Description:** Determines which side the text is aligned to. If you choose **Invariant Left** or **Invariant Righ**t, the text aligns to that side no matter what language the text is displayed in.

##### Verse Text Style

- **Value / Values:** ** Off**, On
- **Description:** Any message that originates from Verse script automatically applies the selected style to its entire message.

##### Shadow Offset

- **Value / Values:** **1**, Pick or enter a number
- **Description:** This option is only displayed if Override Default Text Style is set to On. Determines the drop-shadow offset amount.

##### Outline Strength

- **Value / Values:** 1, Pick or enter a number
- **Description:** This option is only displayed if Override Default Text Style is set to On. Determines the outline strength on the text.

##### Size

- **Value / Values:** **18**, Pick or enter a size
- **Description:** This option is only displayed if Override Default Text Style is set to On. Determines the font size of the text.

### Direct Event Binding

**Direct event binding** allows devices to communicate directly, which makes your workflow more intuitive, and gives you more freedom to focus on your design ideas.

Below are the functions and events for this device.

#### Functions

A function listens for an event on a device then performs an action.

-
For any function, click the **option**, then **Select Device** to access and select from the **Device dropdown menu**.

-
Once you've selected a device, click **Select Even**t to bind the device to an event that will trigger the function for the device.

-
If more than one device or event triggers a function, click the **Add** button to add a line and repeat these steps.

**אפשרויות ותיאורים:**

##### Show When Receiving From

This function displays the HUD message when an event occurs. If more than one device or event can display message, you can click the **Add** button for this option, which adds another line.

##### Hide When Receiving From

This function hides the message. If more than one device or event can hide the message,you can click the **Add** button for this option, which adds another line.

##### Clear Layer When Receiving From

This function clears all text layers when an event occurs. If more than one device or event can clear all layers, click the **Add** button to add another line.

#### Events

This device has no events.

---

## Using Map Indicator Devices in Fortnite Creative

**כותרת מקורית:** Using Map Indicator Devices in Fortnite Creative  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/using-map-indicator-devices-in-fortnite-creative  
**מקור קלט:** `07E_HUD_תקשורת_שמע_וידאו_ומשוב(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `using-map-indicator-devices-in-fortnite-creative`

The **Map Indicator** device lets you add points of interest to your island that can help players quickly orient to where they are in relation to where they want to go.

These markers display on both the [minimap](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#minimap) and the overview map.

To find the Map Indicator device, go to the Creative inventory and select the Devices tab. From there you can search or browse for the device. For more information on finding devices, [Using Devices](https://dev.epicgames.com/documentation/fortnite/using-devices-in-fortnite).

### Device Options

This device has some basic functionality, like determining the icon and icon color, and entering text to display at the indicator location. Additionally, there are some advanced options, like determining which team can see the indicator.

You can configure this device with the following options.

Default values are **bold**.

**אפשרויות, ערכים ותיאורים:**

##### Enabled on Game Start

- **Value / Values:** **Yes**, No
- **Description:** Determines whether the device is enabled when the game starts.

##### Icon

- **Value / Values:** **A**, Pick an icon
- **Description:** Sets the icon the map indicator displays on the map. Click the right arrow to open the **Icon Library Picker**. Choose an icon by scrolling through the Icon Library, or enter a word in the search bar to find a specific icon. Select an icon, then click the checkmark to close the Icon Picker.

##### Icon Color

- **Value / Values:** **White**, Red, Orange, Yellow, Green, Teal, Blue, Purple
- **Description:** Determines the color of the icon.

##### Show on Which Map

- **Value / Values:** **Both**, Minimap, Overview Map
- **Description:** Control which maps you want the indicator to display on.

##### Text

- **Value / Values:** Enter text
- **Description:** You can type in text you want to be displayed on the map at the indicator location. The text field has an 80 character limit.

##### Text Color

- **Value / Values:** **White**, Red, Orange, Yellow, Green, Teal, Blue, Purple
- **Description:** Determines the color of the text. Use the Color Picker to find a color.

##### Assigned Team

- **Value / Values:** **All**, Pick a team
- **Description:** Determines which team can see the map indicator.

##### Invert Team

- **Value / Values:** **No**, Yes
- **Description:** If you select **Yes**, the **Assigned Team** is the only team that cannot see the map indicator. If you leave the default **No**,the assigned team is the only team that can see it.

##### Assigned Class

- **Value / Values:** **Any**, No Class, Pick a class
- **Description:** Players with the selected class assigned can activate the device. If you choose **No Class**, only players who are not assigned a class can activate it. If you choose **Any**, all players with an assigned class can activate it.

##### Invert Class

- **Value / Values:** **No**, Yes
- **Description:** By default, only the **Assigned Class** can see the map indicator. If you set this to **Yes**, the assigned class is the only class that cannot see it.

##### Show Objective Pulse to Instigator Only

- **Value / Values:** **On**, Off
- **Description:** The Objective Pulse will only appear or disappear for the activating player.

##### Show Objective Pulse to Friendly Players

- **Value / Values:** **On**, Off
- **Description:** An Objective Pulse will appear to Friendly players, indicating the location of the device in relation to the player.

##### Icon Scale

- **Value / Values:** **1.0**, select a value
- **Description:** Select a number less than 1.0 to make it smaller, or more than 1.0 to make it larger.

### Direct Event Binding

Direct event binding allows devices to communicate directly, which makes your workflow more intuitive, and gives you more freedom to focus on your design ideas.

Below are the following direct event binding options for this device.

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

Enables this device when an event occurs.

##### Disable When Receiving From

Disable this device when an event occurs.

##### Activate Objective Pulse When Receiving From

When an event occurs that triggers this device, it activates a pulse near the [instigating](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#instigator) player that points toward the device.

##### Deactivate Objective Pulse When Receiving From

Deactivates the pulse when an event occurs.

#### Events

This device has no events.

### Gameplay Examples Using Map Indicators

-
[Search and Destroy](https://dev.epicgames.com/documentation/fortnite/search-and-destroy-bomb-in-fortnite-creative)

---

## Using Message Feed Devices in Fortnite Creative

**כותרת מקורית:** Using Message Feed Devices in Fortnite Creative  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/using-message-feed-devices-in-fortnite-creative  
**מקור קלט:** `07E_HUD_תקשורת_שמע_וידאו_ומשוב(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `using-message-feed-devices-in-fortnite-creative`

The **Message Feed** device gives you the ability to send a short message to the player's message feed. In an [elimination confirmed](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#elimination-confirmed) [game mode](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#game-mode), this could be used to broadcast when eliminations are confirmed or when points are granted. For other game modes, such as [capture the flag](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#capture-the-flag) or [domination](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#domination), the feed could include messages about flags captured or returned, areas that change teams, or other events in a game. In fast-paced game modes, this device gives you the ability to provide players with an on-screen stream of information about rapidly changing conditions.

 For help finding the Helicopter Spawner device, see [Using Devices](https://dev.epicgames.com/documentation/fortnite/using-devices-in-fortnite).

If you're using multiple copies of a device on an island, it can be helpful to [rename](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#rename-a-device) them. You can choose names that relate to each device's purpose, so it's easier to remember what each one does.

### Device Options

This device has some basic functionality, like creating a custom message, and choosing the color of the message. Additionally, there are some advanced options, like choosing which class or team generates messages in the feed.

You can configure this device with the following options.

Default values are **bold**.

**אפשרויות, ערכים ותיאורים:**

##### Enabled at Start

- **Value / Values:** On, Off
- **Description:** **Message**

##### **Default Message**, enter text

- **Value / Values:** Determines the message to display. The field is limited to 150 characters. Custom tags such as {Player Name} and {Icon} are supported.
- **Description:** **Message Color**

##### **Default**, Team Affinity, Team Color, Pick a color

- **Value / Values:** Determines what color the message text displays in. You can match this to a team color or just pick different colors.
- **Description:** **Player Highlight Color**

##### **Default**, Team Affinity, Team Color, Pick a color

- **Value / Values:** If you have used **{PlayerName}** in your message, this option determines if the message has a different color for an instigating player, compared to the other messages in the feed.
- **Description:** **Message Icon**

##### **None**, Pick an icon

- **Value / Values:** Click the arrow to open the Icon Library Picker. You can select an icon by scrolling through the library, or by typing a word into the Search bar.
- **Description:** If you use **{Icon}** in your message, the icon selected here will be displayed in the message.

##### Message Visibility

- **Value / Values:** **All**, Friendlies, Enemies, Triggering Players, Pick or enter a team
- **Description:** Determines who can see the message feed. Make visible to all players, specify a team, choose Friendlies or Enemies, or make the message only available to the Triggering Player.

##### Invert Message Visibility

- **Value / Values:** **Off**, On
- **Description:** If this is set to **On**, the value of the **Message Visibility** option determines who is **not** able to see the message feed.

##### Message Visibility by Class

- **Value / Values:** Any, Pick or enter a class
- **Description:** Determines if the message feed is only visible to players assigned a specific class.

##### Invert Message Visibility by Class

- **Value / Values:** Off, On
- **Description:** If this is set to On, the value of the Message Visibility by Class option determines who is not able to see the message feed.

##### Activating Team

- **Value / Values:** Any, Pick or enter a team
- **Description:** Instigating players must be on the selected team to generate a message in the feed.

##### Invert Team

- **Value / Values:** Off, On
- **Description:** If this is set to On, the value of the Activating Team option determines who does not generate a message in the feed.

##### Activating Class

- **Value / Values:** Any, Pick or enter a class
- **Description:** Instigating players must be assigned the selected class to generate a message in the feed.

##### Invert Class

- **Value / Values:** Off, On
- **Description:** If this is set to On, the value of the Activating Class option determines who does not generate a message in the feed.

### Direct Event Binding

Below are the [functions](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#function) and [events](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#event) for this device.

#### Functions

A [function](https://dev.epicgames.com/documentation/fortnite/function) listens for an event on a device then performs an action.

-
For any function option, click the option, then **Select Device** to access and select from the **Device** dropdown menu.

-
Once you've selected a device, click **Select Event** to bind the timer to an event that will trigger the function for the device.

-
If more than one device should be affected by a function, press the **Add **button and repeat.

**אפשרויות ותיאורים:**

##### Activate When Receiving From

This function generates a message for the message feed when an event occurs.

##### Enable When Receiving From

This function enables the device when an event occurs.

##### Disable When Receiving From

This function disables the device when an event occurs.

#### Events

This device has no events.

---

## Using Pop-up Dialog Devices in Fortnite Creative

**כותרת מקורית:** Using Pop-up Dialog Devices in Fortnite Creative  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/using-popup-dialog-devices-in-fortnite-creative  
**מקור קלט:** `07E_HUD_תקשורת_שמע_וידאו_ומשוב(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `using-popup-dialog-devices-in-fortnite-creative`

The **Pop-up Dialog** device is an interface you can use to make boxes of text appear in the [HUD](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#hud) that players can interact with. The boxes can contain multiple lines of text. They use multiple choice or Yes-No responses. You can use these boxes in many ways:

-
Create a way that players can vote on something.

-
Display messages or instructions for the player.

-
Display background information for objectives (when used with a Tracker device).

-
Connect to invisible Class Selector devices and allow players to choose their class.

-
Create dialog between the player and NPCs.

To find the Pop-up Dialog device, see [Using Devices](https://dev.epicgames.com/documentation/fortnite/using-devices-in-fortnite).

If you're using multiple copies of a device on an island, it can be helpful to [rename](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#rename-a-device) them. Choosing names that relate to a device's purpose makes it easier to remember what each one does, and easier to find a specific device when using the [Event Browser](https://dev.epicgames.com/documentation/fortnite/event-browser-in-fortnite-creative).

### Contextual Filtering

Some devices are affected by a feature called contextual filtering. This feature hides or displays options depending on the values selected for certain related options. This feature will reduce clutter in the Customize panel and make options easier to manage and navigate.

However, it may not be easy to recognize which options or values trigger contextual filtering. To help you identify them, in our device docs we use *italic* for any values that trigger contextual filtering. All options will be listed, including those affected by contextual filtering; if they are hidden or displayed based on a specific option's value, there will be a note about that in the **Description** field for that option.

### Device Options

This device has some basic functionality, like entering a title and description, and deterimning when the text will display. There are also advanced options, like how long the player has to interact with the text, the response type, and what text appears on the displayed buttons.

You can configure this device with the following options.
**

Default values are **bold**. Values that trigger contextual filtering are *italic*.

 Option Value Description
**Title**

Enter text

Type in a title for the text box. The text field is limited to 32 characters.

**Content Alignment**

**Centered**, Pick an alignment

Click to open the Alignment Picker. You can pick a position and shape for the pop-up dialog. You can choose either a box, a banner that is the width or height of your screen, or full screen. If you choose a box or banner you can choose the position of the box or banner.

**Description**

Enter and format text

Click the **Edit Text** button to open a rich text editor that allows you to format the text that displays in the pop-up dialog.

Click the **Enter Text** tab to display a text field with a 350-character limit. Click **Clear Styles** if you have applied styles and want to remove them. Click **Clear Text** if you want to erase everything and start over.

Click the **Format Styles** tab to choose a style for your text. A list of styles available is on the right. Each individual word must be clicked to select, then clicked again to de-select it. When you want to apply a style, click every word you want to have that style. If you want some words to have one style, and other words to have a different style, make sure you de-select previously selected words before selecting new words for the next style.

**Auto Display**

**Never**, Pregame Lobby, Game Start

Displays the text to all valid players that enter the selected phase. It also displays for players joining in progress during this phase.

**Use Dialog Timeout**

**Off**, *On*

Determines if the dialog automatically closes after a period of time. If this is set to **On**, two additional options display below this one.

**Timeout Duration**

**2.0**, Pick or enter a number

This option only displays if the **Use Dialog Timeout** option is set to **On**. Determines the amount of time the dialog box is displayed before automatically closing.

**Timer Options**

None, **Countdown**

This option only displays if the **Use Dialog Timeout** option is set to **On**. Determines if a countdown timer displays on the dialog box.

**Response Type**

*1 Button*, **2 Buttons**, *3 Buttons*, *4 Buttons*, *5 Buttons*, *6 Buttons, 7 Buttons, 8 buttons, 9 Buttons, 10 Buttons, 11 Buttons, 12 Buttons*

Determines how many buttons are shown at the end of your Description text. You can choose up to 6 buttons, and customize the text on these buttons. Depending on how many buttons you choose here, a number of additional button text fields will display below **Button 1 Text**, which allow you to enter text for those buttons.

**Default Back Button**

None, Last Button, Button 1, **Button 2**, Button 3, Button 4, Button 5, Button 6, Button 7, Button 8, Button 9, Button 10, Button 11, Button 12

You can set one of the buttons in the dialog to perform the "back" or "cancel" action.

**Button 1 Text**

**OK**, Enter text

Enter the text that displays on Button 1. The default text is "OK" and the text field is limited to 24 characters.

**Button 2 Text**

**Cancel**, Enter text

Enter the text that displays on Button 2. The default text is "Cancel" and the text field is limited to 24 characters.

**Button 3 Text**

Enter text

Enter the text that displays on Button 3. The text field is limited to 24 characters.

**Button 4 Text**

Enter text

Enter the text that displays on Button 4. The text field is limited to 24 characters.

**Button 5 Text**

Enter text

Enter the text that displays on Button 5. The text field is limited to 24 characters.

**Button 6 Text**

Enter text

Enter the text that displays on Button 6. The text field is limited to 24 characters.

Button 7 Text**

Enter text

Enter the text that displays on Button 7. The text field is limited to 24 characters.

**Button 8 Text**

Enter text

Enter the text that displays on Button 8. The text field is limited to 24 characters.

**Button 9 Text**

Enter text

Enter the text that displays on Button 9. The text field is limited to 24 characters.

**Button 10 Text**

Enter text

Enter the text that displays on Button 10. The text field is limited to 24 characters.

**Button 11 Text**

Enter text

Enter the text that displays on Button 11. The text field is limited to 24 characters.

**Button 12 Text**

Enter text

Enter the text that displays on Button 12. The text field is limited to 24 characters.

**Text Box Opacity**

**100 percent**, Pick a percentage

Determines if the dialog's background is semi-transparent, and how transparent it is.

**Mask Background**

**No**, Yes

Determines if the background is darkened when the dialog is displayed.

**Enabled During Phase**

None, **All**, Pregame Only, Gameplay Only

Determines in which phases the device is enabled. **Pregame Only** includes all phases that occur before the game starts.

**Activating Team**

**Any**, Pick a team

Determines which team can activate the device.

**Invert Team Selection**

**False**, True

If you choose **False**, only the team chosen in the **Activating Team** option can activate the device. If you choose **True**, all teams can activate the device except the one chosen in the **Activating Team** option.

**Allowed Class**

No Class, **Any**, Pick a class

Determines which classes can activate the device. If you choose **No Class**, only players without an assigned class can activate it. If you choose **Any**, any player with an assigned class can activate it.

**Invert Class Selection**

**False**, True

If you choose **False**, only the class chosen in the **Allowed Class** option can activate the device. If you choose **True**, all classes are affected except the one chosen in the **Allowed Class** option.

**Do Not Close on Button Press**

On, **Off**

Causes the dialog to remain open when any button is pressed except the BackActionBoundButton.

### UEFN-Only Options

There are additional options for this device that are only available in UEFN.

**אפשרויות, ערכים ותיאורים:**

##### Use Dialog Timeout

- **Value / Values:** *True*, **False**
- **Description:** Determines if the dialog stays open for a set amount of time, then closes automatically. If this is set to True, two additional options become available.

##### Timeout Duration

- **Value / Values:** **2 seconds**, enter a time
- **Description:** Determines how much time players have to interact with the dialog box before it closes.

##### Timer Options

- **Value / Values:** **Countdown**, None
- **Description:** Determines how the timeout duration is displayed. By default a countdown timer is used.

##### Template Override Class

- **Value / Values:** **None**, select a widget
- **Description:** Determines if a custom UI widget is used to determine the style of the dialog box. Select a widget from the dropdown.

### Functions and Events

For more information on using functions and events, see [Using Devices](https://dev.epicgames.com/documentation/fortnite/using-devices-in-fortnite).

#### Functions

**אפשרויות ותיאורים:**

##### Show When Receiving From

This function displays the pop-up dialog to valid players when an event occurs.

##### Hide When Receiving From

This function hides the dialog from valid players when an event occurs.

##### Enable When Receiving From

This function enables the device when an event occurs.

##### Disable When Receiving From

This function disables the device when an event occurs.

##### Show To All When Receiving From

This function displays the dialog to all players when an event occurs.

##### Hide From All When Receiving From

This function hides the dialog from all players when an event occurs.

#### Events
**

Events in UEFN are read-only. When you set a function on another device that binds to an event on this device, the events are set automatically but cannot be edited.

In Creative, you can link events to functions as well as functions to events.

**אפשרויות ותיאורים:**

##### On Dismissed Send Event To

When the dialog is dismissed, the device sends an event to the selected device, which triggers the selected function.

##### On Time Out Send Event To

When the dialog times out, the device sends an event to the selected device, which triggers the selected function.

##### On Responding Button 1 Send Event To

When a player responds using Button 1, the device sends an event to the selected device, which triggers the selected function.

##### On Responding Button 2 Send Event To

When a player responds using Button 2, the device sends an event to the selected device, which triggers the selected function.

##### On Shown Send Event To

When the dialog is shown, the device sends an event to the selected device, which triggers the selected function.

##### On Responding Button 3 Send Event To

When a player responds using Button 3, the device sends an event to the selected device, which triggers the selected function.

##### On Responding Button 4 Send Event To

When a player responds using Button 4, the device sends an event to the selected device, which triggers the selected function.

##### On Responding Button 5 Send Event To

When a player responds using Button 5, the device sends an event to the selected device, which triggers the selected function.

##### On Responding Button 6 Send Event To

When a player responds using Button 6, the device sends an event to the selected device, which triggers the selected function.

##### On Responding to Any Button Send Event To**

When a player responds to any Button, the device sends an event to the selected device, which triggers the selected function.

##### On Responding Button 7 Send Event To

When a player responds using Button 7, the device sends an event to the selected device, which triggers the selected function.

##### On Responding Button 8 Send Event To

When a player responds using Button 8, the device sends an event to the selected device, which triggers the selected function.

##### On Responding Button 9 Send Event To

When a player responds using Button 9, the device sends an event to the selected device, which triggers the selected function.

##### On Responding Button 10 Send Event To

When a player responds using Button 10, the device sends an event to the selected device, which triggers the selected function.

##### On Responding Button 11 Send Event To

When a player responds using Button 11, the device sends an event to the selected device, which triggers the selected function.

##### On Responding Button 12 Send Event To

When a player responds using Button 12, the device sends an event to the selected device, which triggers the selected function.

---

## Using Video Player Devices in Fortnite Creative

**כותרת מקורית:** Using Video Player Devices in Fortnite Creative  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/using-video-player-devices-in-fortnite-creative  
**מקור קלט:** `07E_HUD_תקשורת_שמע_וידאו_ומשוב(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `using-video-player-devices-in-fortnite-creative`

**
You can add media to your gameplay with the **Video Player** device that incorporates Fortnite-themed music videos. You can also set up these devices to be controlled by players or other devices.

Though multiple instances of the same video can be shown, only one video stream can play at a time.

You can use triggers, such as [Timers](https://dev.epicgames.com/documentation/fortnite/using-timer-devices-in-fortnite-creative), to automatically play a video through [events](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#event) like **Enable When Receiving From** and **Disable When Receiving From**.

Through settings like **Interact Time**, you can also control whether players can directly turn videos on or off.

You can customize the video presentation by changing the device's shape, and adjust the distance at which the videos can be heard.

To find the Video Player device, go to the **Creative inventory** and select the **Devices** tab. From there, you can search or browse for the device. For more information on finding devices see [Using Devices](https://dev.epicgames.com/documentation/fortnite/using-devices-in-fortnite)**.

If you're using multiple copies of a device on an island, it can be helpful to [rename](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#rename-a-device) them. You can choose names that relate to each device's purpose, so it's easier to remember what each one does.

### Contextual Filtering

Some devices are affected by a feature called **contextual filtering**. This feature hides or displays options depending on the values selected for certain related options. This reduces clutter in the Customize panel and makes options easier to manage and navigate. To help identify them, values that trigger contextual filtering are in *italic*.

All options are listed, including those affected by contextual filtering; if they are hidden or displayed based on a specific option's value, there will be a note about it in the Description field for that option.

### Device Options

This device has some basic functionality that allows you to change the device’s volume and interaction time. You can also use channel signals to alternate collision settings and playback for this device.

Default values are **bold**. Values that trigger contextual filtering are *italic*.

**אפשרויות, ערכים ותיאורים:**

##### Video to Play

- **Value / Values:** **Come On Down**, Jungle Jam, Rifting Reality, In The Clouds, Toon Takeover, Jukebox Joint, Current Default Party Royale Mix
- **Description:** The selected video will play when this device takes control. For descriptions, see [Video Choices](https://dev.epicgames.com/documentation/fortnite/using-video-player-devices-in-fortnite-creative) below.

##### Play Automatically

- **Value / Values:** **Yes**, No
- **Description:** Determines if the selected video will stream on all players.

##### Stream Priority

- **Value / Values:** Never Select, **0**, Pick a number
- **Description:** Higher priority streaming devices are chosen to stream first when the stream is not forced to a specific device.

##### Enabled During Phase

- **Value / Values:** None, **All**, Gameplay Only, Create Only
- **Description:** Determines the game phases during which the device will be enabled.

##### Screen Shape

- **Value / Values:** **Default**, Circular, Curved, Portrait, Square, Triangular, Half-Circle
- **Description:** Sets the shape for the device screen.See the [screen shape](https://dev.epicgames.com/documentation/fortnite/using-video-player-devices-in-fortnite-creative) options below.

##### Show Border

- **Value / Values:** **On**, Off
- **Description:** This determines whether a border is shown for the device if the selected shape supports borders.

##### Volume

- **Value / Values:** **1.0X**, Pick a multiplier
- **Description:** Determines the volume multiplier for the device. This is only used if this device is the controlling streaming device.

##### Attenuation Distance

- **Value / Values:** **Island**, Pick a distance
- **Description:** Determines how far the audio sound travels. This setting is only used for the controlling streaming device.

##### Restart When This Stream Is Loaded

- **Value / Values:** Yes, **No**
- **Description:** When this stream is chosen, this option will restart the video at the beginning when loading.

##### Looping

- **Value / Values:** **Yes**, No
- **Description:** This determines whether the video stops when it reaches the end, or plays again from the beginning.

##### Behavior on Other Stream Playing

- **Value / Values:** **Play Other Stream**, Stop Playing Current
- **Description:** Only one stream can be played at a time. This determines what happens when another streaming device takes control.

##### Triggered Seek Time

- **Value / Values:** **0 Seconds**, Pick an amount
- **Description:** When using the **Seek When Receiving From** function, this determines the time (in seconds) to which the video is set.

##### Can Interact

- **Value / Values:** ***Yes***, No
- **Description:** If set to **Yes**, players can turn the video on and off in-game, and the **Interaction Time** option is displayed below.

##### Interact Time

- **Value / Values:** **Instant (0.0)**, Pick a time
- **Description:** This option only displays if the **Can Interact** option is set to **Yes**. Determines how long it takes for a player to toggle the switch to turn the video player on or off.

##### Picture in Picture

- **Value / Values:** **No**, *Yes*
- **Description:** Determines if players can set Picture in Picture. If set to **Yes**, additional options related to Picture in Picture (PIP) will display below.

##### Always Allow PIP

- **Value / Values:** **No**, *Yes*
- **Description:** This option only shows if **Picture in Picture** is set to **Yes**. If **Always Allow PiP** is set to **No**, the **Picture-in-Picture Trigger Range** option displays below.

##### Picture-in-Picture Trigger Range

- **Value / Values:** **250M**, Pick a distance
- **Description:** This option only displays when the **Always Allow PIP** option is set to **No**. Use this setting to determine the distance at which PIP will be visible.

##### Set Collision

- **Value / Values:** **Enabled**, Disabled
- **Description:** Determines whether players can pass through the device.

##### Use Greenscreen

- **Value / Values:** **Disabled**, *Enabled*
- **Description:** Determines if a greenscreen is present. When you select **Enabled**, you can set a color and a transparency value for the greenscreen in the two options that display below.

##### Greenscreen Color

- **Value / Values:** **Green**, Pick a color
- **Description:** Sets the target color for greenscreening. To change from the default, click the color to open the Color Picker. Click in the search field and type to locate a specific color, or use the scroll bar to browse. Click a swatch to select a color, then click the checkmark to close the Color Picker.

##### Use Manual Color Entry

- **Value / Values:** **Disabled**, *Enabled*
- **Description:** Determines if you can enter RGB values manually to set the greenscreen color. If this is set to **Enabled**, the **Greenscreen Color** option is hidden, and three more options display below.

##### Manual Color (Red)

- **Value / Values:** **0**, Pick a value
- **Description:** This option only displays if the **Use Manual Color Entry** option is set to **Enabled**. Manually enter a color value for red.

##### Manual Color (Green)

- **Value / Values:** **0**, Pick a value
- **Description:** This option only displays if the **Use Manual Color Entry** option is set to **Enabled**. Manually enter a color value for green.

##### Manual Color (Blue)

- **Value / Values:** **0**, Pick a value
- **Description:** This option only displays if the **Use Manual Color Entry** option is set to **Enabled**. Manually enter a color value for blue.

##### Cutoff Adjustment

- **Value / Values:** **0.5**, Set a value
- **Description:** Controls the tolerance for greenscreen color detection. A lower value means less tolerance when detecting the color to mask, and a higher value gives more tolerance for variations in the color.

##### Show Color Values

- **Value / Values:** Yes, **No**
- **Description:** This shows the color values for screen locations during playback. This only functions when you are editing your island, and is a helpful tool for determining the RGB value of a video when using the Manual Color options.

##### Force Fullscreen on Activation

- **Value / Values:** On, **Off**
- **Description:** Determines whether making the video fullscreen is optional or automatic. If this is set to **On**, the player cannot exit fullscreen normally. You will have to use events to exit them from fullscreen, or fullscreen will end when the video ends.

##### Audience

- **Value / Values:** **Everyone**, Player, Party
- **Description:** Determines who will see the video.

#### UEFN-Only Device Options

**Custom Video ID**

Enter the Video ID

If you have a Custom Video ID you want to display instead of the default stream, you can enter it in this text field. The character limit on the text field is 42.

### Videos to Play

 Video Description

**Come On Down**

A country-themed video that encourages friends to visit the Butter Barn.

**Jungle Jam**

A jungle-themed video of friends on their journey to a tropical dance party.

**Rifting Reality**

An adventurous video of an expedition through various rifts.

**In The Clouds**

An upbeat video showing a hopeful journey to win back a partner.

**Toon Takeover**

A rap-themed video of Toon Meowscles and his friend’s journey to a concert performance.

**Jukebox Joint**

A randomized mix of back-to-back videos.

### Event Binding

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

##### Enable When Receiving From

Enables the device when an event occurs.

##### Disable When Receiving From

Disables the device when an event occurs.

##### Stop All Streaming When Receiving From

Turns off all video devices of this type when an event occurs.

##### Seek When Receiving From

Seek to a triggered seek time when this event occurs. While the video buffer is loading, the stream will pause.

##### Restart When Receiving From

When an event occurs, this will restart the stream on the triggered device from the beginning.

##### Enable Collision When Receiving From

Enable collision on this device when an event occurs.

##### Disable Collision When Receiving From

Disable collision on this device when an event occurs.

##### Enable Visibility When Receiving From

When an event occurs, this enables the video player visibility. This also enables collision based on the **Enable Collision** setting above.

##### Disable Visibility When Receiving From

Disables both visibility and collision when an event occurs.

##### Make PIP Full Screen When Receiving From

Set the picture-in-picture (PIP) to full screen when an event occurs.

##### Make PIP Default Size When Receiving From

Set the PIP to default size when an event occurs.

##### Hide PIP When Receiving From

Hide the PIP window when an event occurs.

##### Enter Full Screen When Receiving From

Set the device to full screen when an event occurs.

##### Exit Full Screen When Receiving From

Exit full screen when an event occurs.

##### Remote Video Start When Receiving From

Start the video remotely when an event occurs.

##### Mirror Another Screen When Receiving From

When an event occurs, this screen mirrors another screen.

#### Events

Direct event binding uses events as transmitters. An event tells another device to perform a function.

-
For any event option, click the **option**, then **Select Device** to access and select from the **Device dropdown menu**.

-
Once you've selected a device, click **Select Function** to bind the timer to a function for that device.

-
If more than one function is triggered by the event, press the **Add** button and repeat.

**אפשרויות ותיאורים:**

##### On Stream Started Send Event To

If you have multiple video players on your island, only one at a time can stream. This sends an event to linked devices when this device becomes the controlling streaming device.

##### Mirror This Screen Send Event To

This event causes the selected video player to mirror what is streaming on this screen.

##### On Stream Ended

When the stream ends, an event is sent to the selected device, which triggers the selected function.
