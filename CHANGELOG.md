# Elden Coop Changelog

Elden Coop lets friends play Elden Ring together in one shared world. The newest version comes first.

The host is the player who owns the world. A guest is a player who joins the host's world. The party is every player in that world. A session is the time the party plays together.

## v0.0.31

November 27, 2026. All players must update.

This update removes an item from the world of every player when one player picks that item up, fixes a fall through the floor after GO TO, and stops Melina from offering the trip to Roundtable Hold after each join.

### Changes

- Changed where GO TO takes a player when a friend fights a boss behind a fog. The player now arrives at the spot where the friend walked into the fog. The player walks through the fog to join the friend. When the game does not know that spot, the player arrives at a grace near the fight.
- Changed the party message for an item that another player picks up. The party message now names the player and the item, such as "Tarnished picked up Golden Seed".
- Changed the game so that the game no longer opens the microphone of a player during a session. Elden Coop has no voice chat.

### Bug fixes

- Fixed a bug where an item that one player picked up stayed in the world of the other players. Now the item disappears from the world of every player in the party as soon as one player picks the item up.
- Fixed a bug where a player who used GO TO to reach a friend in a boss fight fell through the floor and died. Now the game holds the player in place until the floor under the player is ready.
- Fixed a bug where the game counted a boss as defeated after that boss fell through the floor with no fight. Now the game holds the boss in place until the floor under the boss is ready.
- Fixed a bug where Melina offered a guest the trip to Roundtable Hold again at the first rest after each join. Now Melina makes that offer to a guest only once.
- Fixed a bug where a guest lost the Level Up option at a grace and the talk with Melina after a join. Now the game checks the guest before every join and reloads the guest first when the check fails.
- Fixed a bug where a guest had to join the host again from the title screen when the session ended in the middle of a join. Now the game waits for the old session to close, reloads the guest at the last grace and joins the host again.
- Fixed a bug where the game of a player froze for more than one second during a session. Now the game keeps running during a session.
- Fixed a bug where the game froze for about one second when a session started on a PC that uses a Bluetooth headset as the microphone. Now the game does not open the microphone.
- Fixed a bug where a friend on Torrent moved in small jumps when the friend was far away. Now a friend on Torrent moves smoothly when the friend is far away.
- Fixed a bug where a guest who stood on a lift fell to the bottom when the host used the same lift. Now the guest stays on the lift.

### Known issues

- A lift sometimes does not move for a guest who stands on the lift at the top.

## v0.0.30

November 26, 2026. All players must update.

This update changes how a guest joins the host again after a lost connection.

### Changes

- Changed what happens when a guest loses the connection to the host three times in a row. The game now stops and tells the guest to join again from the Multiplayer menu.

### Bug fixes

- Fixed a bug where a guest who lost the connection to the host joined the host again at once, with no reload. Now the game reloads the guest at the last grace of that guest and then joins the host again.
- Fixed a bug where a short press of F9 did not mark the moment in the bug report. Now every press of F9 marks the moment.

### Known issues

- A guest can lose the Level Up option at a grace, the talk with Melina and the use of lifts during a session. Workaround: the guest quits to the title screen and joins the host again.

## v0.0.29

November 25, 2026. All players must update.

This update fixes players on Torrent who appeared high in the sky, fixes friends who stayed invisible after GO TO, and gives the column of light over a friend a new look.

### New features

- Added the setting "Column of light fades toward the top". The setting is on by default. When the setting is on, the column of light over a friend is strong near the ground and fades smoothly toward the sky. When the setting is off, the column of light keeps the same strength from the ground to the top of the screen.

### Changes

- Changed the column of light over each friend. The game now draws the column of light as a round column with a bright edge on each side and a clear middle. The column of light rises to the top of the screen. The column of light is faint when the friend is near and bright when the friend is far away. The game draws no column of light over a friend who stands next to the player.
- Changed the path to a friend. The game now draws the path as a dark shade that a player can see the ground through.
- Changed how the host treats a guest with a lost connection. When the host cannot reach a guest for 30 seconds, the host removes that guest from the party. When the connection of that guest works again, the game tells that guest that the session ended.

