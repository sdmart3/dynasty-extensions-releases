# Changelog

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
