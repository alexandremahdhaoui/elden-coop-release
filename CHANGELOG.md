# Elden Coop Changelog

Elden Coop lets friends play Elden Ring together in one shared world. The newest version comes first.

The host is the player who owns the world. A guest is a player who joins the host's world. The party is every player in that world. A session is the time the party plays together.

## v0.0.26

November 21, 2026. All players must update.

This update fixes the graces of a guest after a trip to Roundtable Hold, a boss that kept fighting after the whole party died, map fragments, items that a player got twice and the place where a guest joins again.

### New features

- Added a message for players who play two different versions of Elden Coop. The message tells the player with the older version to update Elden Coop.

### Changes

- Changed the bug report. A bug report now holds the last two runs of the game and the crash files from those runs. A bug report is now much smaller.
- Changed resting at a grace. The enemies come back only when every player in the world rests. A player who is dead or in a loading screen keeps the enemies from coming back. A player at the title screen does not count.
- Changed graces. When one player lights a grace, the game lights that grace for every player in the party. No other player has to touch that grace.
- Changed what happens when every player in a boss fight dies. Each player who fought the boss gets a loading screen. A player who fought the boss gets the loading screen even at a grace. A player who did not fight the boss gets no loading screen. A player who leaves the session during a boss fight counts as a dead player in that fight. A boss fight ends when the party defeats the boss.

### Bug fixes

- Fixed a bug where a guest could not light a grace or rest at a grace after the party left Roundtable Hold.
- Fixed a bug where a boss kept fighting after every player in the fight died. Now the boss fight starts over for each player who fought the boss when all of those players die.
- Fixed a bug where a map fragment that one player found did not open the map for the other players. Now a map fragment opens the map for the whole party.
- Fixed a bug where a guest got the same items again each time the guest joined a world. Now each character of a guest gets each item of a world once. Now a new character in the slot of a deleted character also gets every item of the world.
- Fixed a bug where each player got the reward of a boss twice. Now each player gets the boss reward once.
- Fixed a bug where the game stopped for a moment when a player got an item from another player. Now the game keeps running while a player gets an item from another player.
- Fixed a bug where a guest who lost the session and joined again started far from the host. Now the guest joins again at the place of the host.
- Fixed a bug where the main menu did not show the Elden Coop version.
- Fixed a bug where the main menu opened on LOAD GAME or NEW GAME after a player started a world from the Elden Coop menu. Now the main menu opens on its usual row.
- Fixed a bug where the map did not show the name of another player. Now the map shows the name of each player under the marker of that player.
- Fixed a bug where a player saw another player on foot while that player rode Torrent. Now the game puts that player on Torrent.
- Fixed a bug where a player who rode Torrent stayed in an old place on the screens of the other players. Now the game puts that player in the right area of the map.

### Known issues

- When a player dies far from a Stake of Marika, the game still reloads the area for that player.
- When the host dies far from a Stake of Marika in a boss fight, the boss can start over for the other players.
- When one player finds a map fragment, the other players find no map fragment at that spot. The map is already open for them.
- The first time a guest joins a world after this update, the guest gets the items of that world once more.
- When a player stands up at a Stake of Marika inside a boss fight and the boss bar does not show again, the game can reload the area for that player when the other players in the fight die.
- When a player dies in a boss fight and walks back before the rest of the party dies, that player gets a second loading screen.
- When the host or a guest plays v0.0.25 or an older version, the guest sees no message about the other version.
- Outside Limgrave, some NPCs may not share talks and quest progress with the whole party.

## v0.0.25

November 19, 2026. All players should update.

This update fixes how a player sees the other players in the world and on the map. This update also adds a What's new link and an Uninstall link to the launcher.

### New features

- Added a What's new link under the version in the launcher. The What's new link shows the changes of each version.
- Added a gold dot beside the What's new link. The gold dot shows after the launcher updates.
- Added an Uninstall link to the launcher. The Uninstall link removes the mod files and the Elden Coop certificates from the PC. The Uninstall link keeps the coop worlds, the party chest, the save backups and elden_coop.ini.

### Changes

- Changed the launcher window. The launcher no longer shows the red button for the Elden Coop certificates. The Uninstall link now removes the Elden Coop certificates.
- Changed what happens when a player dies near a Stake of Marika while another player in the party is alive. The player stands up at the Stake of Marika with no loading screen.

### Bug fixes