### Bug fixes

- Fixed a bug where one guest with a bad connection stopped the host from sending world progress to the guests who joined after that guest. Now the host keeps sending to every other guest.
- Fixed a bug where a guest could wait forever to enter the world of the host when a message got lost during the join. Now the guest asks the host again after 20 seconds.
- Fixed a bug where the party chest kept an item for a long time after the player who took that item lost the connection. Now the party chest gives that item back after 30 seconds.
- Fixed a bug where a player on Torrent appeared high in the sky on the screen of another player. Now the game shows a player on Torrent on the ground.
- Fixed a bug where a player who got on Torrent jumped back and forth between the saddle and the place where the player got on, for up to 2 seconds. Now the game shows that player in the saddle at once.
- Fixed a bug where a friend stayed invisible after that friend used GO TO to reach a player in a dungeon. Now the game shows that friend next to the player within a few seconds.
- Fixed a bug where the column of light over a friend stood far away from that friend. Now the column of light stands at the last known place of that friend.
- Fixed a bug where the column of light flashed in the wrong place when a friend appeared. Now the column of light appears half a second after that friend does.
- Fixed a bug where a player who rested at a grace and then died while a friend was alive stood up high in the air and then got a loading screen. Now the player stands up at the grace with no loading screen.
- Fixed a bug where the game reloaded the area for a player who stood up with no loading screen while the body of that player was still falling. Now the game reloads the area only when the body of that player does not come back.

### Other

- Improved the work that Elden Coop does in the background while a player plays. Elden Coop now needs much less time to keep the game clock, to save the progress of the world and to welcome a friend who joins.

## v0.0.28

November 24, 2026. All players must update.

This update gives the whole party each item that one player finds, adds crafting with the materials in the party chest and NPC invaders for the party, and fixes sessions that broke, boss items, messages about friends and the path to a friend.

### New features

- Added crafting with the materials in the party chest. When a player crafts an item, the game moves the missing materials from the party chest into the inventory of that player.
- Added the materials in the party chest to the crafting page. The number beside each material counts the materials in the inventory and in the party chest.
- Added NPC invaders for the party. When any player walks into the place where an NPC invades, the NPC invades the world of the host. Every player in the party can fight that NPC invader.
- Added items for the whole party. When a player picks up an item from a chest, a corpse or the ground, the game gives the same item to every other player in the party. A player who joins the world later gets every item that the party found before. Plants and other materials that grow back stay with the player who picks them up.
- Added a party message for items from the party. When the party gives a player an item, the game shows a message to that player. The game shows the message about items from the party even when the player turns off the setting Party messages.
- Added the setting Items from friends. When a player turns the setting Items from friends off, the party gives that player no items from chests, corpses or the ground. The other players in the party still get each item that the player picks up.
- Added the setting Stand up with no loading screen. When a player turns the setting Stand up with no loading screen off, the player gets the loading screen of the base game after each death.

### Changes

- Changed the fight view during an NPC invasion. When a player who watches presses X or F7 twice and the last grace is in another part of the map, the player stands up where the player died. The NPC invader stays in the world of the host.
- Changed the column of light over each friend. The game now draws the column of light as a tall ring of bars. A player sees the column of light through walls.
- Changed the end of the path to a friend. When the path stops before the friend, a small column of light stands at the end of the path.
- Changed the messages about friends. The game shows each message about a friend in the game's own message box.
- Changed the message that a guest sees when the host leaves. The message now names the host.
- Changed the last rest of the party at a grace. The last player to rest at a grace sees the screen go black two times again.
- Changed items that a player already got from the party. When the player picks up the same item in the world, the game removes the item and gives nothing.
- Changed items from the party. The game now puts each item from the party in the inventory with no item box. The party message tells the player about the items. A player who joins the world late gets the items from the party one after the other.
- Changed items from the Land of Shadow. A player without Shadow of the Erdtree gets no item that the party found in the Land of Shadow. A player who buys Shadow of the Erdtree gets the item the next time that player enters the world.

