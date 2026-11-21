# Advanced settings

115 settings across nine categories: 57 sliders, 55 booleans, and 3 enums.

Source: **all advanced settings.mp4**, Standard Rules tab, build **3.1-643074**.

Supporting images: [browse all 553 extracted video frames](../../assets/advanced-settings/README.md).

Ranges below are the demonstrated slider endpoints, inclusive. Decimal sliders display two decimal places; the clip does not establish their exact step size or internal precision. Timestamps are approximate. Current values are not treated as defaults.

**Unresolved range:** Enemy Portal Wall Spawn Sort Weight shows 5.00, but its slider limits are not demonstrated.

**UI discrepancy:** Both in-progress respawn modifiers have descriptions saying they can be negative, but the demonstrated sliders stop at 0.00.

| Category | Settings |
|---|---:|
| Base | 6 |
| Mode | 28 |
| Map | 11 |
| Teams | 6 |
| Players | 18 |
| Loadouts | 1 |
| Abilities | 16 |
| Bots | 4 |
| Spawning | 25 |

## Base

| Name | Type | Description | Allowed values | Video |
|---|---|---|---|---|
| Round Length | Slider (integer) | Number of seconds that a round should last. Set to -1 for infinite duration. | -1 to 999 | 00:02.0–00:04.5 |
| Overtime Length | Slider (integer) | Number of seconds that overtime should last. Set to -1 to disable overtime. | -1 to 999 | 00:05.0–00:08.5 |
| Sudden Death Length | Slider (integer) | The amount of time added to the timer for sudden death. A time of 0 or less will instantly end sudden death once no objectives are being interacted with. | 0 to 999 | 00:09.5–00:13.0 |
| Allow Normal Sudden Death | Boolean | If true, sudden death can be triggered when the normal timer ends before going to overtime. | Off / On | 00:13.5–00:15.0 |
| Allow Overtime Sudden Death | Boolean | If true, sudden death can be triggered when the overtime timer ends. | Off / On | 00:15.5–00:16.5 |
| Score Mode | Enum | No description displayed. | HIGHEST SCORE WINS; LOWEST SCORE WINS | 00:17.0–00:18.0 |

## Mode