- Fixed a bug where other players blinked or jumped from place to place.
- Fixed a bug where the name and the health bar of another player disappeared.
- Fixed a bug where the map showed another player in the wrong place.
- Fixed a bug where a guest saw a lit grace as unlit after a loading screen. Now a guest can rest at a lit grace after every loading screen.

### Known issues

- When a player dies far from a Stake of Marika, the game still reloads the area for that player.
- When a player dies far from a Stake of Marika in a boss fight, the boss fight can start over for the other players.
- Outside Limgrave, some NPCs may not share talks and quest progress with the whole party.

## v0.0.24

November 18, 2026. All players must update.

This update adds shared quest progress, a shop stock for each player, and a new rule for resting.

### New features

- Added shared quest progress. Every player can talk to every NPC. Two players can talk to the same NPC at the same time. When one player takes a quest step, the quest step counts for the whole party.
- Added a separate shop stock for each player. When one player buys a limited item, the other players can still buy that item. When one player unlocks something such as the Crafting Kit, the whole party still gets the unlock.
- Added the character name under each player's marker on the map.
- Added the boss health bar and the boss music for guests in every boss fight.

### Changes

- Changed resting at a grace. When a player rests while another player is out in the world, the enemies do not come back. The player who rests still heals, refills flasks and can level up. The enemies come back when every player rests or when the whole party dies.

### Bug fixes

- Fixed a bug where a boss froze in the middle of a fight.
- Fixed a bug where some NPCs, such as D, stopped talking to a guest right away.
- Fixed a bug where one player saw an NPC and another player did not see that NPC.
- Fixed a bug where a guest's Torrent stayed hidden after Torrent died. Now Torrent comes back when the guest whistles again.
- Fixed a bug where an Evergaol fight broke when a player crossed a map border inside the arena.
- Fixed a bug where a bug report was empty after the game crashed.
- Fixed a bug where a guest could not join again after the guest's game crashed during a join. Now the host's game recovers by itself.

### Known issues

- Other players may blink or jump from place to place. Fixed in v0.0.25.
- The name and the health bar of another player may disappear. Fixed in v0.0.25.
- The map may show another player in the wrong place. Fixed in v0.0.25.
- When a player dies, the game reloads the area for that player.
- When a player dies in a boss fight, the boss fight can start over for the other players.
- Outside Limgrave, some NPCs may not share talks and quest progress with the whole party.

## v0.0.23

November 18, 2026. All players must update.

This update makes an Evergaol fight a fight for the whole party. This update also fixes problems when a guest cannot join.

### New features

- Added party fights in Evergaols. When one player touches an Evergaol seal, every player enters the same fight. The game first moves a player who is far away to the seal. A player who is in another boss fight stays in that boss fight and gets a message.

### Changes

- Changed what the game does when a guest cannot join. The game tries again after 2, 4, 8, 16 and 30 seconds. The game stops after six tries and shows a message. The guest can pick the GO TO row of the party page to try again.

### Bug fixes

- Fixed a bug where the host's game crashed when a guest failed to join many times in a row.
- Fixed a bug where a guest stood frozen inside an Evergaol.
- Fixed a bug where the boss music did not play inside an Evergaol.
- Fixed a bug where the other players often did not see a guest's Torrent.
- Fixed a bug where the other players often saw a dead player freeze or jump.

### Other

- Improved bug reports. A bug report is now one file. A bug report now holds more details about Torrent, map markers and lost connections.

### Known issues

- When a guest's game crashes while the guest joins, the guest may not be able to join again. Workaround: the host hosts the world again.
- When a player dies in an Evergaol, the game reloads the area for that player.
- When a player dies in an Evergaol, the Evergaol fight can start over for the other players.
- Outside an Evergaol, a guest may get no boss health bar and no boss music.
- Some NPCs stop talking to a guest right away.

## v0.0.22

November 18, 2026. All players must update.

This update fixes problems with bosses, guests, merchants, fast travel and the party chest.

### New features

- Added the boss reward for guests who join late. When a guest joins after the party beat a boss, the guest gets the reward item of that boss once.

### Bug fixes

- Fixed a bug where the game removed players from the session after the party beat a boss.
- Fixed a bug where a guest who died did not come back as a normal, visible character.
- Fixed a bug where merchants and other NPCs did not talk or trade with a guest.
- Fixed a bug where a guest could not open the grace list on the map. Now a guest can fast travel from the grace list.
- Fixed a bug where a guest's dead Torrent did not come back after the guest rested at a grace.
- Fixed a bug where a guest who joined again lost the progress of the world. Now a boss that the party beat stays beaten.
- Fixed a bug where the host's clock moved when a guest rested at a grace.
- Fixed a bug where the party chest showed a wrong item count.
- Fixed a bug where a player could not take back a single item from the party chest.
- Fixed a bug where the party chest showed wrong items after a player rested at a grace and refilled several items.
- Fixed a bug where shops, crafting and smithing used items from the party chest. Now shops, crafting and smithing use the items a player carries, like in the base game.
- Fixed a bug where the party chest could lose or copy an item.