### Bug fixes

- Fixed a bug where a party message said that a guest lit a grace when the host lit that grace. Now the party message names the player who lit the grace.
- Fixed a bug where party messages and the GO TO rows of the Multiplayer page showed the Steam name of a player. Now the game shows the character name of that player.
- Fixed a bug where the path to a friend went away when the game did not load the body of that friend. Now the path leads toward the last known place of that friend in the open world.
- Fixed a bug where the path to a friend showed as a wide white band. Now the game draws the first 40 meters of the path as a thin dark line on the ground.
- Fixed a bug where the path to a friend went away for 30 seconds or more when that friend was far away. Now the path leads toward a far friend. When the game finds only a part of the way, the path shows that part.
- Fixed a bug where the path to a friend blinked on and off when the body of that friend jumped between two places. Now the game keeps the last path on the ground for up to 10 seconds while the body of that friend jumps.
- Fixed a bug where the path went back to the nearest friend after the player traveled to a grace. Now the path keeps the friend that the player picked.
- Fixed a bug where the game reloaded the area for a player who stood up at a grace and walked back into a boss fight when the other players died. Now the game counts that player in the boss fight while the player stands in the boss arena.
- Fixed a bug where a player who rode Torrent could stay on foot on the screen of another player. Now the game puts that player back on Torrent.
- Fixed a bug where a player who got on Torrent kept jumping between two places on the screens of the other players. Now the game tries to stop that jump about two seconds after the jump starts.
- Fixed a bug where the Torrent of a player could stand in the wrong place on the screens of the other players. Now each game sends the place of its own Torrent to the other players.
- Fixed a bug where a player got the items of a defeated boss again each time the player joined a world. Now a player gets the items of each boss only once.
- Fixed a bug where normal enemies kept their health when a friend joined or left the party. Now the game changes the health of normal enemies when the party changes.
- Fixed a bug where an item from the party could go to another character of the player after the player quit to the main menu. Now an item from the party goes only to the character that played in the session.
- Fixed a bug where a player could get the same item from the party twice. Now a player gets each item from the party once.
- Fixed a bug where a guest without Shadow of the Erdtree was sent into the Land of Shadow when the host stood there. Now that guest joins the world at the place where the guest stands.
- Fixed a bug where an NPC could stay at an old step of a quest for a player who heard a missed NPC line. Now the NPC moves on with the quest after the player hears the line.
- Fixed a bug where the path to a friend could stay hidden after a loading screen. Now the path shows again a few seconds after the load.
- Fixed a bug where the game could crash in rare cases when a session started or ended.
- Fixed a bug where a door that a friend opened with a key in an earlier session could stay shut for a player. Now the door opens when that player joins the world.
- Fixed a bug where a player could still get Baldachin's Blessing twice when the game of that player gave Baldachin's Blessing late. Now a player gets Baldachin's Blessing once.
- Fixed a bug where a player missed a map fragment when the game failed to give the map fragment. Now the game tries again to give the map fragment.
- Fixed a bug where some NPCs in the Land of Shadow reacted to a friend who stood far away. Now those NPCs react to the player who stands near them.
- Fixed a bug where a guest who walked away from an NPC invader sent that NPC invader home for the whole party. Now the NPC invader goes home only when every player walks away from the NPC invader.
- Fixed a bug where the host could no longer see an NPC invader after the host died. Now a player who dies while a friend fights an NPC invader watches the fight. The player who died comes back when the NPC invader is gone.
- Fixed a bug where a guest who lost the session came back at the start of Limgrave. Now the guest joins the host again from the world of that guest and arrives next to the host.
- Fixed a bug where a guest who could not join the host again waited on a loading screen for more than a minute. Now the guest goes back to the world of that guest and sees a message that the session ended.
- Fixed a bug where GO TO moved the host to the start of Limgrave long after the host picked GO TO. Now GO TO moves a player only to a friend who plays in the same session.
- Fixed a bug where a guest could not join the host again for two minutes after a boss fight. Now a guest can join the host again as soon as the boss falls.
- Fixed a bug where a player who was dead when the party defeated a boss got no runes from that boss. Now every player who fought the boss gets the runes once.
- Fixed a bug where a guest could mark a boss as defeated after a session broke. Now a guest marks a boss as defeated only after that guest fought the boss.
- Fixed a bug where a guest who lost the session could not join the host again until the host quit the game. Now the game of the host restarts the session after the first failed join of that guest. The host and the guest each see a short message. Each other guest goes back to the world of that other guest and then joins the restarted session.
- Fixed a bug where a player who died and watched a boss fight kept watching after the party defeated some bosses. Now the fight view ends when the boss falls.
- Fixed a bug where the column of light over a friend went away when the game did not load the body of that friend. Now the column of light stands at the last known place of that friend in the open world.
- Fixed a bug where a player who kept pressing X or F7 after the fight view ended could stand up at the place of death during the loading screen. Now the game ignores those presses while the area loads.
- Fixed a bug where a player who died in a boss fight could fall through the world after the boss fell. Now the player stands up at the last place where the player stood on the ground.
- Fixed a bug where a player could fall under the world and keep falling. Now the game moves the player back to the last place where the player stood on the ground.
- Fixed a bug where the boss fight did not reset for the host when the last friend in the fight died just after the host left a loading screen. Now the game reloads the area for the host as soon as the host stands in the world.
- Fixed a bug where a guest saw no Glintstone Whetblade on the ground while the host saw the Glintstone Whetblade. Now when a friend picks up a key item that the game hides from a player, that player gets the key item.
- Fixed a bug where a player left the session when the player chose to quit and the game did not quit. Now a player leaves the session only when the game of that player goes back to the title menu.
- Fixed a bug where a player who died while a friend was alive got a loading screen in some areas and in the open world. Now the player stands up with no loading screen at the same place where a loading screen would put the player.
- Fixed a bug where a player who stood up with no loading screen was invisible and could not move or die again until the next loading screen. Now the player shows again after the stand up, and the next death works.
- Fixed a bug where an NPC could stay at another step of a quest for a guest after a loading screen. Now the game of the guest takes the quest step of each NPC from the host when the loading screen ends.

