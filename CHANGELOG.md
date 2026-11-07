# Changelog

## 0.1.9
New:
- Spring Situations (beta, off unless you pick it): a fifth Spring Game choice in League Settings, **Game + Practice + Situations**. You still play the spring game
  (your starters against your second string) and get the practice XP, but the game is set up as five situations: a two-minute drill before the half (the game starts there, no coin
  toss and no kickoff), a red-zone stand, 3rd and medium, backed up at your own 2, and protecting a 3-point lead late. Each one gets a letter from A to F,
  and at the next Advance the letters scale the spring game XP for your starting offense and defense (A = 125 %, F = 60 %). A situation the game ended
  before you reached it counts as a C (normal XP); kickers, punters and the second string get the normal XP.
- Pick it while you are on Preseason Week 0, before the Advance into the spring week (the extra preseason week). If you change it once the spring week has
  started, it waits until next year. In a brand-new dynasty the rows are greyed out until the first Advance, so the first spring game can't use it.
- With Dynasty Midgame Save 0.2.4 or later installed, Midgame Save runs the start of the spring game. With an older Midgame Save, Spring Situations
  switch themselves off for that game (normal spring game, normal XP).
- Works with every compatibility patch, with no extra save row.

Known:
- On downs 1 to 3 the CPU defense doesn't use its situation plays, so a two-minute drill or red-zone stand may feel less realistic.

Also in this release: 0.1.8.2's fix (a NEW dynasty with the AIO dynasty mod 1.4.0 or 1.4.1 and its patch could crash at the coach contract screen).
The default Spring Game choice is still Game + Practice.

Updating from 0.1.8.2, 0.1.8.1 or earlier:
- Replace the main mod (`Dynasty-Extensions-0.1.9.fbmod`), the plugin (the `Plugins` folder from `Manual install`) AND your ONE patch: every patch is
  new in 0.1.9 (they carry the new Spring Game choice). If you edited `Plugins\DynastyExtensions\dynasty-extensions.ini`, copy it somewhere safe first, copy the new `Plugins` folder over the old one, then put your ini back; the new setting uses its default.

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
- Spring game attendance is now really half the stadium (12,483 at JMU). In 0.1.6 the setting had no effect: the game worked the crowd out again at kickoff. The game seats fans sideline first, so the empty seats show mostly in the end zones and the sideline stands still look full. Support for the spring game type in the Dynamic Gameday Atmosphere mod could show a properly thinner crowd later.
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
