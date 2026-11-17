# Changelog

## 0.6.4
New:
- Works on the 2026-11-17 game update, and keeps working on the 2026-10-29 update. On the 2026-11-17 update 0.6.1 turns Weekly Strategy, the spring game, the spring game kits and the runtime merge off; 0.6.4 knows that game build.
- A new mod file, `Dynasty-Extensions-0.6.4.fbmod`, for the 2026-11-17 update: the same screens as the 0.5.0 file, rebuilt for the update's game data. Remove `Dynasty-Extensions-0.5.0` from the Mod Manager and import it. A game still at the 2026-10-29 update keeps the 0.5.0 file (in the zip, in `For the 2026-10-29 game update`).
- The spring game kit fix of 0.6.3 (below), which was not released on its own. The kits work on the 2026-11-17 and 2026-10-29 updates.
Unchanged: the runtime merge, Instant Replay while you watch a CPU game, Spring Game, Spring Practice, Weekly Strategy, practice drills and Press Box work as in 0.6.1, with the same supported setups. Your ini is kept.
Files: a new mod file, `wsdata.dll`, `demerge.dll`, `anygame.dll`, `DynastyExtensionsPlugin.dll`, its `README.txt` and `dynasty-extensions.ini` (text only: which game updates). `de-expr.pack` is 0.6.1's.

## 0.6.3 (not released on its own; part of 0.6.4)
Fixed:
- Spring game kits work. The kit swap added in 0.6.1 did not work on the field: the stand-in kept its own FCS kit and only your side changed, to your school's dark kit. Now the stand-in (your second string, at home) wears your school's white kit and your starters its dark kit, on team select and on the field. The scorebug keeps the stand-in's name and logo. Every other game is unchanged.
- The 2026-10-29 title update (from 0.6.4 also the 2026-11-17 update). On the 2026-10-13 update the spring game kits stay stock.
New settings: `spring_kits_teamrow` (1) and `spring_kits_teamrow_dry` (0) under the test switches in `[Weekly Strategy]`; they are part of the kits, leave them as they are. An older ini gets them from the plugin. `spring_kits = 1` is the default, as in 0.6.1; a `spring_kits` line already in your ini is kept.
Unchanged: the main mod is the same file as 0.5.0 to 0.6.1; the runtime merge, Instant Replay while you watch a CPU game, Spring Game, Spring Practice, Weekly Strategy, practice drills and Press Box work as in 0.6.1.
Files: a new `wsdata.dll`, `DynastyExtensionsPlugin.dll` and `dynasty-extensions.ini`. `demerge.dll`, `de-expr.pack`, `anygame.dll` and the main mod are 0.6.1's.
0.6.2 was not released.