### Other

- Improved items from the party during a loading screen. The game now gives the item after the loading screen ends.
- Improved the game near some NPCs such as Gatekeeper Gostoc in Stormveil Castle. The game now sends far fewer messages between the players while the party stands near those NPCs.

### Known issues

- When a player uses a red sign that leads into the world of an NPC during a session, the game refuses the red sign. Workaround: leave the session, then use the red sign.
- An NPC invader still makes enemies a little stronger while the NPC invader is in the world of the host.
- When the body of a player does not come back after the player stands up with no loading screen, the game reloads the area for that player. Workaround: turn the setting Stand up with no loading screen off.
- The column of light over a friend is hard to see from far away. The column of light and the path to a friend are not see through yet.
- A guest can still lose the session when every player rests at a grace. The guest then joins the host again and arrives next to the host.
- After a guest loses the session at a grace, the grace menu of that guest can show no Level Up. When a guest sees no Level Up at a grace, the guest sends a bug report.
- Some NPCs can be missing in the world for a guest. When a guest does not see an NPC that the host sees, both players send a bug report.
- A guest can get a lower frame rate after 30 minutes or more in a session. When the frame rate of a guest drops, the guest sends a bug report.
- A player who rides Torrent can still jump between two places on the screens of the other players. When a player sees a friend on Torrent jump between two places, both players send a bug report.
- When a friend joins or leaves during a boss fight, the boss keeps the health that the boss had when the fight started.
- A player who joins a session after a friend heard an NPC line does not hear the full line from that NPC.
- When a save takes more than 10 seconds as a player closes the game, the game can still crash while the game closes.
- When a player stands up at a grace and walks back into some boss fights, the game can reload the area for that player when the other players in the fight die.
- When an enemy drops an item only once, only the player who picks up the item gets the item. Workaround: every player picks up the item from the enemy.
- Some chests can keep their item for the player who opens the chest. Workaround: every player opens the chest.
- A chest that another player already opened can stay closed for the rest of the party. When a player opens that chest, the chest is empty.