### Other

- Improved bug reports. A bug report now holds more details about Torrent, player markers and the map.

### Known issues

- When a guest cannot join, the game tries again at once. Many tries in a row can crash the host's game. Workaround: the guest goes back to the title menu. The host then hosts the world again. The guest then joins again.
- When a guest's game crashes while the guest joins, the guest cannot join again. Workaround: the host hosts the world again.
- The other players sometimes do not see a guest's Torrent.
- Other players can blink or jump from place to place.
- In an Evergaol, the game of each player runs its own fight. A second player can stand frozen in the Evergaol. A player who dies and enters the Evergaol again may see no boss.
- A guest sometimes gets no boss health bar and no boss music.
- Some NPCs stop talking to a guest right away.

## v0.0.21

November 18, 2026.

This update makes a guest a full player. This update also fixes the split worlds of v0.0.20.

### New features

- Added full player status for guests. A guest no longer joins as a summoned phantom. A guest can use graces, the smithing table, shops and Torrent. A guest no longer has the phantom glow.
- Added the full flask count for guests.
- Added item pickups from the ground for guests.

### Bug fixes

- Fixed a bug where each PC ran its own copy of the world. Now every player sees the same enemies, the same movement and the same names. Now every player gets runes from each kill.
- Fixed a bug where a guest got stuck while joining.
- Fixed a bug where the frame rate dropped.

### Other

- Improved bug reports. A bug report now shows the role of each player. A bug report now shows whether the character of another player is still loading.

## v0.0.20

November 17, 2026. Use v0.0.21, not this version.

### Bug fixes

- Fixed a bug where a guest could not use graces or Torrent.
- Fixed a bug where a guest could not see the host after the host died.

### Other

- Improved bug reports. A bug report now uses one time format. A bug report now shows when an NPC gift is missing.

### Known issues

- Each PC runs its own copy of the world. Each player sees different enemies, different movement and different names. Fixed in v0.0.21.

## v0.0.19

November 17, 2026.

### Bug fixes

- Fixed a bug where the host and a guest could not see each other for the whole session. The bug happened when a guest joined while the host stood in the first chapel. Now the guest joins again by itself when the host leaves the first chapel.
- Fixed a bug where a guest got no new try after the host's game refused the guest.

## v0.0.18

November 17, 2026. All players must update.

### New features

- Added the actions of the character page to the game's button bar. The actions are Create, Delete, Import, and World options for worlds you host.
- Added the world name to the title of the character page.
- Added the message "The host left the world" for guests. When the host leaves, a guest sees the message and goes back to the guest's own world.

### Changes

- Changed party chest moves. A party chest move now ends after 30 seconds. A player who crashes or leaves can no longer lock items in the party chest.

### Bug fixes

- Fixed a bug where a player who played alone could not skip a cutscene.
- Fixed a bug where a guest stayed stuck in a session after the host lost the connection.
- Fixed a bug where the rows of the Multiplayer menu did not line up with the game's menu.
- Fixed a bug where the cursor of the Multiplayer menu started on the wrong row.
- Fixed a bug where a player could put a unique quest item into the party chest. Now a unique quest item stays with its owner.
- Fixed a bug where the items a player picked up did not stay personal on every PC.
- Fixed a bug where the party chest could copy an item when the game crashed during a party chest move.

### Other

- Improved crash files and bug reports. A bug report now shows how much time the mod uses each frame.

## v0.0.17

November 6, 2026.

### Bug fixes

- Fixed a bug where Windows blocked the mod from loading.

## v0.0.16

November 6, 2026.

This update adds the party chest.

### New features

- Added the party chest. The party chest is one shared storage for the whole party. A player can open the party chest at every grace. The party chest holds goods, weapons, armor, talismans and ashes. The party chest gives materials for crafting. The party chest keeps its items when the game crashes.
- Added character cards. Each world now opens on the characters of that world, with the game's own load cards.
- Added a way to rename a character.
- Added a way for any player to pass time at a grace.
- Added gifts for guests who join late. A guest who joins late gets every gift that the party already has in that world.
- Added a way for any player to skip a cutscene for the whole party.
- Added the host's Great Rune effect for guests. A guest loses the Rune Arc when the guest dies, like the host.
- Added the Arxan disabler. The Arxan disabler makes the game run smoother. The Arxan disabler is on by default. A player can turn the Arxan disabler off in elden_coop.ini.

