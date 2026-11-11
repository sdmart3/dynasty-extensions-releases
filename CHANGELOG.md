# Changelog

## 0.2.3
Fixed:
- Spring game in leagues where a mod replaced the five stock FCS teams: your second string plays as one of your real FCS schools, which is put back exactly after the spring.
- Spring restore fixed on saves with lots of other mods' data (the stand-in school is now put back even when the save carries many other mods' rows).
- Uninstall-crash fix: removing Dynasty Extensions no longer crashes saves at a stage end. Old entries are converted at your first Advance after updating.

Before you remove it: update to 0.2.3 and Advance once; after that it is safe to remove. If a save already crashes after removing an older version: turn Dynasty Extensions back on, load the save, Advance once, then remove it.

Updating from 0.2.0: replace the main mod (`Dynasty-Extensions-0.2.3.fbmod`) and your ONE patch (every patch is new in 0.2.3), then Advance once. The plugin is unchanged since 0.2.0. From anything older, replace the plugin too.

Compatibility patches (separate downloads): every patch is also attached to this release on its own, with a `.sha256.txt` file. Use only the ONE patch for your base mod and put it at the very bottom of the Mod Manager list.

## 0.2.0
New:
- Spring Practice (beta, off unless you pick it): a fifth Spring Game choice in League Settings. The preseason gets four extra weeks instead of one.
  Weeks 1 to 3 are practice weeks, each with a drill game on the hub (your starters against your second string) that plays five set situations: a
  two-minute drill before the half (the game starts there, no coin toss and no kickoff), a red-zone stand, 3rd and medium, backed up at your own 2, and
  protecting a 3-point lead late. Each situation gets a letter from A to F. Week 4 is the normal spring game (kickoff, full game, normal XP).
- Practice XP is the same four weeks' worth as Game + Practice, paid one week at a time (all C = the same total). Weeks 2 to 4 are scaled for your starting offense and defense by the
  drill game of the week before (A 125 %, B 110 %, C 100 %, D 80 %, F 60 %; offense = S1 / S3 / S4, defense = S2 / S5). A situation the game ended before you reached it, or a drill game you skip, counts as a C (normal XP).
  Kickers, punters and the second string get the normal XP.