## 0.6.1
New:
- Spring game kits: in the spring game your second string (the stand-in team) wears your school's away kit and your starters your home kit, so it looks like an intrasquad scrimmage. The scorebug still shows the stand-in's name and logo. Every other game is unchanged. New setting `spring_kits` in `[Weekly Strategy]` (1 = on, the default; 0 = off); an older ini gets it from the plugin.
Unchanged: the main mod is the same file as 0.5.0, 0.5.1 and 0.6.0; the runtime merge, Instant Replay while you watch a CPU game, Spring Game, Spring Practice, Weekly Strategy, practice drills and Press Box work as in 0.6.0.
Files: a new `wsdata.dll`, `DynastyExtensionsPlugin.dll` and `dynasty-extensions.ini`. `demerge.dll`, `de-expr.pack`, `anygame.dll` and the main mod are 0.6.0's.
Checked in game: the spring game kits on the game alone (the stand-in in the school's away kit, the user in its home kit). Correction (0.6.3): this check was wrong; the kits did not work on the field until 0.6.3.

## 0.6.0
New:
- Dynasty Extensions fits other dynasty mods while the game runs, without a ready-made fit for each version. A new version of Playoff Customizer, Dynasty Customizer or the AIO dynasty mod no longer has to wait for a Dynasty Extensions update. If a file can't be fitted safely, Dynasty Extensions turns itself Off for that session and `dynasty-extensions-merge.txt` says why.
Changed:
- The plugin's helper (`demerge.dll`) and its data file (`de-expr.pack`) are new. The data file no longer lists individual versions of other mods.
- For the game alone and DRI+ 3.0 the merged result is the same as in 0.5.x.
Unchanged: the main mod is the same file as 0.5.0 and 0.5.1; Instant Replay while you watch a CPU game, Spring Game, Spring Practice, Weekly Strategy, practice drills and Press Box work as in 0.5.1.
Files: new `demerge.dll` and `de-expr.pack`. The plugin, `anygame.dll`, `wsdata.dll`, `dynasty-extensions.ini` and the main mod are 0.5.1's.
Checked in game: the game alone (same result as 0.5.0), DRI+ 3.0, Playoff Customizer 1.3.0 (preseason and week 9 into 10), Dynasty Customizer 1.1.0, the AIO dynasty mod 1.4.1 and the ZEO + Playoff Customizer + DRI combined download.

## 0.5.1
New:
- Press Box: Instant Replay in the pause menu while you watch a CPU game (after the whistle or before the snap, never during a play), the same as in a game you play. Your own games are not changed. New setting `watch_replay` in `[Press Box]` (1 = on, the default; 0 = off); an older ini gets it from the plugin.
Changed:
- The separate Press Box mod is retired: Dynasty Extensions has everything it had. See INSTALL.md, "Coming from the separate Press Box mod".
Unchanged: the main mod is the same file as 0.5.0; Spring Game, Spring Practice, Weekly Strategy, practice drills and Press Box work as in 0.5.0.
Files: a new `DynastyExtensionsPlugin.dll`, `anygame.dll` and `dynasty-extensions.ini`. `demerge.dll`, `de-expr.pack`, `wsdata.dll` and the main mod are 0.5.0's.

## 0.5.0
New:
- No patch files. The game alone, DRI+ 3.0, Playoff Customizer 1.3.0, Dynasty Customizer 1.1.0 and the AIO dynasty mod 1.4.1 all work with the one download. The Dynasty Extensions rows, screens and logic are added while the game runs, on top of whatever the game or another mod loaded.
- League Settings rows (Spring Game, Weekly Strategy, Press Box) are added while the game runs. Other mods' own rows, such as Playoff Customizer's bracket and sites rows, stay where they are.
- The Weekly Strategy View button and the Press Box popup work on Playoff Customizer, Dynasty Customizer and the AIO dynasty mod with no extra file.
- Fixed: two "Take this game" picks in one week. Each Play Game card now opens its own game (before, the second card could open the first game's teams).
- Dynasty Extensions' requests stay out of the dynasty hub's card list on every base (they used to show as cards on some setups).
Changed:
- The Compatibility patches folder is gone. If you have a "Dynasty Extensions x ..." patch, remove it.
- The main mod no longer replaces League Settings, so it can sit anywhere in your Mod Manager list.
- The plugin is new: replace your Plugins folder (keep a copy of your dynasty-extensions.ini first).
- Conference Customizer and older versions of Playoff Customizer, Dynasty Customizer and the AIO dynasty mod are not supported. Dynasty Extensions may read Off with them (safe, and the merge file says why).
- Only want Press Box? Set Spring Game and Weekly Strategy to Off in League Settings (once per dynasty).
Unchanged: Spring Game, Spring Practice, Weekly Strategy, practice drills and Press Box work as in 0.4.0.

## 0.4.0
New:
- Dynasty Extensions works with other mods that change the dynasty logic without a copy of that logic in its own file. A helper in the plugin adds it while the game runs, each time you load a dynasty, on top of whatever the game or another mod loaded.
- DRI+ 3.0 works with Dynasty Extensions with no patch.
- Conference Customizer 1.0.2 needs only a small screens patch.
- dynasty-extensions-merge.txt (in Plugins\DynastyExtensions) says in one line whether Dynasty Extensions is ON this session, and why not if it is OFF.
- When Dynasty Extensions can't run in a session, the Spring Game, Weekly Strategy and Press Box rows read "Off this session", and the Weekly Strategy View button and "Take this game" are not shown, so nothing can be pressed that needs the missing logic.
Changed:
- The plugin is now required, and it is new: replace your old Plugins folder (keep a copy of your dynasty-extensions.ini first).
- With Playoff Customizer 1.1.0 (no patch for it) Dynasty Extensions stays off and says so; your dynasty is not affected.
Unchanged: Spring Game, Spring Practice, Weekly Strategy, practice drills and Press Box work as in 0.3.0. The Playoff Customizer 1.3.0, Dynasty Customizer 1.1.0 and AIO dynasty mod patches carry the same content as the 0.3.0 patches.

## 0.3.0
New:
- Practice drills in your dynasty: on Weekly Strategy's Team Profile, START TRAINING opens Road to Glory's practice drill menu (Team drills and Skill drills for your drill player's position). The drill player is your first filled focus player; X on a filled focus card picks another one (his drills load the next time you open Weekly Strategy). He is the one on the field in the drill; your real depth chart is never changed.
- Drill XP: bronze +100, silver +250, gold +500, once per player per week (replaying only tops up to a better medal). `drill_xp_pct` in the ini scales it (50 = these numbers, 100 = the full Road to Glory table, 0 = none). A drill does not count as the week's practice plan.

Everything else is the same as 0.2.3. The plugin is new (replace yours; keep your ini and put it back, the new drill settings are added on their own). The compatibility patches are unchanged: keep your 0.2.3 patch or use the 0.3.0 one.

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
- Spring game attendance is now really half the stadium (12,483 at JMU). In 0.1.6 the setting had no effect: the game worked the crowd out again at kickoff. The game seats fans sideline first, so the empty seats show mostly in the end zones and the sideline stands still look full.
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