### Bug fixes

- Fixed a bug where the cursor left a world after a player went back from the characters of that world.
- Fixed a bug where save backups kept too many copies. Now save backups keep the five newest copies.
- Fixed a bug where a gift from another player could make the game unstable.

## v0.0.15

November 3, 2026.

### New features

- Added separate progress for each world. The host loads the progress of a world each time the host enters that world.
- Added gifts for every player. A gift such as Torrent now reaches every player.
- Added shared cutscenes. The whole party now watches a cutscene together.
- Added the Elden Coop version to the main menu.

### Bug fixes

- Fixed a bug where the world clock moved when a player died.
- Fixed a bug where the other players could not see a guest after the guest came back to life.

## v0.0.14

November 2, 2026.

### Bug fixes

- Fixed a bug where a guest could not finish joining when the host warped. Now the game waits for the guest before the game warps the host.
- Fixed a bug where Melina gave Torrent to only one player.
- Fixed a bug where the button prompts did not match the device a player uses.
- Fixed a bug where an error in the mod closed the game.

## v0.0.13

November 1, 2026.

### New features

- Added the Elden Coop version to the title menu.

## v0.0.12

November 1, 2026.

### New features

- Added a row on the party page that saves a bug report.

### Changes

- Changed the menus. A player now reaches a world in fewer presses.

### Bug fixes

- Fixed a bug where some world events stayed on one PC.

## v0.0.11

November 1, 2026.

### Bug fixes

- Fixed a bug where doors and events were different for each player.

### Other

- Improved crash files. A crash file now holds more details.

## v0.0.10

November 1, 2026.

This update adds the party page. This update also removes the base game's limits for sessions.

### New features

- Added a party page to the Esc menu. The party page lists the party, sends invites, warps a player to another player and marks a moment for a bug report.
- Added a way to join a world again with no new invite.
- Added Torrent in a session.

### Changes

- Changed how a guest looks. A guest now looks like a normal character with no red glow.
- Changed the session limits. Every player can now use any item. The limits on fast travel, rune recovery and spirit ashes are gone.
- Changed where an imported character starts. An imported character now starts at the first grace of that character.

### Bug fixes

- Fixed a bug where many world events ran at once when a player entered a world.

## v0.0.9

October 31, 2026.

### Changes

- Changed how a guest joins. A guest now joins as a white phantom.
- Changed the server login. The FromSoftware server login now stays off during a session.

### Bug fixes

- Fixed a bug where a guest lost the host after the connection broke. Now the guest follows the host to the new lobby of the host.

## v0.0.8

October 31, 2026.

### New features

- Added Steam networking. Game data now travels over Steam. Only players in the lobby can connect.

### Changes

- Changed map loads. Players now stay connected when the game loads a map.

## v0.0.7

October 31, 2026.

### New features

- Added graces and Torrent in a session.
- Added invite keys and join messages.

### Bug fixes

- Fixed a bug where a guest could reach the host only in some areas.

## v0.0.6

October 31, 2026.

### Bug fixes

- Fixed a bug where Windows could block a new release.

## v0.0.5

October 31, 2026.

### New features

- Added a Check for updates button.
- Added the Host, Join and Characters pages to the menu.
- Added worlds for up to six players.

## v0.0.4

October 31, 2026.

### New features

- Added world creation with a name and a player limit.
- Added a way to import or copy a character from another world or from the normal save.
- Added personal progress. Personal progress stays with each player.

### Bug fixes

- Fixed a bug where the session ended when the game loaded a map.
- Fixed a bug where a failed update broke the launcher. Now the launcher brings back the old version when an update fails.

## v0.0.3

October 31, 2026.

### New features

- Added sessions for two players with shared world progress.
- Added one launcher with automatic updates and save backups.

## v0.0.2

October 31, 2026.

### Bug fixes

- Fixed a bug where the first public build had packaging problems.

## v0.0.1

October 31, 2026.

### New features

- Added the Multiplayer menu to the title screen. The Multiplayer menu holds the coop worlds of a player.
- Added a separate save file for each world. The normal save of a player stays untouched.
- Added character creation and character loading inside each world.