## v0.0.27

November 22, 2026. All players must update.

This update adds a path to a friend, a fight view for players who die in a boss fight, messages about friends, missed NPC lines for the whole party, settings for enemy scaling, and a settings page in the launcher and in the game.

### New features

- Added a path to a friend. The game draws an orange band on the ground from the player to one friend. The band goes around walls and down stairs.
- Added a path toward a friend who is far away. The orange band leads to the edge of the land that the game has loaded in the direction of that friend.
- Added a column of light over each friend. A player can see where a friend stands from far away.
- Added the setting Pillars over friends. A player turns the columns of light on or off with the setting Pillars over friends.
- Added settings for enemy scaling. The host picks how much more health, damage and posture enemies get for each extra player. The host picks the health, damage and posture of bosses in separate settings. The host also picks how many more items the party finds for each extra player.
- Added the scaling settings of the host to the settings page of each guest. During a session, a guest sees the values that the host picked. A guest cannot change the values that the host picked.
- Added a PATH row to the Multiplayer page of the pause menu. A player picks a friend with that row. A player also turns the path off with that row.
- Added a Settings link to the launcher under the What's new link. The Settings link opens the settings page of the launcher.
- Added a SETTINGS row to the MULTIPLAYER menu of the main menu and to the Multiplayer page of the pause menu. The SETTINGS row opens a settings page. A player changes the settings with a controller during a session.
- Added three settings. Bug report detail sets how much the game writes for a bug report. Stutter fix turns the stutter fix on or off at the next start of the game. Path to friends turns the path to a friend on or off.
- Added the file settings.yaml to the EldenCoop folder of the game. The file settings.yaml holds the settings that a player changed. A player can open the file settings.yaml with Notepad from the settings page of the launcher.
- Added a Bug report link to the launcher. A player picks how many runs of the game the bug report holds. The launcher shows the size of each bug report in MB.
- Added a fight view for players who die in a boss fight. When a player dies in a boss fight and another player still fights the boss, the player who died watches the other players. The player who died comes back when the boss falls, when the whole party dies, or when a player rests at a grace.
- Added the Steam keyboard for naming a world with a controller. In Big Picture and on Steam Deck, a player types the name of a world on the screen.
- Added buttons to the fight view. A player who watches presses RB or F6 to watch the next player. A player who watches presses LB or F5 to watch the previous player. A player who watches presses X or F7 twice to stop watching and go back to the last grace.
- Added a message when a friend talks to an NPC. The message names the friend and the NPC. The game shows the message for the same friend and the same NPC at most once in 5 minutes.
- Added a message when the party moves a quest forward. The message names the NPC of the last talk. The game shows at most one quest message each minute.
- Added a message when a friend dies. The message names the friend.
- Added a message when a friend leaves the world. The message names the friend.
- Added a message when a friend lights a grace. The message names the friend and the grace.
- Added a message when a friend travels to a grace. The message names the friend and the grace.
- Added a message when a friend does not have Shadow of the Erdtree. The message says that the friend cannot enter the Land of Shadow.
- Added the level, the ping and the number of deaths of each friend under the GO TO row of that friend on the Multiplayer page of the pause menu.
- Added the setting Party messages. A player turns off the messages about friends with the setting Party messages.
- Added missed NPC lines. When one player hears an NPC say a quest line, the quest moves on for the whole party. When another player talks to that NPC later, the NPC says the full line to that player once. The game keeps the missed NPC lines of each character after the player leaves the session.