| Name | Type | Description | Allowed values | Video |
|---|---|---|---|---|
| Spectate Closest Player on Start Spectating | Boolean | If we want to automatically spectate the nearest player upon starting spectating. If false we just freecam at our death's camera location. | Off / On | 00:22.0–00:22.5 |
| Spectate Player Who Killed Us when on Start Spectating as Participant | Boolean | If we want to try spectating the player that killed us when we start spectating. Only applies to situations that allow viewing enemies | Off / On | 00:23.0–00:23.5 |
| Can Spectate Enemies | Boolean | If spectators can ALWAYS spectate enemies, injunction or not. | Off / On | 00:24.5–00:25.0 |
| Can Spectate Enemies with Injunction Active | Boolean | Allows spectating enemies if you have injunctions blocking your respawn, even if bCanSpectateEnemies is false. | Off / On | 00:25.5–00:27.0 |
| Free Cam Enabled | Boolean | If true, spectators can control a "Free Cam" floating spectator pawn to observe the game | Off / On | 00:27.5–00:28.0 |
| Free Cam Enabled with Injunction Active | Boolean | If true, spectators can Free Cam even with injunctions blocking their respawn. | Off / On | 00:28.5–00:29.0 |
| One Shot One Kill | Boolean | If enabled, all weapons kill instantly | Off / On | 00:29.5 |
| Kill Score | Slider (integer) | Applied when a player scores a kill | -10 to 10 | 00:30.5–00:33.0 |
| Death Score | Slider (integer) | Applied when a player dies (but not when they commit suicide) | -10 to 10 | 00:33.5–00:36.5 |
| Assist Score | Slider (integer) | Applied when a player scores an assist. Only applied to personal score, never to team score. | -10 to 10 | 00:37.5–00:40.5 |
| Suicide Score | Slider (integer) | Applied when a player kills themselves | -10 to 10 | 00:41.0–00:43.5 |
| Friendly Fire Score | Slider (integer) | Applied when a player kills a teammate | -10 to 10 | 00:44.5–00:48.0 |
| Airdrops Enabled | Boolean | Whether airdrops are enabled | Off / On | 00:48.5–00:49.5 |
| Min Time Between Spawns | Slider (decimal) | The minimum time between triggering airdrop spawns. | 10.00 to 999.00 | 00:50.0–00:52.5 |
| Max Time Between Spawns | Slider (decimal) | The maximum time between triggering airdrop spawns. | 10.00 to 999.00 | 00:53.5–00:56.0 |
| Min Spawn Count | Slider (integer) | The minimum number of airdrops to spawn at a time. | 1 to 5 | 00:56.5–00:59.0 |
| Max Spawn Count | Slider (integer) | The maximum number of airdrops to spawn at a time. | 1 to 5 | 01:00.0–01:03.0 |
| Time Between Airdrops | Slider (decimal) | The time between each airdrop spawning when spawning multiple at a time. | 1.00 to 30.00 | 01:03.5–01:07.0 |
| Min Objective Range | Slider (decimal) | The minimum distance from an objective that an airdrop is allowed to spawn. This is not exact due to how airdrop volumes work, but instead uses the center of the volume's bounds to disqualify a volume for airdrop spawning. | 0.00 to 100,000.00 | 01:07.5–01:10.0 |
| Max Objective Range | Slider (decimal) | The maximum distance from an objective that an airdrop is allowed to spawn. This is not exact due to how airdrop volumes work, but instead uses the center of the volume's bounds to disqualify a volume for airdrop spawning. | 0.00 to 100,000.00 | 01:11.0–01:13.0 |
| Min Average Player Range | Slider (decimal) | The minimum distance airdrops should spawn from the average of all player positions. This is not exact due to how airdrop volumes work, but instead uses the center of the volume's bounds to disqualify a volume for airdrop spawning. | 0.00 to 100,000.00 | 01:13.5–01:16.0 |
| Max Average Player Range | Slider (decimal) | The maximum distance airdrops should spawn from the average of all player positions. This is not exact due to how airdrop volumes work, but instead uses the center of the volume's bounds to disqualify a volume for airdrop spawning. | 0.00 to 100,000.00 | 01:16.5–01:18.5 |
| Team Wipes Enabled | Boolean | If true, rounds will be ended on a team wipe. | Off / On | 01:19.5–01:20.0 |
| Score Limit Enabled | Boolean | Whether the score limit is enabled. | Off / On | 01:20.5–01:21.5 |
| Score Limit | Slider (integer) | The score at which the game will end. | 1 to 999 | 01:22.5–01:24.5 |
| Always Show Scores | Boolean | If enabled, indicates that scores should show up even when score limits aren't enabled. | Off / On | 01:25.0–01:25.5 |
| Override Score Display Type | Boolean | No description displayed. | Off / On | 01:27.5–01:28.0 |
| Score Display Type Override | Enum | No description displayed. | POINTS EARNED; FRACTION; PERCENTAGE | 01:26.5; 01:28.5–01:29.0 |

## Map

