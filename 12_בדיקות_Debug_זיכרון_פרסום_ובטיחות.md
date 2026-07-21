# בדיקות, Debug, זיכרון, פרסום ובטיחות

> **מטרת הקובץ:** לרכז את מחזור הבדיקה והמסירה: Debug, Event Browser, Navigation Mesh, זיכרון, אופטימיזציה, Playtesting, Publishing ו־Moderation.  
> **מתי להשתמש בו:** בבדיקת מערכת, איתור תקלה, שיפור ביצועים, הכנה לפרסום או טיפול בכללי בטיחות ודיווח.  
> **לא כלול:** בניית מכניקות ותכנון חוויית המשחק עצמה.  
> **מקורות עיקריים:** `10_בדיקות_Debug_זיכרון_ואופטימיזציה(1).md`, `11_Playtesting_פרסום_Moderation_ובטיחות(1).md`

## תוכן עניינים

- [Debug Settings in Fortnite Creative](#debug-settings-in-fortnite-creative)
- [Event Browser in Fortnite Creative](#event-browser-in-fortnite-creative)
- [Navigation Mesh in Fortnite Creative](#navigation-mesh-in-fortnite-creative)
- [Using the Spatial Thermometer in Fortnite Creative](#using-the-spatial-thermometer-in-fortnite-creative)
- [Adding Playtesters in Fortnite Creative](#adding-playtesters-in-fortnite-creative)
- [Island Moderation and Guidelines in Fortnite Creative](#island-moderation-and-guidelines-in-fortnite-creative)
- [Island Moderation Tips and FAQs in Fortnite Creative](#island-moderation-tips-and-faqs-in-fortnite-creative)
- [Publishing from the Creator Portal in Fortnite Creative](#publishing-from-the-creator-portal-in-fortnite-creative)
- [Publishing Islands in Fortnite Creative](#publishing-islands-in-fortnite-creative)
- [Reporting Islands and Misconduct in Fortnite Creative](#reporting-islands-and-misconduct-in-fortnite-creative)

---
## Debug Settings in Fortnite Creative

**כותרת מקורית:** Debug Settings in Fortnite Creative  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/debug-settings-in-fortnite-creative  
**מקור קלט:** `10_בדיקות_Debug_זיכרון_ואופטימיזציה(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `debug-settings-in-fortnite-creative`

Like other Island Settings, any settings you change here apply only to your current island. To access the debug features, go to **Island Settings** and select the **Debug** category.

The debug settings can be changed at [**runtime**](https://dev.epicgames.com/documentation/en-us/uefn/unreal-editor-for-fortnite-glossary#runtime) in UEFN when you're playtesting. These settings do not affect published islands.

### Debug Options

The **Debug** category provides a way to debug the movement of [AI](https://dev.epicgames.com/documentation/en-us/fortnite/fortnite-creative-glossary#ai) entities on your island (such as guards or wildlife). While some of the options available on this tab are only useful if you're working in [Unreal Editor for Fortnite (UEFN)](https://dev.epicgames.com/documentation/en-us/fortnite/fortnite-creative-glossary#unreal-editor-for-fortnite), others — particularly the navigation option — are also useful in Fortnite Creative.

Debug settings can be managed from **Fortnite Creative** or from **UEFN**. Any toggle settings you change here are reflected in the [Island Settings](https://dev.epicgames.com/documentation/en-us/uefn/island-settings-in-unreal-editor-for-fortnite#useroptions-debug) in UEFN, and vice versa.

These options are on/off toggles, and they all default to Off.

 Option Values Description
Debug

On, Off

This setting defaults to Off. Set it to On to access the settings below it.

Navigation

On, Off

A navigation mesh, or NavMesh, is a way to provide a path for an AI to move through complicated spaces. This setting determines whether a visualization of the NavMesh will display in Creative in both [Create mode](https://dev.epicgames.com/documentation/en-us/fortnite/fortnite-creative-glossary#create-mode) and [Play mode](https://dev.epicgames.com/documentation/en-us/fortnite/fortnite-creative-glossary#play-mode).

The mesh shows up in Fortnite Creative whether you're in [Create mode](https://dev.epicgames.com/documentation/en-us/fortnite/fortnite-creative-glossary#create-mode) or [Play mode](https://dev.epicgames.com/documentation/en-us/fortnite/fortnite-creative-glossary#play-mode).

A NavMesh can only be generated if your island has at least one AI spawner device placed, such as a [Guard Spawner](https://dev.epicgames.com/documentation/assets/using-guard-spawner-devices-in-fortnite-creative), a [Wildlife Spawner](https://dev.epicgames.com/documentation/assets/using-wildlife-spawner-devices-in-fortnite-creative), or [Creature Spawner](https://dev.epicgames.com/documentation/assets/using-creature-spawner-devices-in-fortnite-creative).

For a full description of the colors used in the NavMesh and what they represent, see [Navigation Mesh](https://dev.epicgames.com/documentation/en-us/fortnite/navigation-mesh-in-fortnite-creative).

Invincibility

On, Off

Determines whether players take damage during playtesting. It does not affect standard gameplay.

Verse Debug Draw

On, Off

When you use [Verse](https://dev.epicgames.com/documentation/en-us/fortnite/fortnite-creative-glossary#verse) to tweak aspects of your island in UEFN, you can use a Verse feature called Debug Draw for debugging your code. This feature can be enabled from UEFN, as described in [Debug Your Game with Debug Draw](https://dev.epicgames.com/documentation/en-us/uefn/debug-draw-in-verse), or here in Island Settings.

This is the only debug setting that does not work in Creative directly. You can set it here, but you won't see the effects if you are in Edit/Create mode on your island — **the feature can only be used in UEFN. **

Fast Iteration Mode

On, Off

Sets whether fast iteration between Edit mode in UEFN and Creative Play mode is enabled. When set to On, your transitions from one mode to the other are faster — game countdowns are shortened, and scoreboards are skipped. This setting is intended to shorten time between edits in UEFN and playtesting, but does not affect anything in Creative if you're not using UEFN.

Test Players Added at Game Start

On, Off

Determines how many test players spawn at start of game. Test players behave as though they are idle players.

Test Players on Start

None, Fill, Custom

**None **spawns no test players.

**Fill **spawns the maximum number of players allowed per the island settings (go to **Mode > Structure > Max Players** to change this value.)

With **Custom**, you can select the number of test players up to the maximum number of players allowed.

Number of Test Players

Select a number

This option is only available if Test Players Added at Game Start is set to Custom.

Test Player Behavior

None, Random Movement, Follow Player

Determines the behavior assigned to Test Players:

**None: **Test Players have no behavior.

**Random Movement:** Test Players move within a random area.

Follow Player: Test Players start and stop following players who crouch in front of them.

Custom Test Player

Select a character

**UEFN only**. Paste a character definition, or browse.

---

## Event Browser in Fortnite Creative

**כותרת מקורית:** Event Browser in Fortnite Creative  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/event-browser-in-fortnite-creative  
**מקור קלט:** `10_בדיקות_Debug_זיכרון_ואופטימיזציה(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `event-browser-in-fortnite-creative`

The **Event Browser** is a window that shows devices you've placed on your island, and their relationships with [events](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#event) and [functions](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#function) based on [direct event binding](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary).

While the Event Browser isn't directly available from the Island Settings tab, it plays an important role in island design, allowing you to review [game mechanics](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#game-mechanics) you've already set up and improve on them.

The Event Browser can also be accessed from any Island Settings category by clicking the **Event Browser** button at the bottom of the screen.

[
](https://dev.epicgames.com/community/api/documentation/image/bbd8a76e-d0ee-4ce6-8f15-5e54129a70df?resizing_type=fit) If the buttons at the bottom don't display, click anywhere on the screen to open the button bar.

You can also access the Event Browser from any device **Customize options** window.

### Using the Event Browser

Accessing the **Event Browser** opens a window that displays a list of all devices in use on your island.

This screen lists every device on your island, along with the number of interactions (called **bindings**) for each.

Bindings between devices fall into one of two categories: **outgoing [events]** and **called [functions]**.

A [call](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#call) is an instruction that activates a specific function.

When you select a device, it shows the number of functions and events associated with the device. It also lists more information about each on the right.

To drill down into more information about a specific device's bindings, highlight it, then click the **Details** button at the bottom of the screen to see more details.

Press **Esc** to return to the previous screen.

### Teleporting to a Device

You can teleport directly to any device on your island by highlighting the device, then clicking and holding the **Hold to Teleport** button.

This can be useful if you want to change any of the bindings (or other device settings).

### Sorting and Filtering Devices

To sort or filter the results displayed, click **Sort + Filter**, select your criteria, then click **Apply**.

When you click **Sort + Filter**, this opens a panel where you can set your viewing criteria.

Sorting and filtering becomes important when you have more devices than will display at one time and want to quickly find specific information.

#### Sorting

Sorting changes the order that devices are listed based on the criteria you select. You can only select one sort method at a time:

-
**Sort alphabetically** (A–Z or Z–A).

-
**Sort by number of bindings** (events or functions) a device has, most to least or least to most.

When you've selected your sort criteria, click **Apply** to save your selection.

#### Filtering

Filtering is how you limit the device display to only those devices you're interested in seeing.

You can only select one filter at a time. **You can, however, combine sorting with filters.**

Filters include:

-
**With events or functions** only shows devices that have bindings applied.

-
**With links** only shows devices that have at least one event or function **linked** to another event or function. .

-
**With functions** shows devices with at least one bound function.

-
**With events** shows devices with at least one bound event.

-
**With functions and no events** shows devices with functions only.

-
**With events and not functions** shows devices with events only.

Any time you change the filter, click **Apply** to save your changes.

To examine the settings on a specific device in Creative, highlight the device in the list, then click and hold the **Hold to Teleport** button.

Pressing **Esc** takes you back to the **Island Settings** tab.

---

## Navigation Mesh in Fortnite Creative

**כותרת מקורית:** Navigation Mesh in Fortnite Creative  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/navigation-mesh-in-fortnite-creative  
**מקור קלט:** `10_בדיקות_Debug_זיכרון_ואופטימיזציה(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `navigation-mesh-in-fortnite-creative`

The **navigation mesh** (or NavMesh for short) is a grid that AIs use to navigate your game world. AIs don't see the game world the same way players do, and can't tell where they can and can't go just by looking. To decide where to go and how to get there, they need a grid that tells them where they can navigate to, and what kind of surface they're walking on. The way in which an AI chooses how to get to a destination is called **pathfinding**, and the navigation mesh is what AIs use to make pathfinding choices. You can use the navigation mesh to create complex AI patrol routes, pathfinding puzzles, tower defense waves, and much more.

### Enabling the Navigation Mesh

To enable the navigation mesh in Creative, navigate to **My Island**, then **Debug. **Make sure **Debug** is set to **On**, then enable **Navigation**. **NOTE**: Even if navigation is on, the NavMesh will only be generated if you've placed at least one AI spawner in your island.

Reminder: You need at least one AI spawner for a NavMesh to be generated. This can be any of Creature Spawner/Place, Wildlife Spawner, or Guard Spawner, but your island requires at least one of these for the NavMesh to generate.

#### Enabling the Navigation Mesh in UEFN

To enable the setting in UEFN, select your island settings device in the** Outliner**, and under **User Options - Debug, **enable both **Debug **and **Navigation**. The navmesh will appear in your live edit session. You will not see this in the editor viewport.

For more on the Debug tab on Island Settings, see [Debug Settings](https://dev.epicgames.com/documentation/fortnite/debug-settings-in-fortnite-creative).

### Navigation Mesh Colors

When enabled, the navigation mesh displays as a 6-tile by 6-tile grid centered on your character. The navigation mesh displays several colors based on the ability of AI to navigate to that area.

#### Navigable Areas

Navigable areas are areas where AI can navigate normally anywhere within the space. AI can path to objectives in these areas without interruption.

 Color Description Gif
Green

**Navigable **ground. AI can navigate normally anywhere within this space.

Light Blue

**Stairs**. AI can navigate normally up and down stairs in this area.

#### Obstacles

Obstacles can be props, walls, or other objects the AI attempts to navigate around. AI can either smash or mantle to navigate to or around these when possible.

 Color Description Gif
Purple

**Smashable walls**. AI will attempt to mantle these if possible, but will smash them to get through if mantling is disabled or impossible.

Gray

**Wall corners**. If AI are blocked by a wall, they will prefer to either smash or mantle the wall from the center of the wall, rather than the corners. AI can still navigate to corners normally.

Yellow

A **cheap obstacle**. Cheap obstacles are destroyed immediately when taking any damage, such as a pickaxe hit. AI will navigate around these and will prefer destroying walls over obstacles.

Brown

A **regular obstacle**. Obstacles have a set amount of HP, and may take multiple hits to destroy. AI will navigate around these, and will prefer destroying walls over obstacles.

#### Water

Water is any area that causes the AI to enter the swimming state. AI except creatures spawned from the creature spawner can navigate through these areas normally and will incorporate them into their pathing.

 Color Description Gif
Silver

**Shallow Water**, or water that does not cause the swimming state. AI can navigate normally.

Lighter Grey-Blue

**Water**. AI such as guards and wildlife can navigate water normally by swimming. Creatures spawned from the Creature Spawner are eliminated immediately upon entering the water, so they will avoid these areas.

#### Unreachable

Unreachable areas cannot be navigated to by any means. These areas occur around indestructible props or walls, and AI will either navigate around them or attempt to mantle to get over them.

 Color Description Gif
Black

**Unnavigable**. Either obstacles that cannot be destroyed or areas blocked from AI navigation, such as the AI Navigation Modification Device. Keep in mind AI can still mantle these obstacles if they are short enough.

Pink

**Indestructible walls**. AI will attempt to path around or mantle the wall but will not attempt to smash it.

Brass

**Indestructible wall corners**. AI will prefer to mantle indestructible walls from the center rather than the corners. AI can still navigate to corners normally.

### Navigation Link Arrows

Navigation Link arrows, or **navlink** arrows, are guides that help AI navigate the world vertically. Like areas in the navigation mesh, navlink arrows come in multiple colors that indicate AI interact with them. The tail of the navlink arrow is where the AI starts navigating from, and the head of the arrow is where the AI ends up.

 Color Description Gif
Green

Navigable down arrows. AI can jump down from these areas without obstruction.
*
Yellow

Jump down arrows. These function similarly to green navlink arrows, but AI will avoid using them in favor of green navlink arrows when possible. If no green arrows are generated in the area, AI will prefer to smash structures to follow purple navlink arrows.

Magenta

Navigable up arrows. AI can mantle these areas without obstruction.

Purple

Smashable down arrows. AI can smash the surface that these arrows originate from to navigate to the area below.

---

## Using the Spatial Thermometer in Fortnite Creative

**כותרת מקורית:** Using the Spatial Thermometer in Fortnite Creative  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/using-the-spatial-thermometer-in-fortnite-creative  
**מקור קלט:** `10_בדיקות_Debug_זיכרון_ואופטימיזציה(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `using-the-spatial-thermometer-in-fortnite-creative`

The Spatial Thermometer is a method for displaying and managing memory across your island. The island is divided into cells (equal to a grid tile), and a heatmap can be displayed that shows how much memory each cell is using. Instead of just having an overall memory limit, you can adjust the amount of memory used cell by cell. This gives you greater flexibility when you are building complex islands that use a lot of memory.

### Spatial Thermometer

The Spatial Thermometer memory management system measures memory cell by cell, comparing the memory use of each one to the cells next to it. Instead of loading everything in the island and storing it, the island will only use memory to store what is seen and used. It unloads unseen props and terrain from memory. As players move around the island, the system only loads things the player can see and interact with.

### Prop and Device Memory

The **Spatial Thermometer** breaks an island down into a grid of cells. Each prop you place has a memory cost that affects the area around it, within a specific radius. When you place a prop, its memory cost is added to all the cells around it from which it can be seen.

When you add a **[device](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#device)** to the island, its memory cost is added to all cells in the island. Devices always need to be loaded in memory to operate and can't be swapped in and out like props. That's because devices affect players no matter where they are on the island, and you don't want them to stop working when players get too far away from them.

When you place a prop or device, the memory usage is shown by a colored circle around the item when you are previewing it before placing it. That colored circle shows how placing that prop or device will affect the memory in that area.

The Spatial Thermometer system gives you two methods to see how much memory you have used:

-
The **Cell Memory Used** bar

-
The **Heatmap**

#### Cell Memory Used Bar

When you place a prop, the **Cell Memory Used** bar displays memory usage for the cell with the highest memory use within range of the spot where you place the prop. This shows the highest effect that placing the prop has on the memory use of nearby cells. If you don’t have a prop in hand, the Cell Memory Used Bar will show values for the cell with the highest memory cost on your island.

[
](https://dev.epicgames.com/community/api/documentation/image/5a7d759b-927d-48ec-829e-de4c217b27b7?resizing_type=fit) The Cell Memory Used bar

*Click image for full size.*

#### Heatmap

The **Heatmap** shows you a color-coded representation of the cells on your island. On PC, open the Map screen by pressing M. The heatmap is displayed on the Map screen by default. While in the Map Screen, you can press T to toggle between three different modes:

-
No Heatmap displayed

-
Heatmap only

-
Heatmap with cell memory amount displayed

[
*](https://dev.epicgames.com/community/api/documentation/image/42837f8c-c447-420b-a2b6-d33427cfc9b6?resizing_type=fit) Map Screen with Heatmap

[
](https://dev.epicgames.com/community/api/documentation/image/21464725-47c5-4a4b-8cde-af919ad0364d?resizing_type=fit) Map Screen Heatmap with Cell Memory

Map Screen with Heatmap

Map Screen Heatmap with Cell Memory

*Click image for full size.*

*Click image for full size.*

If you have the heatmap displayed on the Map screen, it will also display on the minimap when you close the Map screen.

[
](https://dev.epicgames.com/community/api/documentation/image/274b1dcf-65e9-42aa-b1df-fdbece746c58?resizing_type=fit) Minimap with no heatmap

[
](https://dev.epicgames.com/community/api/documentation/image/d98c7159-5112-4da6-b142-5b8e183d0496?resizing_type=fit) Minimap with Heatmap Only

[
](https://dev.epicgames.com/community/api/documentation/image/184278a9-7b17-4f73-8b0a-aca9ca713d03?resizing_type=fit) Minimap Heatmap with Cell Memory Used

Minimap with No Heatmap

Minimap with Heatmap Only

Minimap Heatmap with Cell Memory Used

*Click image for full size.*

*Click image for full size.*

*Click image for full size.*

You must be in Fly mode to toggle between the heatmap modes. This may change in future releases.

The colors on the heatmap give you an idea of the amount of memory that each cell is currently using.

-
**Dark Blue**: 0% memory used

-
**Light Blue**: 50% memory used

-
**Yellow**: 75% memory used

-
**Red**: 99% - 100% memory used. The cell is close to being over budget.

Tips for reducing memory in cells:

-
**Remove props from the cell** itself to reduce its memory use.

-
**Delete props from densely-packed cells nearby** to reduce the memory cost of the over-budget cell.

-
**Delete some devices**, since those contribute memory use to every cell on the island.

---

## Adding Playtesters in Fortnite Creative

**כותרת מקורית:** Adding Playtesters in Fortnite Creative  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/adding-playtesters-in-fortnite-creative  
**מקור קלט:** `11_Playtesting_פרסום_Moderation_ובטיחות(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `adding-playtesters-in-fortnite-creative`

Playtesters help to ensure island quality before publishing by working out the bugs and issues on your project through playtesting. This kind of quality control is part of a project release schedule and good practice for serious island developers.

Playtesters are people you invite to playtest your islands. They should be people you trust, and who will provide feedback on the quality of the experience and log any issues they encounter during gameplay.

Ideally, a playtester would look for possible issues with game mechanics, art, messaging, and clarity of goals in the game.

Playtesters do not have a hand in creating the island.

### Create a Playtest

To turn the **Private Version** of your island into a playtestable project, follow the steps below.

-
Open the **Projects** page and select **Playtests** from the tab menu.

-
Click **Create Playtest** and a Private Version panel opens.
**

-
Select the **Private Version** from the panel and click **Create Playtest**.

This creates a special code playtesters can use to access the island. The Private Version code is also visible from the private code message. Click Manage Playtest Group** to add playtesters to the project.

Clicking the **Manage Team** button on the playtest island code takes you to the **Manage Teams** page where you can add playtesters to your project.

### Adding Playtesters to a Project

Add playtesters to work in tandem with the project team. Follow the instructions below to invite playtesters to your team:

-
Click **Manage Team** from the main menu.

-
Click **Playtest Group** tab

-
Click **Add New Playtesters** from the tabbed options.

-
Click **Copy URL to Clipboard** to copy the invite URL.

-
Paste the URL into an email.

-
Send the email to invite to people you trust to playtest your project.

The number of playtesters you can have is limited to 50. You’ll need to remove previous playtesters from the team if you want to add new playtesters.

When invitees accept the invitation, they are listed under the **Playtest Group** tab. Go into the Playtest Group tab to add playtesters to specific projects.

### Accepting a Playtest Invitation

All playtesters receive an email invitation to join a team.

As a playtester, when you receive an invitation, click the link in the email to open the **Epic Games Sign In** page. If you don’t have an Epic Games account, you’ll be prompted to create one.

-
Sign in to your Epic Games account.

-
Click the **Join Playtest group** button. You’ll see a **Joined Successfully** message when you’ve joined the team.

-
You must be an adult to accept a Playtest Invitation. If you haven’t done so already, you will need to complete the age verification process. Epic Games has partnered with SuperAwesome to confirm that you are an adult. The verification methods available to you will vary depending on where you live. See [Parent Verifications FAQs](https://parents.superawesome.com/parent-verification-faqs/) from SuperAwesome for more information.

-
Click **Home** to go to the Creator Portal home page.

If the team you’ve been invited to join is at capacity for playtesters, you’ll receive a message:

Contact the person who invited you to join the team.

### Removing Playtesters

You can remove playtesters from a project once their testing is complete, or if you no longer need the person to playtest.

Go to the **Playtesters** tab under **Manage Team** to remove playtesters.

-
Click the **ellipsis menu** next to the playtester’s name. The option to remove the playtester opens in a popup.

-
Click **Remove Playtester **> **Confirm**. The person is removed from the Playtesters page.

You can add a new person after removing a playtester by clicking the **Add New Playtester** button.

### Switch Playtest Version

To playtest an iterated version of your island, update the playtest version and create a new playtest code.

-
Open the project from the **Playtest** tab.

-
Click **Update Playtest**.

[
*](https://dev.epicgames.com/community/api/documentation/image/bf0c3990-fa14-4815-9f4a-f30cf3701cd8?resizing_type=fit)

-
Select the project version from the slideout panel and click **Create Playtest**.

The island’s playtest code updates to a new code and shows the Private Version code for the newly selected version.

---

## Island Moderation and Guidelines in Fortnite Creative

**כותרת מקורית:** Island Moderation and Guidelines in Fortnite Creative  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/island-moderation-and-guidelines-in-fortnite-creative  
**מקור קלט:** `11_Playtesting_פרסום_Moderation_ובטיחות(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `island-moderation-and-guidelines-in-fortnite-creative`

*

Preparing your island for publication? Be sure to read through these guidelines and policies before you upload your island. Knowing how your island will be moderated ahead of time will help your island approval go more smoothly.

- [

IARC Overview and FAQs

Learn about IARC and how to apply age ratings to your island.

](https://dev.epicgames.com/documentation/fortnite/iarc-overview-and-faqs-in-fortnite-creative)
- [

Island Moderation Tips and FAQs

If your island fails moderation, use this page to get your submission back on track.

](https://dev.epicgames.com/documentation/fortnite/island-moderation-tips-and-faqs-in-fortnite-creative)
- [

Lobby Background Image Guidelines

Get the best practices for creating images for your islands!

](https://dev.epicgames.com/documentation/fortnite/lobby-background-image-guidelines-in-fortnite-creative)
- [

Reporting Islands and Misconduct

Learn how to report misconduct and illegal content on projects and islands from Fortnite Creative, UEFN, and Creator Portal.

](https://dev.epicgames.com/documentation/fortnite/reporting-islands-and-misconduct-in-fortnite-creative)
- [

Thumbnail Image Policies

Understand the policies for creating thumbnails for your islands!

](https://dev.epicgames.com/documentation/fortnite/thumbnail-image-policies)
- [

Reporting Unoriginal Promotional Assets

Report island promotional assets that imitate your original island media ideas.

](https://dev.epicgames.com/documentation/fortnite/reporting-unoriginal-promotional-assets-in-fortnite-creative)

---

## Island Moderation Tips and FAQs in Fortnite Creative

**כותרת מקורית:** Island Moderation Tips and FAQs in Fortnite Creative  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/island-moderation-tips-and-faqs-in-fortnite-creative  
**מקור קלט:** `11_Playtesting_פרסום_Moderation_ובטיחות(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `island-moderation-tips-and-faqs-in-fortnite-creative`

When you submit your island for publishing from the Creator Portal, your island goes through a two step review process to determine whether your island complies with the [Fortnite Developer Rules](https://www.fortnite.com/news/fortnite-island-creator-rules) and the [Epic Games Content Guidelines](https://www.epicgames.com/site/en-US/content-guidelines) and either gets approved and published or rejected. This process is called **moderation**.

Having your island rejected can be disappointing, but there are some simple steps you can take to make it more likely that your island will pass moderation the next time around.

If your island fails, you’ll receive an email with a link that opens the Creator Portal. You'll find your rejected island on the **Public Release** tab in the Creator Portal, along with the reason(s) the island failed review.

Click the information icon to open a moderation report that provides details. A failed release does not affect a currently live island, and so your last approved release remains as the current version.

Address the detailed issues, then generate a new private version before submitting the new iteration for review by creating a new public release.

#### What are the two stages of publishing moderation?

Moderation is conducted in two distinct stages. The first is a review of an island’s metadata and assets. The second stage is an in-island review.

During the first stage, moderators review the information and assets submitted with your island, including:

-
Island Title/Name

-
Description

-
Loading Screen Text

-
Thumbnails

-
Lobby Background

-
Promotional Screenshots

-
Trailers

-
Assets

If no violations are found, your submission will move to in-island moderation review.

#### Why was my island rejected before an in-island review?

Before moderators review your island’s gameplay, they first review the metadata and assets submitted with your island. This is the first stage of publishing moderation.

This first stage includes your island name, description, thumbnail, loading screen text, lobby background, promotional screenshots, trailers and assets. If a violation is identified in this stage, your island will be rejected before an in-island review takes place and you’ll receive feedback explaining the violation and associated rules so you can update your content and resubmit your island.

### Most Common Submission Errors

When an island is disabled, it loses analytical statistics and monetization.

-
Disabled islands are islands that cannot be played, opened, or playtested.

-
Deleted islands are islands that are deleted from Epic’s content service.

To learn more about submission errors, see this [Fortnite blog](https://create.fortnite.com/news/common-mistakes-to-avoid-when-submitting-your-fortnite-island-for-featuring) post, and Epic Games’ [IP and DMCA guidelines](https://create.fortnite.com/news/intellectual-property-ip-and-dmca-guidelines-for-fortnite-island-creators).

The following is a list of the most common errors that cause an island to fail moderation.

-
**Misleading Content:** This usually refers to the thumbnail you created for your island. Thumbnails must contain visual content that is true to your island experience. If your thumbnail doesn’t show real gameplay from your island, it will not pass moderation.

-
**Promoting SAC:** Advertising your SAC code inside your game is strictly prohibited and will immediately cause a fail. **Do not** advertise your SAC code. Your island is not the appropriate place for self promotion. Instead, use your social media accounts to promote your islands and your SAC code.

-
**Realistic Photos:** Using real images of yourself or others is not allowed in your island or for your island thumbnail. All island thumbnails in Discover **must** depict the gameplay experience of your island.

-
**Profanity:** The use of offensive language in your island name, description, or media used to advertise your island is strictly prohibited and results in failed moderation. Profanity used on your island will also be flagged during moderation.

If you are uncertain how to create appropriate media to accompany your island and how to advertise your island, check out the following documentation to learn about creating promotional material:

-
[Making Thumbnails and Videos](https://dev.epicgames.com/documentation/en-us/fortnite-creative/making-thumbnails-and-videos-in-fortnite-creative)

-
[How to Use the Replays Feature](https://dev.epicgames.com/documentation/en-us/fortnite-creative/replays-in-fortnite-creative)

-
[Marketing Your Fortnite Island](https://dev.epicgames.com/documentation/en-us/fortnite-creative/fortnite-creative-marketing-guide)

### Moderation FAQs

Below is a curated list of the most frequently asked questions when an island fails moderation.

#### Why is my Fortnite Creative or UEFN project disabled?

Epic’s moderation team reviews Fortnite Creative islands at the time of submission. Epic’s moderation team may also review your island or project because it was reported by a player. If your project is disabled, it’s because content within your project violates the [Fortnite Developer Rules](https://www.fortnite.com/news/fortnite-island-creator-rules) or the [Epic Games Content Guidelines](https://www.epicgames.com/site/en-US/content-guidelines).

When you receive notification that your island failed moderation, it’s your responsibility to address any reasons your island failed moderation before resubmitting for publishing.

#### Is the project locked for all members of my team?

Yes, if your project is locked, it will be inaccessible to all members of your team.

You will need to address the reasons your island failed moderation (create new promotional material, delete self-promoting material inside your island, and so on). After you've done this, you will need to generate a new link code in order to resubmit your project.

#### Can I recover my project?

If you believe moderation has not been applied correctly, you have the right to appeal. Submitting an appeal is the only way to recover a project. To submit an appeal, log into the [Player Support](https://www.epicgames.com/help/en-US/) website and use the **Contact Us** form to appeal the decision.

---

## Publishing from the Creator Portal in Fortnite Creative

**כותרת מקורית:** Publishing from the Creator Portal in Fortnite Creative  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/publishing-from-the-creator-portal-in-fortnite-creative  
**מקור קלט:** `11_Playtesting_פרסום_Moderation_ובטיחות(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `publishing-from-the-creator-portal-in-fortnite-creative`

You’ve tinkered with the tools, devices, and assets to build the game of your dreams. You’ve created at least one island and Fortnite Developer & Engagement Program.

Now you’re ready to take that next step and publish your island.

Keep in mind that your island must comply with the [Fortnite Developer Rules](https://www.fortnite.com/news/fortnite-creative-creator-content-rules-and-guidelines) before it can be considered for publishing.

After your island is out there, you can (and should!) continue to iterate and manage your island’s Discover thumbnail and trailer video from the Creator Portal.

### The Publishing Workflow

When you're ready to reveal your island to the world, start the publishing process from Fortnite Creative or UEFN.

#### Initiate the Publishing Process

From **Fortnite Creative**, go to **Creative Island Settings** > **Overview**, and click **Publish Island**.

From **UEFN**, click the **Project** dropdown in the toolbar, then select **Publish Project**. This creates a new private version code.

#### Publish in Creator Portal

Once you’re in the [****](https://create.fortnite.com/)**[Creator Portal](https://dev.epicgames.com/documentation/fortnite/fortnite-glossary#creator-portal)**, you’re ready to create a new release and submit it for moderation. To create a new release from your private version, follow these steps.

-
In the left navigation panel, click **Projects** to open the **Projects page**.
**

-
Click on a project tile to open the island's Publishing** page.
**

-
Click the Private Versions** screen. Select a private version from the list and click **Create release**. A pop-up will open as your selected version is validated for publishing eligibility.
**

-
Fix any errors that arise, then click Continue. The Publishing flow will open on the Game Details screen.

If your private version contains experimental features, you will not be able to create a release from a private version. If you try to initiate the Create Release workflow, a warning will display during validation to remind you that islands with experimental features cannot be published.

-
Fill out the island’s public metadata under Game Details** and click **Next** to move to the **Rating** screen.
**

Island titles and thumbnails go through a series of content pre-checks before approval and advancing the publishing flow. For information on Discover filtering and how it affects islands in Discover, see [How Discover Works](https://dev.epicgames.com/documentation/fortnite/how-discover-works-in-fortnite).

-
Provide the requested email addresses for ratings-related communications, then click Begin Questionnaire**.
**

You will not be able to progress beyond this step in the publishing process without completing the IARC questionnaire. To learn more about IARC, see the [IARC Overview and FAQ](https://dev.epicgames.com/documentation/fortnite/iarc-overview-and-faqs-in-fortnite-creative)**s.

-
You receive a message that you are leaving the Creator Portal, and being redirected to the IARC questionnaire. Click Continue to IARC to proceed filling out the questionnaire.
**

-
Once the questionnaire is filled out, click the check box** to agree to the IARC ratings.

-
Click **Finished** to return to the Creator Portal.
**

You will not be able to progress beyond this step in the publishing process without completing the IARC questionnaire. To learn more about IARC, see the [IARC Overview and FAQs](https://dev.epicgames.com/documentation/fortnite/iarc-overview-and-faqs-in-fortnite-creative).

-
From the Creator Portal, click Next** to continue to the **In-Island Transactions screen**, where you can review any entitlements for purchase you have on this island.
**

-
From the In-Island Transactions screen, click Next to continue on to the Promotional Media screen.

-
On the [Promotional Media](https://dev.epicgames.com/documentation/fortnite/promotional-media-screen-in-fortnite)** screen, upload your [thumbnails](https://dev.epicgames.com/documentation/fortnite/thumbnail-image-policies), [trailers](https://dev.epicgames.com/documentation/fortnite/making-thumbnails-and-videos-in-fortnite-creative), and [lobby backgrounds](https://dev.epicgames.com/documentation/fortnite/creating-custom-lobby-backgrounds-in-fortnite-creative). Then click **Next** to continue to the **[Attribution](https://dev.epicgames.com/documentation/fortnite/attribution-screen-in-fortnite-creative)** screen.
**

To add a second thumbnail to your promotional media, select Create A/B Test. To opt out of A/B testing, see [A/B Thumbnail Testing.](https://dev.epicgames.com/documentation/fortnite/ab-thumbnail-testing-in-fortnite-creative)

-
To ensure you receive credit for your promotional assets, submit a release with those assets for content review and wait for approval before sharing them externally. This is best practice whenever assets are updated.

-
On the Attributions** screen, click **Add New Attribution** to acknowledge any third-party assets used in your island. After entering all the necessary attributions, click **Next** to move to the **Visibility** screen.
**

Under the **[Visibility screen](https://dev.epicgames.com/documentation/fortnite/visibility-screen-in-fortnite), choose the **Project Visibility Status** for your island, and add any additional publishing information.

Click Submit for review to send your release to moderation.
**

Upon submitting for review, islands now go through a metadata and asset review before in-island gameplay review.

Moderation is conducted in two distinct stages. The first is a review of an island’s metadata and assets. The second stage is an in-island review.

If a violation is identified in your metadata or assets, you’ll receive feedback in the creator portal and by email explaining the violation and associated rules so you can update your content and resubmit your island. Only when no violations are found in metadata or assets, will an island continue to in-island review. For more information, see the [Island Moderation Tips and FAQs](https://dev.epicgames.com/documentation/fortnite/island-moderation-tips-and-faqs-in-fortnite-creative) page.

The release you submitted is now listed on the Releases** screen of the island's ****[Publishing page](https://dev.epicgames.com/documentation/fortnite/publishing-page-features-in-fortnite-creative).

If one of the publishing screens is missing information, a red exclamation mark appears next to the screen.

For more detailed information on any of the publishing workflow screens, see the linked pages below.

### Publishing Overview

- [
*

Game Details Screen

Learn everything you need to know to fill out the Game Details tab in Creator Portal.

](https://dev.epicgames.com/documentation/fortnite/game-details-screen-in-fortnite)

- [

Rating Screen

Learn more about filling out the IARC questionnaire and how age ratings are assigned to islands.

](https://dev.epicgames.com/documentation/fortnite/rating-screen-in-fortnite)

- [

Promotional Media Screen

Learn more about how you can use promotional media to support your island.

](https://dev.epicgames.com/documentation/fortnite/promotional-media-screen-in-fortnite)

- [

Attribution Screen

Give another developer their due! Let the world know whose assets you used on your island.

](https://dev.epicgames.com/documentation/fortnite/attribution-screen-in-fortnite-creative)

- [

Visibility Screen

Learn about the different publishing states to choose the right one for your island.

](https://dev.epicgames.com/documentation/fortnite/visibility-screen-in-fortnite)

- [

Project Publishing Page

Learn about the different publishing page features available in the Creator Portal.

](https://dev.epicgames.com/documentation/fortnite/publishing-page-features-in-fortnite-creative)

---

## Publishing Islands in Fortnite Creative

**כותרת מקורית:** Publishing Islands in Fortnite Creative  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/publishing-islands-in-fortnite-creative  
**מקור קלט:** `11_Playtesting_פרסום_Moderation_ובטיחות(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `publishing-islands-in-fortnite-creative`

Whether you’re publishing from Fortnite Creative or from Unreal Editor for Fortnite (UEFN), the Creative Portal is where you go to publish your islands. The portal provides everything you’ll need to prepare and submit your island.

### The Publishing Workflow

When you're ready to reveal your island to the world, start the publishing process from Fortnite Creative or UEFN.

#### Initiating the Publishing Process

From **Fortnite Creative** begin by:

-
Clicking **Publish Island** in the Overview category of the Fortnite Creative **Island Settings**.

From **UEFN** begin by:

-
Clicking the **Project** dropdown in the toolbar, then select **Publish Project**. This creates a new private version code.

#### Publishing in Creator Portal

Once you’re in the [Creator Portal](https://create.fortnite.com/), you’re ready to create a new release and submit it for moderation. To create a new release from your private version, follow the instructions below:

-
In the left navigation panel, click **Projects** to open the **Projects page**.
**

-
Click on a project tile to open the island's Publishing** page.
**

-
Click the Private Versions** tab. Select a private version in the list, and click **Create release**. A validity popup opens.
**

A validity popup opens, dismiss the window by clicking Continue**. The publishing tabs open on **Game Details**.
**

-
Fill out the island’s public metadata under Game Details** and click **Next** to move to the **Rating** tab.
**
[
](https://dev.epicgames.com/community/api/documentation/image/c1fc943a-64b5-4860-adea-105f80bf1790?resizing_type=fit) Click to enlarge image.

Island titles and thumbnails go through the Discover Filter before approval and advancing the publishing flow. For information on Discover Filtering and how it affects islands in Discover, see How Discover Works.

-
Provide an email address where you can receive ratings related communications from IARC, then click Begin Questionnaire** at the bottom of the page. You receive a message that you are leaving the Creator Portal, and being redirected to the IARC questionnaire.
**
[
](https://dev.epicgames.com/community/api/documentation/image/f0474d2d-365e-4e5b-bb20-4cbda767cd9f?resizing_type=fit) Click to enlarge image.

Click Continue to IARC** to proceed filling out the questionnaire.

-
Once the questionnaire is filled out, click the **check box** to agree to the IARC ratings.

-
Click **Finished** to return to the Creator Portal.

-
From the Creator Portal, click **Next** to continue on to the **Promotional Media** tab.

**

-
To add a second thumbnail to your promotional media, select Create A/B Test**. To opt out of A/B testing, see [A/B Thumbnail Testing.](https://dev.epicgames.com/documentation/fortnite/ab-thumbnail-testing-in-fortnite-creative)

-
To ensure you receive credit for your promotional assets, submit a release with those assets for content review and wait for approval before sharing them externally. This is best practice whenever assets are updated.

-
From the **Promotional Media** tab, upload your thumbnails, trailers, and lobby backgrounds. Then click **Next** to continue to the **Attribution** tab.
**
[
](https://dev.epicgames.com/community/api/documentation/image/71e11aa3-7a75-4294-b47a-c70fd835c9b7?resizing_type=fit) Click to enlarge image.

All islands are automatically entered into A/B thumbnail testing. To opt out of A/B testing, see the [A/B Thumbnail Testing document](https://dev.epicgames.com/documentation/fortnite/ab-thumbnail-testing-in-fortnite-creative).

-
On the Attributions** tab, select **Add New Attribution** to acknowledge any third-party assets used in your island. After entering all the necessary attributions, click **Next** to move to the **Visibility** tab.
**
[
](https://dev.epicgames.com/community/api/documentation/image/49432e65-53a2-45eb-a379-9e903b41bef0?resizing_type=fit) Click to enlarge image.

-
Under the Visibility** tab, choose the **Project Visibility Status **for your island, and any additional publishing information.
**
[
](https://dev.epicgames.com/community/api/documentation/image/ce8e5031-c55b-4f63-bac6-f62a7f21be32?resizing_type=fit) Click to enlarge image.

-
Click Submit for review** to send your release to moderation.

Your release enters a review process to ensure that the island adheres to Fortnite standards. The release you submitted is now listed on the **Releases** tab of the island's **Publishing** page.

If one of the publishing tabs is missing information, a red exclamation mark appears next to the tab.

### Publishing Overview

- [
*

Publishing from the Creator Portal

Learn how to create a release for your projects and submit it for publishing.

](https://dev.epicgames.com/documentation/fortnite/publishing-from-the-creator-portal-in-fortnite-creative)
- [

Schedule Publishing

Publish your islands strategically by scheduling the publish date to create marketing and media buzz for your next big release!

](https://dev.epicgames.com/documentation/fortnite/schedule-publishing-in-fortnite)
- [

Unpublishing Islands

Unpublish an island to work on an older island that needs a refresh.

](https://dev.epicgames.com/documentation/fortnite/unpublishing-islands-in-fortnite-creative)

---

## Reporting Islands and Misconduct in Fortnite Creative

**כותרת מקורית:** Reporting Islands and Misconduct in Fortnite Creative  
**כתובת מקור:** https://dev.epicgames.com/documentation/fortnite/reporting-islands-and-misconduct-in-fortnite-creative  
**מקור קלט:** `11_Playtesting_פרסום_Moderation_ובטיחות(1).md`  
**היקף:** Creative / Shared בהתאם לעמוד המקור  
**מזהה עמוד:** `reporting-islands-and-misconduct-in-fortnite-creative`

While creating or playing other islands, you may come across content that you believe is illegal. Illegal content includes any content or behavior that breaks the law in any country. There are several places where you can report developers and islands for illegal content or misconduct.

This does not include improper use of IP (intellectual property) assets. To report IP violations, see the [Reporting Intellectual Property Infringement](https://www.epicgames.com/site/infringement).

For more information on what assets are considered illegal and in violation of Epic's policies, see the [Epic Games Content Guidelines](https://www.epicgames.com/site/en-US/content-guidelines).

### Reporting from Creator Portal

To report illegal content from Creator Portal:

-
Go to the Project Overview page.

-
Select the menu ellipses **...** and choose **Report Project**.

-
Click the link for illegal content reporting at the bottom of the popup. Select the link to go to the [**Reporting Misconduct Form**](https://epic.gm/submit-report).

### Reporting from UEFN

To report illegal content from UEFN:

-
Go to **Project** in the top main menu.

-
Select **Report Project** from the drop down.

This will take you to the Terms and Service form for [**Reporting Misconduct**](https://epic.gm/submit-report).

### Reporting from Fortnite.com

To report an island or developer, you need to go to their island or developer page on Fortnite.com. Scroll down to the bottom of the page and select **Report Island** or **Report Developer**.

The link for Illegal Content Reporting is at the bottom of each popup. You must select the link to go to the [**Reporting Misconduct Form**](https://epic.gm/submit-report).

[
*](https://dev.epicgames.com/community/api/documentation/image/b142cae9-4845-44bc-8a16-972315bff974?resizing_type=fit)