### Changes

- Changed the settings file. The game no longer reads the file elden_coop.ini. A player who turned the stutter fix off in elden_coop.ini turns the Stutter fix off again on the settings page.
- Changed the Save a diagnostic report button of the launcher. The Save a diagnostic report button now opens the same choice as the Bug report link.
- Changed the bug report. A bug report now also holds the file settings.yaml.
- Changed the Uninstall link. The Uninstall link now keeps the file settings.yaml.
- Changed the map so that the icon of each friend is 1.5 times as large. The map now shows the name of each friend in light blue under the icon of that friend.
- Changed how the party finds items. Each friend in the party now raises the item discovery of every player by 100 percent. The host can change the item discovery for each friend on the settings page.
- Changed the STUTTER FIX row of the settings page in the game. The row now says AT NEXT START after a player changes the stutter fix.
- Changed what happens when a player dies far from a Stake of Marika outside a boss fight while another player in the party is alive. The player stands up at the last grace with no loading screen when the last grace is in the same part of the map.
- Changed what happens when a player dies in a boss fight and the boss falls. The player stands up where the player fell, with full health.
- Changed what happens when a player quits to the title. The other players now see at once that the player left.
- Changed the box where a player types the name of a world. The game now keeps running while the box is open.
- Changed the Data Analysis question at the start of the game. A player now answers the Data Analysis question as in the base game.
- Changed the log files. The game now keeps the log files of the last 10 runs. The choice Every run of the Bug report link now holds the last 10 runs.
- Changed resting at a grace. When a player rests at a grace, the game now always refills the items of that player from the party chest.
- Changed GO TO for a player without Shadow of the Erdtree. A player without Shadow of the Erdtree cannot travel to a friend in the Land of Shadow. The game shows a message that says why.

### Bug fixes