| Name | Type | Description | Allowed values | Video |
|---|---|---|---|---|
| Weapon Pickups Enabled | Boolean | If true, weapon pickups are enabled. | Off / On | 01:33.0–01:34.5 |
| Drop Only Equipped Weapon | Boolean | Drop only the currently equipped weapon on death. | Off / On | 01:35.5–01:37.0 |
| Life Span | Slider (decimal) | The amount of time before weapon pickups are destroyed (doesn't apply to pickups on item pads). | 1.00 to 120.00 | 01:37.5–01:41.5 |
| Power Weapon Life Span | Slider (decimal) | The amount of time before power weapon pickups are destroyed (doesn't apply to pickups on item pads). | 1.00 to 120.00 | 01:42.0–01:45.0 |
| Destroy Power Weapon Pickups Ammo Percentage | Slider (decimal) | If the power weapon pickup has less total ammo than this percentage of its magazine size, it will be destroyed. | 0.00 to 1.00 | 01:45.5–01:48.5 |
| Destroy Weapon Pickups Ammo Percentage | Slider (decimal) | If the weapon pickup has less total ammo than this percentage of its magazine size, it will be destroyed. | 0.00 to 1.00 | 01:49.0–01:52.5 |
| Destroy Pickups with No Ammo | Boolean | If true, weapon pickups with no ammo will be destroyed. | Off / On | 01:53.5–01:54.0 |
| Enable Map Boundaries | Boolean | Whether map boundaries are enabled. | Off / On | 01:54.5–01:55.0 |
| Item Pads Enabled | Boolean | If true, item pads will be made available at the start of the round. | Off / On | 01:55.5–01:56.0 |
| Item Respawning Enabled | Boolean | If true, item pads will respawn items after they are picked up within a round. | Off / On | 01:57.0–01:58.0 |
| Selection Behavior | Enum | Defines how item pads select their items. | FIRST IN LIST; RANDOM PER MATCH; RANDOM PER ROUND; RANDOM PER SPAWN | 01:58.5–02:02.5; 02:04.0 |

## Teams

| Name | Type | Description | Allowed values | Video |
|---|---|---|---|---|
| Allow Friendly Fire | Boolean | If true, players on the same team can damage each other. | Off / On | 02:06.5–02:07.0 |
| Allow Enemy Healing | Boolean | If true, enemies can be healed by allied abilities. | Off / On | 02:07.5–02:08.5 |
| Ally Collision | Boolean | If true, allied players can collide with each other. | Off / On | 02:09.0–02:10.0 |
| Enemy Collision | Boolean | If true, enemy players can collide with each other. | Off / On | 02:10.5–02:11.0 |
| Show Enemy Respawn Timers | Boolean | If true, enemy respawn timers can/should be shown on the HUD. | Off / On | 02:12.0–02:12.5 |
| Show Enemy Health | Boolean | If true, enemy health can/should be shown on the HUD. | Off / On | 02:13.5–02:14.0 |

## Players

| Name | Type | Description | Allowed values | Video |
|---|---|---|---|---|
| Max Health | Slider (decimal) | The Max Health the player spawns with. | 1.00 to 900.00 | 02:16.5–02:19.0 |
| Drop All Reserve Ammo | Boolean | If true, all reserve ammo for a weapon will be dropped when a weapon pickup is spawned. | Off / On | 02:20.0 |
| Infinite Magazine | Boolean | If true, weapons have infinite magazines. | Off / On | 02:21.0–02:21.5 |
| Infinite Reserves | Boolean | If true, weapons have infinite ammo reserves. | Off / On | 02:22.0–02:22.5 |
| Infinite Equipment | Boolean | If true, equipment has infinite uses. | Off / On | 02:23.0–02:23.5 |
| Damage Multiplier | Slider (decimal) | How much to multiply player outgoing damage by. | 0.25 to 2.50 | 02:24.0–02:28.0 |
| Melee Damage Multiplier | Slider (decimal) | How much to multiply player melee damage by. | 0.25 to 2.50 | 02:28.5–02:31.5 |
| Precision Damage Multiplier | Slider (decimal) | How much to multiply player precision damage by. | 0.25 to 2.50 | 02:32.0–02:35.0 |
| Precision Damage Only | Boolean | Whether to enable precision damage only (e.g. headshots). | Off / On | 02:35.5–02:36.0 |
| Enable Big Head Mode | Boolean | Whether big head mode is enabled. | Off / On | 02:36.5–02:37.0 |
| Movement Speed Multiplier | Slider (decimal) | Multiplier for the player's movement speed (and acceleration) | 0.25 to 2.50 | 02:37.5–02:41.0; 02:57.0 |
| Gravity Scale Multiplier | Slider (decimal) | Multiplier for the player's gravity scale | 0.25 to 2.50 | 02:41.5–02:44.0 |
| Jump Height Multiplier | Slider (decimal) | Multiplier for the player's jump velocity | 0.25 to 2.50 | 02:44.5–02:47.0 |
| Allow Beginning Recharge in Air | Boolean | Whether the thruster can start to recharge while the player is in the air or on a non-walkable surface. | Off / On | 02:48.0–02:49.0 |
| Allow Recharge After Teleport | Boolean | Whether the thruster recharge can start when you go through a portal but are in mid-air, even when Allow Beginning Recharge in Air is false. | Off / On | 02:49.5–02:50.0 |
| Thruster Recharge Delay | Slider (decimal) | Time we need to wait for the thruster to start recharging. | 0.00 to 100.00 | 02:50.5–02:52.0 |
| Lives Enabled | Boolean | If true, player respawns will be restricted based on their number of lives. | Off / On | 02:53.0 |
| Number Of Lives | Slider (integer) | The number of lives granted to players by default. | 1 to 100 | 02:54.0–02:56.5 |

## Loadouts

| Name | Type | Description | Allowed values | Video |
|---|---|---|---|---|
| Allow Loadout Changes During Gameplay | Boolean | No description displayed. | Off / On | 02:58.0 |

## Abilities

| Name | Type | Description | Allowed values | Video |
|---|---|---|---|---|
| Disable Radar | Boolean | If true, the radar will be disabled on player HUDs. | Off / On | 03:01.0 |
| Weapon Attacks Reveal Self on Radar | Boolean | If enabled, the player is revealed on their enemy's radar when they attack with their weapon. | Off / On | 03:02.0 |
| Radar Boundary Extent | Slider (decimal) | The distance of how far the radar can see (in world units) | -1.00 to 20,000.00 | 03:02.5–03:04.5 |
| Number of Portal Charges | Slider (integer) | Number of portal uses before needing to recharge. Set to 0 for unlimited. | 0 to 100 | 03:05.0–03:07.5 |
| Portal Gun Recharge Rate | Slider (decimal) | Recharge rate of our Portal Gun. Set to 0 to never recharge. | 0.00 to 300.00 | 03:08.0–03:10.0 |
| Refill All Portals on Recharge | Boolean | Whether to fill all portal charges at once on recharge or one at a time. | Off / On | 03:10.5 |
| Portal Wall Overloading | Boolean | Whether or not to overload a Portal Wall when you place portals on it | Off / On | 03:11.5 |
| Enable Portals | Boolean | Whether portals are enabled | Off / On | 03:12.0–03:12.5 |
| Allow Replacing Ally Portals | Boolean | No description displayed. | Off / On | 03:13.0–03:13.5 |
| Allow Replacing Enemy Portals | Boolean | No description displayed. | Off / On | 03:14.0–03:14.5 |
| Block Replacement Time | Slider (decimal) | The amount of time after placement that a portal can't be replaced by other players. Set to 0 to always allow replacement. | 0.00 to 10.00 | 03:15.0–03:18.0 |
| Equipment Cooldown Multiplier | Slider (decimal) | Multiplier for the equipment cooldown | 0.10 to 10.00 | 03:18.5–03:20.5 |
| Thruster Usage Multiplier | Slider (decimal) | Multiplier for how long a player can use the thruster | 0.25 to 2.50 | 03:21.0–03:23.0 |
| Thruster Acceleration Multiplier | Slider (decimal) | Multiplier for the thruster's acceleration | 0.25 to 2.50 | 03:23.5–03:25.5 |
| Enable Sprint | Boolean | Whether sprinting is enabled | Off / On | 03:26.0–03:26.5 |
| Enable Thruster | Boolean | Whether thruster is enabled | Off / On | 03:27.0–03:27.5 |

## Bots

| Name | Type | Description | Allowed values | Video |
|---|---|---|---|---|
| Bots Enabled | Boolean | If true, bots will be spawned | Off / On | 03:29.0–03:30.0 |
| Auto Rebalance | Boolean | If true, bots will automatically try to rebalance teams if players join or leave during a round. | Off / On | 03:30.5–03:31.0 |
| Spawn Custom Num Bots | Boolean | If true, will spawn a custom number of bots. If false, will spawn bots until all player slots are filled. | Off / On | 03:31.5–03:32.0 |
| Custom Bot Num | Slider (integer) | A custom number of bots to spawn | 0 to 24 | 03:32.5–03:35.0 |

## Spawning

| Name | Type | Description | Allowed values | Video |
|---|---|---|---|---|
| Respawn Time | Slider (decimal) | The amount of time after dying that the player can respawn. | 0.00 to 999.00 | 03:37.0–03:39.0 |
| Death Respawn Time Penalty | Slider (decimal) | Dead player gets this penalty applied to their respawn time (can be negative). | -999.00 to 999.00 | 03:39.5–03:41.5 |
| Kill Respawn Time Penalty | Slider (decimal) | Killer gets this penalty applied to their respawn time (can be negative). | -999.00 to 999.00 | 03:42.0–03:44.5 |
| Periodic Penalty Time | Slider (decimal) | If > 0, this is the repeating period after which all players' respawn penalties will increase. | 0.00 to 999.00 | 03:45.0–03:47.0 |
| Periodic Penalty Amount | Slider (decimal) | If not 0, this is the amount by which all players' respawn penalties will increase after PeriodicPenaltyTime. | -999.00 to 999.00 | 03:47.5–03:49.0 |
| Respawn Penalty Min | Slider (decimal) | Minimum value for respawn penalty. | -999.00 to 999.00 | 03:49.5–03:51.5 |
| Respawn Penalty Max | Slider (decimal) | Maximum value for respawn penalty. | -999.00 to 999.00 | 03:52.0–03:54.0 |
| Death in Progress Respawn Modifier | Slider (decimal) | Dead players (and their teammates, if team penalties are enabled) get this modifier applied to their current respawn time (can be negative). Note: The description says this can be negative, but the demonstrated slider minimum is 0.00. | 0.00 to 999.00 | 03:54.5–03:56.5 |
| Kill in Progress Respawn Modifier | Slider (decimal) | Killers (and their teammates, if team penalties are enabled) get this modifier applied to their current respawn time (can be negative). Note: The description says this can be negative, but the demonstrated slider minimum is 0.00. | 0.00 to 999.00 | 03:57.0–03:58.5 |
| Allow Timed Respawns | Boolean | If false, the timed respawn component will never trigger a respawn by itself. | Off / On | 03:59.5–04:00.0 |
| Team Based Respawn Penalties | Boolean | If true, team-based games will apply kill/death respawn penalties to the entire team rather than individual players. If false, kill/death respawn penalties will only apply to instigator/target. | Off / On | 04:00.5–04:01.5; 04:35.0 |
| Always Use Team Spawns | Boolean | If true \*and\* in a team game, requires the use of team-specific spawns. This enables "CTF-style" spawning, where teams only ever spawn in their own bases. | Off / On | 04:02.5–04:03.0 |
| Require Nearby Allies | Boolean | If true, only spawns with allies nearby will be considered. This is a simple "is an ally nearby" check, it is not weighted like enemies are. If there are no allies found then this option is ignored. This option isn't super useful for normal arena maps. | Off / On | 04:03.5–04:04.0 |
| Require Nearby Objective | Boolean | If true, only spawns with objectives nearby will be considered. This is a simple "is an objective nearby" check, it is not weighted like enemies are. If there are no objectives found then this option is ignored. | Off / On | 04:04.5–04:05.0 |
| Require No Nearby Objective | Boolean | If true, only spawns with objectives beyond a specific distance will be considered. | Off / On | 04:05.5–04:06.0; 04:35.5–04:36.0 |
| Ally Consideration Distance | Slider (decimal) | The max distance from an ally for a spawn to be considered when bRequireNearbyAllies is on. | 0.00 to 50,000.00 | 04:06.5–04:09.5 |
| Objective Max Distance | Slider (decimal) | The maximum distance away from objectives that a player should spawn at. Only used if bRequireNearbyObjective is enabled. | 0.00 to 50,000.00 | 04:10.0–04:11.0; 04:12.0–04:13.0 |
| Objective Min Distance | Slider (decimal) | The minimum distance away from objectives that a player should spawn at. Only used if bRequireNoNearbyObjective is enabled. | 0.00 to 50,000.00 | 04:13.5–04:16.0 |
| Enemy Portal Spawn Sort Weight | Slider (decimal) | How much linked enemy portals influence spawn location selection (higher is less influence). | 0.00 to 10.00 | 04:16.5–04:19.0 |
| Enemy Unlinked Portal Spawn Sort Weight | Slider (decimal) | How much unlinked enemy portals influence spawn location selection (higher is less influence). | 0.00 to 10.00 | 04:19.5–04:21.5 |
| Enemy Portal Wall Spawn Sort Weight | Slider (decimal) | How much enemy-viewed Portal Walls influence spawn location selection (higher is less influence). Note: The clip shows 5.00 but does not demonstrate the slider endpoints. Minimum and maximum are unknown. | Unknown range; 5.00 shown | 04:22.4 |
| Enemy Far Distance | Slider (decimal) | Distance at which an enemy actor is considered far away. The spawn will be assumed to not be visible if an enemy is far away and the spawn is behind them. | 0.00 to 50,000.00 | 04:22.5–04:24.5 |
| Enemy Portal Wall Consideration Distance | Slider (decimal) | The distance at which Portal Walls will be searched for when finding ones within line of sight of enemies. | 0.00 to 50,000.00 | 04:25.0–04:28.0 |
| Enemy Portal Consideration Distance | Slider (decimal) | The distance at which portals will be searched for when finding ones within line of sight of enemies. | 0.00 to 50,000.00 | 04:29.0–04:31.0; 04:34.0–04:34.5 |
| Prevent Spawning when Team Is Dead | Boolean | If true, blocks respawning once your team is dead. | Off / On | 04:33.4 |