- The drill grades show on the scorebug as they happen (the down-and-distance box), tested with the stock scorebug and CFB on CN (other scorebug mods show it if they use the game's down-and-distance text). Off with
  `spring_hud_grades = 0` in the ini.
- Each extra week moves the season one week later, so with Spring Practice the national title game is in February.
- Pick it while you are on Preseason Week 0. A change made once the extra weeks have started waits until next year. In a brand-new dynasty the rows are
  greyed out until the first Advance, so the first season can't use it.
- Dynasty Midgame Save: you don't need it. If you already use it, update it to 0.2.4 so the two work together (Midgame Save then starts each drill game).
  With an older Midgame Save the drill game plays as a normal game (no situations, normal practice XP that week).
- Every compatibility patch carries it, with no extra save row (played through in testing with Playoff Customizer; the others are built the same way).

Known:
- On 1st to 3rd down the CPU defense calls ordinary plays instead of situation plays, so a two-minute drill or red-zone stand can feel a bit easier.
- Your starters play every drill game: they take wear (healed after each week) and can get hurt.

The default Spring Game choice is still Game + Practice, and Off / Game Only / Game + Practice / All Teams Practice work exactly as in 0.1.8.2.

Updating from 0.1.8.2, 0.1.8.1 or earlier:
- Replace the main mod (`Dynasty-Extensions-0.2.0.fbmod`), the plugin (the `Plugins` folder from `Manual install`) AND your ONE patch: every patch is
  new in 0.2.0 (they carry Spring Practice). If you edited `Plugins\DynastyExtensions\dynasty-extensions.ini`, copy it somewhere safe first, copy the new `Plugins` folder over the old one, then put your ini back; the new settings use their defaults.
- If you briefly had 0.1.9 (up for a few hours on 2026-11-07, then taken down): update the same way. Its "Game + Practice + Situations" choice is now Spring Practice.

Compatibility patches (separate downloads): every patch is also attached to this release on its own, with a `.sha256.txt` file. Use only the ONE patch for your base mod and put it at the very bottom of the Mod Manager list.


## 0.1.8.2
Fixed:
- Creating a NEW dynasty with the AIO dynasty mod (1.4.0 or 1.4.1) and its Dynasty Extensions patch could crash at the coach contract screen. The AIO mod's own code looks at a field on every open request when that screen finishes, and 41 of its own settings requests carry a record that does not have that field; the game sometimes read past the end of that record and crashed. The two AIO 1.4.x patches now skip that look for those requests. Only those two patches changed.
- Existing dynasties were not affected, and the AIO dynasty mod alone is not changed by this.

Updating from 0.1.8.1:
- AIO dynasty mod 1.4.0 or 1.4.1: replace ONLY your AIO patch (remove the old Dynasty Extensions x AIO patch, import the new one, keep it at the very bottom of the list). Nothing else changes.
- Everyone else: nothing to do. The main mod (still `Dynasty-Extensions-0.1.8.1.fbmod`), the plugin and the other four patches are the same as 0.1.8.1's.

Compatibility patches (separate downloads): every patch is also attached to this release on its own, with a `.sha256.txt` file. Use only the ONE patch for your base mod and put it at the very bottom of the Mod Manager list.

## 0.1.8.1
Fixed:
- Weekly Strategy said "Bye week: no opponent" (and Team Profile "No game this week") in a week with a game, with Playoff Customizer,
  Dynasty Customizer or the AIO dynasty mod. Those mods keep their settings in hidden requests, and some of them are a kind the game
  treats as "do this first". While one is open, the list Weekly Strategy read held only those, so your game was missing from it.
  Weekly Strategy now reads the game list the controller screen uses. It works on your existing dynasty too; you don't need a new one.
- Press Box: your own HOME game could sit on READY forever on the controller screen when a keyboard or a second controller was
  connected. The screen gave that one the other team and waited for it to ready up too. Your home games now use the game's own
  screen: your controller starts on your team, and you can still move it to the opponent (to play them) or to the middle (to watch).
  If you are stuck on READY with an older version, press B to back out.
- The install guide now says which way round the load order goes in the Mod Manager list: base mod at the TOP, Dynasty Extensions
  under it, the patch at the very BOTTOM.

Updating from 0.1.8:
- Replace the main mod and the plugin (the `Plugins` folder from `Manual install`). The compatibility patches are the same as 0.1.8's;
  keep yours. If you kept your own `dynasty-extensions.ini`, keep it: the new `ctrl_select_stock_screen = 1` is applied for you. If you
  added `ctrl_select_stock_screen = 0` yourself, change it to 1 or delete the line.

Compatibility patches (separate downloads): the patches are the same as 0.1.8's. Every patch is also attached to this release on its own, with a `.sha256.txt` file. Use only the ONE patch for your base mod and put it at the very bottom of the Mod Manager list.

## 0.1.8
Fixed:
- Press Box: watching a game after taking control of the opponent could crash. Fixed.
- No longer conflicts with mods that change the controller/options menu file. Dynasty Extensions doesn't replace that file any more, so it works alongside such mods with no patch. The AIO Broadcast mod, for example, works next to it as it is: its settings (the scorebug included) work, and you can take a game and watch it.

New:
- Compatibility patch for the AIO dynasty mod 1.4.1 (it was a separate download for 0.1.7; it is in the zip now). The patches for the other base mods are rebuilt for 0.1.8.

Updating from 0.1.7, 0.1.6 or 0.1.4:
- Replace the main mod, your ONE patch AND the plugin (the `Plugins` folder from `Manual install`). If you changed `dynasty-extensions.ini`,
  keep your copy: your choices stay, and the new options get their default values automatically.

## 0.1.7
Fixed:
- Spring game attendance is now really half the stadium (12,483 at JMU). In 0.1.6 the setting had no effect: the game worked the crowd out again at kickoff. The game seats fans sideline first, so the empty seats show mostly in the end zones and the sideline stands still look full. I'll be chatting with Ace about having the spring game type supported in his Dynamic Gameday Atmosphere mod, which would show a properly thinner crowd.
- Press Box: with two or more game cards on your hub, each card now opens its own game. After you had watched a game, another card could open the wrong one.
- Press Box: watching a game no longer fails to start when another plugin in your game also changes the controller setup. If one is in the way, `anygame.log` names it.

Updating from 0.1.6 or 0.1.4:
- Replace the main mod, your ONE patch AND the plugin (the `Plugins` folder from `Manual install`). If you changed `dynasty-extensions.ini`,
  keep your copy: your choices stay, and the new options get their default values automatically.

## 0.1.6
New:
- Weekly Strategy shares your weekly gameplan focus with Call Sheet 0.14.1 or later, so Call Sheet's suggestions follow it. Nothing to set up.
- More Weekly Strategy focus players: 3 to start, plus 1 for each position Whisperer talent your HEAD COACH owns, up to 6.
  The Whisperers are in the Talent Developer tree in Upgrade Coach Skills: QB, RB, WR/TE, OL, DL, LB and DB Whisperer (30 points each)
  and K/P Whisperer (15 points). They keep their normal effect too (freshmen and sophomores at that position progress faster).
  The extra players get focus XP and the weekly goal bonus like the first three.
- The spring game crowd is now about half the stadium.
- New patch for the AIO dynasty mod 1.4.0. The AIO 1.3.1 patch is still included: pick the one that matches your AIO version.

Fixed:
- Creating a NEW dynasty crashed with Dynasty Customizer, Playoff Customizer or the AIO dynasty mod plus its Dynasty Extensions patch.

Updating from 0.1.4:
- Replace the main mod, your ONE patch AND the plugin (the `Plugins` folder from `Manual install`). If you changed `dynasty-extensions.ini`,
  keep your copy: your choices stay, and the new options get their default values automatically.

## 0.1.4
First release. Press Box 0.7.1, Weekly Strategy and Preseason Weeks (the spring game) in one mod.
- League Settings rows: Spring Game (Off / Game Only / Game + Practice / All Teams Practice), Weekly Strategy (On / Off), Press Box (On / Off).
- One plugin (DynastyExtensionsPlugin.dll) and one settings file (dynasty-extensions.ini).
- Patches for Conference Customizer 1.0.2, Playoff Customizer 1.3.0, Dynasty Customizer 1.1.0 and AIO dynasty mod 1.3.1. With the last
  three, the three rows sit on that mod's own League Settings screen, right after Quarter Length. The two On / Off switches share a row
  the Spring Game already uses, so a 64-team playoff field still fits (147 of the 150 save rows).
- The spring game comes back every season, including with Playoff Customizer.