- Fixed a bug where normal enemies kept the health of a solo game in a party. Now enemies get more health for each extra player.
- Fixed a bug where the map and the compass showed a friend in the wrong place while the friend rode Torrent. Now the map and the compass show each friend at the place that the friend's own game reports.
- Fixed a bug where a player who rode Torrent showed up far away on the screens of the other players. Now the game shows that player at the right place within two seconds after the player gets on Torrent.
- Fixed a bug where the spirit summon of another player could stand far from that player. Now the game shows the spirit summon next to that player.
- Fixed a bug where a player flickered between two places on the screens of the other players after the player got off Torrent. Now the game shows that player in one place.
- Fixed a bug where a player who rode Torrent showed up on foot on the screen of another player after a load. Now the game puts that player back on Torrent within two seconds.
- Fixed a bug where a player who got on Torrent was pulled off Torrent on the screen of another player. Now the game shows that player on Torrent from the moment the player gets on.
- Fixed a bug where a player could not offer a bell bearing to the Twin Maiden Husks after a friend had offered the same bell bearing. Now each player offers his own bell bearing to the Twin Maiden Husks. After the offer, the Twin Maiden Husks sell the new items to the player who offered the bell bearing.
- Fixed a bug where a boss fight ended at once when the clock of the host's PC changed. Now a boss fight ends only when the party wins, when the party dies or when the party walks away from the boss.
- Fixed a bug where the last player to rest at a grace saw two black screens. Now the last player to rest at a grace sees one black screen, like a rest in the base game.
- Fixed a bug where some boss fights, such as the fight with Starscourge Radahn, did not end when the party defeated the boss. Now the boss fight ends when the party defeats the boss.
- Fixed a bug where a boss fight with two bosses ended when the first boss fell. Now the boss fight starts over for the party when the second boss defeats every player who fought.
- Fixed a bug where the boss started over for the other players when the host died far from a Stake of Marika in a boss fight. Now the host watches the fight.
- Fixed a bug where a player who died in a boss fight got two loading screens. Now the player who died gets one loading screen when the whole party dies.
- Fixed a bug where a player who died in a boss fight got a loading screen when the boss fell right after that death. Now that player watches the fight and stands up where the player fell.
- Fixed a bug where a player who used GO TO and then died came back at a grace far away from the party. Now the player comes back at the grace closest to the place where GO TO took the player. The game picks only a grace that the player found before.
- Fixed a bug where the guests lost the session when the host died and the loading screen came late. Now the guests stay in the session while the host loads after a death.
- Fixed a bug where a guest still played as a guest in his own world after he left the host's world. Now a guest who goes home plays his own world again.
- Fixed a bug where a player who stood up at a grace stayed invisible to the other players. Now the other players see that player at once.
- Fixed a bug where the game could crash when a player closed the game. Now the game finishes saving and then closes at once.
- Fixed a bug where a player got Baldachin's Blessing twice when a friend got Baldachin's Blessing at the same time. Now a player gets the Baldachin's Blessing of a friend only when the game of that player gave no Baldachin's Blessing.
- Fixed a bug where a guest who joined later did not get a boss item that the host got before friends could join. Now the game records every boss item that the host gets in that world. A guest who joins later gets each of those boss items.
- Fixed a bug where a player could lose part of a purchase when the inventory was full. Now a merchant sells a player only as many items as the inventory holds.
- Fixed a bug where a door that one player opened with a key could stay shut for the other players after a loading screen. Now a door that one player opens with a key stays open for the whole party.
- Fixed a bug where a player found no map fragment at a spot where a friend had found the map fragment. Now every player in the party gets the map fragment when one player finds it.
- Fixed a bug where some NPCs outside Limgrave reacted to a player who stood far away. Now each NPC in every area reacts to the player who stands near that NPC.
- Fixed a bug where the Talk to Ranni choice at a grace appeared and disappeared while a friend walked near Ranni. Now each player sees the Talk to Ranni choice only when that player stands near Ranni.

### Other

- Improved how the game saves the character of a guest. The character of a guest now always loads as a main player.

### Known issues

- When the last player rests at a grace, every player who already rests at that grace sees one short black screen over the grace menu.
- When a player dies far from a Stake of Marika and the last grace is in another part of the map, the game still reloads the area for that player.
- When a player stands up at a grace inside a boss fight and the boss bar does not show again, the game can reload the area for that player when the other players in the fight die.
- When the host dies in a boss fight, the boss fight can start over for the other players while the host watches the fight.
- Some field bosses do not end the fight view when they fall. Workaround: Press X or F7 twice.
- When an NPC dies or leaves the area, the NPC does not say a missed line again.
- Some NPCs say only the short line to a player who missed the full line.

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
- When one player finds a map fragment, the other players find no map fragment at that spot. The map is already open for them. Fixed in v0.0.27.
- The first time a guest joins a world after this update, the guest gets the items of that world once more.
- When a player stands up at a Stake of Marika inside a boss fight and the boss bar does not show again, the game can reload the area for that player when the other players in the fight die.
- When a player dies in a boss fight and walks back before the rest of the party dies, that player gets a second loading screen.
- When the host or a guest plays v0.0.25 or an older version, the guest sees no message about the other version.
- Outside Limgrave, some NPCs may not share talks and quest progress with the whole party. Fixed in v0.0.27.

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
- Outside Limgrave, some NPCs may not share talks and quest progress with the whole party. Fixed in v0.0.27.

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
- Outside Limgrave, some NPCs may not share talks and quest progress with the whole party. Fixed in v0.0.27.

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
