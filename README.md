# Dynasty Extensions

**Download:** https://github.com/sdmart3/dynasty-extensions-releases/releases/latest (the zip has the mod, the plugin and the install steps).

Three dynasty add-ons in one mod: Press Box, Weekly Strategy and Preseason Weeks (the spring game).

**New in 0.6.4: works on the 2026-11-17 game update.** That update switched off Weekly Strategy, the spring game, the spring game kits and the runtime merge of 0.6.1, and the old mod file no longer fits it. 0.6.4 works on the 2026-11-17 update and keeps working on the 2026-10-29 update. It also brings the spring game kits that work (your second string in your school's white kit, your starters in its dark kit). **Import the new mod file** `Dynasty-Extensions-0.6.4.fbmod` and copy the new Plugins folder (see "What's new in 0.6.4").

**0.6.0: it keeps working when the other mods update.** Dynasty Extensions now fits itself to the dynasty files of Playoff Customizer, Dynasty Customizer and the AIO dynasty mod while the game runs, instead of waiting for a Dynasty Extensions update for each new version. If a version is too different, it turns itself Off safely and says why (see "Is it on?"). Nothing to relearn: same mod file, and updating is just replacing the Plugins folder.

**0.5.1: Instant Replay while you watch a CPU game.** Press Box now offers Instant Replay in the pause menu of a game you watch, the same as in a game you play. With this, the separate Press Box mod is retired.

**No patch files (since 0.5.0).** Before, if you ran Playoff Customizer, Dynasty Customizer or the AIO dynasty mod, you had to find and import a second file made for your exact version. Now one download covers the game alone, DRI+ 3.0, Playoff Customizer 1.3.0, Dynasty Customizer 1.1.0 and the AIO dynasty mod 1.4.1 (the table below lists what was checked). Import the mod, copy the Plugins folder, done.

## Install in 3 steps

Extract the zip first. You import the `.fbmod` in the Mod Manager, not the zip. Back up your dynasty save before you try it.

1. Close the game and the Mod Manager. Copy the `Plugins` folder from `Manual install` into your Mod Manager folder (next to `MMCModManager.exe`). **The plugin is required**: without it nothing of Dynasty Extensions runs.
2. Open the Mod Manager, import `Dynasty-Extensions-0.6.4.fbmod` and turn it on. Put it anywhere in the list. (Game still at the 2026-10-29 update? Import `For the 2026-10-29 game update\Dynasty-Extensions-0.5.0.fbmod` instead.)
3. Launch the game from the Mod Manager and load your dynasty. About 30 seconds after the game starts the plugin's helper is in. (The Mod Manager loads plugins only when it starts. If it was already open when you copied the `Plugins` folder, close it and start it again first.)

Then open `Plugins\DynastyExtensions\dynasty-extensions-merge.txt`: its first line says `Dynasty Extensions is ON`. If it says `ready`, go back to the main menu and load the dynasty again. If it says `OFF this session because ...`, see "Is it on?" below.

Updating from 0.4.0 or older: see INSTALL.md. **Remove any "Dynasty Extensions x ..." patch you have.** You don't need it any more.

## Which mods work with it

No patch for any of them. "In game" means it was run in a dynasty and checked. "Off" means Dynasty Extensions turns itself off safely and says so. The checks below were made on the 2026-10-29 game update. On the 2026-11-17 update the game alone is checked in game; the other mods need their own versions for that update from their authors.

| You also use | Result | Checked |
|---|---|---|
| Nothing (the game alone) | works | in game |
| DRI+ 3.0 | works | in game |
| Playoff Customizer 1.3.0 | works (preseason, and week 9 into 10; the bracket still shows) | in game |
| Dynasty Customizer 1.1.0 | works | in game (preseason) |
| AIO dynasty mod 1.4.1 | works (in a dynasty you already had) | in game (preseason) |
| ZEO 1.0.1 + Playoff Customizer 1.3.0 + DRI 3.0 (the combined download) | works (DRI+ starts as normal) | in game (mid-season, one Advance) |
| Conference Customizer, or an older version of the mods above | not supported: it may read Off | not tested |
| Any other mod that changes the dynasty logic | not supported: Off | by design |

When it is Off, the three League Settings rows read **Off this session**, nothing that needs Dynasty Extensions can be pressed, and your dynasty plays and saves normally.

Only the versions above are supported. They are the ones that were run in a game. A newer version of Playoff Customizer, Dynasty Customizer or the AIO dynasty mod may work too, now without a new Dynasty Extensions download, but it has not been checked: if it does not fit, Dynasty Extensions turns itself Off and says why. DRI+ older than 3.0 is not covered.

## Only want Press Box?

Dynasty Extensions has Press Box in it, and it needs no patch files. Install Dynasty Extensions as above, then open League Settings in each dynasty and set Spring Game to Off and Weekly Strategy to Off. Do it in the preseason: during the season these two rows are locked. You only do this once per dynasty. Using the separate Press Box mod? It is retired: Dynasty Extensions now has its instant-replay fix too. Don't run both. To switch, see INSTALL.md, "Coming from the separate Press Box mod".

## What it does

- **Press Box.** Play or watch any game of the week. Go to EA SPORTS Network > Scores / Schedules, press A on a game and pick
  **Take this game**. It shows up as a card on your hub. On the controller screen, move your controller to a team to play it, or leave it in the middle to watch. You can take more than one game in a week: each Play Game card opens its own game.
- **Weekly Strategy.** Press the **View** button on the dynasty hub (it is not under Practice). You get the Weekly Strategy screen: pick focus players, see this week's
  coach goal and choose a gameplan focus. They give your players XP each week. START TRAINING on Team Profile opens Road to Glory's practice drills for your players (see "Practice drills" below). You start with 3 focus players; each position Whisperer talent your head coach owns
  opens one more, up to 6 (Talent Developer tree in Upgrade Coach Skills: QB, RB, WR/TE, OL, DL, LB, DB and K/P Whisperer). It works with Call Sheet's Weekly Strategy link: your gameplan focus is written to a small
  file that Call Sheet 0.14.1 or later reads, so Call Sheet's suggestions follow it, with nothing to set up.
- **Spring Game.** One extra preseason week with a spring game: your starters against your second string, with attendance set to half the stadium (the empty seats show mostly in the end zones).
  Your players also get four weeks' worth of practice XP before it. Records and stats don't count. Play it from the hub like any other game.
  - **Spring Practice** (beta, off unless you pick it). Four extra preseason weeks instead of one: three practice weeks, each with a drill game
    of five graded situations, then the normal spring game. The grades raise or lower the next week's practice XP. See "Spring Practice" below.
  - **Spring game kits** (working since 0.6.3). In the spring game your second string (the stand-in team, at home) wears your school's white kit and your
    starters wear its dark kit, so it looks like an intrasquad scrimmage. The scorebug still shows the stand-in's name and logo (for example DUKES). Every
    other game is unchanged. The 2026-11-17 and 2026-10-29 title updates; on the 2026-10-13 update the kits stay stock. To turn it off, set `spring_kits = 0` in the
    `[Weekly Strategy]` part of `Plugins\DynastyExtensions\dynasty-extensions.ini`.
## Turning things on and off

Open **League Settings** in your dynasty (the screen is titled Dynasty Settings). Three rows sit right after Quarter Length, under Clock Management:

| Row | Choices |
|---|---|
| Spring Game | Off / Game Only / Game + Practice / All Teams Practice / Spring Practice |
| Weekly Strategy | On / Off |
| Press Box | On / Off |

Spring Game choices:

- **Off**: no extra week.
- **Game Only**: the extra week and the spring game, with game XP. No practice XP.
- **Game + Practice** (default): the same, plus four weeks' worth of practice XP for your team before the game (roughly one to two skill points a player).
- **All Teams Practice**: the same as Game + Practice, and every CPU team gets that practice XP too. CPU teams never play a game.
- **Spring Practice** (beta): four extra weeks on the calendar, three practice weeks with a drill game each and then the spring game (below).

- In a brand-new dynasty these rows are greyed out until your first Advance. Until then everything runs at its default (all on, Game + Practice).
- Weekly Strategy and Press Box change right away. A new Spring Game choice counts from the Advance out of Preseason Week 0: pick it while you are on
  Preseason Week 0. If you change it once the extra weeks have started, this spring finishes the way it started and your new choice starts next year.
- Turning one off leaves the other two alone.

More detail settings (watch pause, the controller screen, which Weekly Strategy panels fill in, the Call Sheet file, the scorebug text, the spring game kits) are in
`Plugins\DynastyExtensions\dynasty-extensions.ini`. You don't need to touch it.


## Is it on?

Open `Plugins\DynastyExtensions\dynasty-extensions-merge.txt` after you load a dynasty. Its first line says `Dynasty Extensions is ON` or `Dynasty Extensions is OFF this session because ...`, and the next line says what to do. When it is ON you do not have to do anything.

When it is OFF, nothing of Dynasty Extensions runs, and nothing that needs it can be pressed: the Spring Game, Weekly Strategy and Press Box rows in League Settings are greyed and read **Off this session**, Scores / Schedules shows the game's own menu (no "Take this game"), and the dynasty hub has no Weekly Strategy View button. Your dynasty is not harmed: you can play, advance and save, and your settings are kept for the next time it is ON.

If you loaded the dynasty before the helper was in (about 30 seconds after the game starts), the file still says "ready": go back to the main menu and load the dynasty again.


## Older mods and Conference Customizer

Conference Customizer and older versions of Playoff Customizer (1.2.1, 1.2.0, 1.1.0, 1.0.2), Dynasty Customizer and the AIO dynasty mod (1.4.0, 1.3.1) are not supported. If you use one, Dynasty Extensions may turn itself off while you play: the three League Settings rows read **Off this session**, there is no spring game, no Weekly Strategy View button and no "Take this game". That is on purpose, not a bug. Your dynasty is not harmed and the other mod works exactly as it did. The merge file says why.

To get Dynasty Extensions working, update that mod to a version in the table above.

## Practice drills

Play Road to Glory's practice drills with your own players, in your dynasty.

1. Open **Weekly Strategy** (the **View** button on the dynasty hub) and go to **Team Profile**.
2. Press **START TRAINING**. The practice drill menu opens: Team drills and Skill drills for your drill player's position. Pick one, press Continue on the instructions, play it, and you land back in Weekly Strategy.
3. **Who plays the drill:** your first filled focus player (pick at least one focus player on Team Profile first). To pick someone else, press **X** on any filled focus card (the hint at the bottom says "Set drill player"). His drills show up the next time you open Weekly Strategy: back out to the dynasty hub and press View again. Until then his card says "Drill player (reopen Weekly Strategy)".
4. The drill player is the one on the field in the drill. Your real depth chart is never changed.

**XP:** bronze +100, silver +250, gold +500, paid once per player per week. Replaying a drill only tops you up to a better medal. A drill does not count as that week's practice plan.

**Settings** (in `Plugins\DynastyExtensions\dynasty-extensions.ini`, under `[Weekly Strategy]`; you don't need to touch them):

- `drill_xp_pct = 50` is the default. 100 pays the full Road to Glory table (200 / 500 / 1000), 0 pays nothing.
- `drill_xp = 0` turns the drill XP off. `drill_pick = 0` turns the X pick off. `drill_player_swap = 0` makes START TRAINING open an empty menu.
- Leave `drill_apply` at 0 (it skips a Road to Glory step that would crash a dynasty).

Needs the game's current version (the 29 October update).

## Spring Practice (beta)

Before you pick it, two things to know:

- **Your season starts four weeks later.** Each extra week moves the whole season one week later on the calendar, so the national title game is in February.
- **Your real starters play the drill games, so they can get hurt.** Wear is healed after each week; an injury is a real injury (a hurt player also gets no
  practice XP while he is out).

**Turning it on.** Open League Settings while you are on **Preseason Week 0** (the first week of the preseason, before the extra weeks) and set the Spring Game
row to **Spring Practice**. Then Advance as usual. A change made after that Advance waits until next year. In a brand-new dynasty the row is greyed out
until your first Advance, so your first season uses the default (Game + Practice); pick Spring Practice for year 2.

The preseason then gets four extra weeks:

- **Weeks 1, 2 and 3 are practice weeks.** Each one has a **drill game**: a game card on your dynasty hub, like the spring game, your starters against your
  second string. Playing it is optional: skip it and that week counts as a C (normal XP).
- **Week 4 is the normal spring game**: coin toss, kickoff, a full game, the normal spring game XP. No situations.

Every drill game plays the same five set situations (S1 to S5):

1. **S1 Two-minute drill** before the half, your offense. The drill game starts right there: no coin toss, no kickoff.
2. **S2 Red-zone stand**, your defense.
3. **S3 3rd and medium**, your offense.
4. **S4 Backed up** at your own 2, your offense.
5. **S5 Protect the lead**: your defense holds a 3-point lead late in the game.

Each one starts the next time that side has the ball in its half; the game is played normally in between. Each situation gets a letter from A to F
(for example the two-minute drill: touchdown A, field goal B, no points D, turnover F).

**The grades show on the scorebug** while you play, in the down-and-distance box. "1s" are your starters and "2s" your second string:

- `S2 RED ZONE` while situation 2 is on,
- `S2 1s B 2s D` after its result (your starters' letter, then your second string's; the second string's letter is only shown, it doesn't change XP),
- `DRILL D B D F F` once all five are done (`-` = not reached).

Between situations the box shows the normal down and distance. Scorebug mods that use the game's own down-and-distance text show it in their own box (tested with CFB on CN). You can turn this off in the ini
(`spring_hud_grades = 0`).

**What the grades do.** You get the same four weeks' worth of practice XP as Game + Practice, paid one week at a time; if every grade is a C, the total is
exactly the same. The first week is always the normal amount. Weeks 2, 3 and 4 are scaled by the drill game of the week before: your starting offense by
the average of S1, S3 and S4, your starting defense by the average of S2 and S5.

| Grade | A | B | C | D | F |
|---|---|---|---|---|---|
| That week's practice XP | 125 % | 110 % | 100 % | 80 % | 60 % |

A situation the game ended before you reached it counts as a C, and so does a drill game you skip. Kickers, punters and the second string always get the
normal XP, and the week-4 spring game always pays its normal XP.

Good to know:

- Your second string plays on a stand-in team (it carries your school's nickname, for example the Dukes against James Madison). It is set up again each
  week from your depth chart that week, and put back exactly as it was after each week.
- Drill games don't count: no record, no stats.
- **Known:** on 1st to 3rd down the CPU defense calls ordinary plays instead of situation plays, so a two-minute drill or red-zone stand can feel a bit easier.
- `Plugins\DynastyExtensions\wsdata.log` has a line for each situation, its result and its letter.
- **Dynasty Midgame Save:** you don't need it. If you already use it, update it to 0.2.4 or later
  (https://github.com/sdmart3/dynasty-midgame-save-releases/releases/latest) so the two work together: Midgame Save then starts each drill game, with nothing
  to set up. With an older Midgame Save the drill game plays as a normal game (no situations, normal practice XP that week).


## What's in the download

Extract the zip first. You import the `.fbmod` in the Mod Manager, not the zip.

- `Dynasty-Extensions-0.6.4.fbmod`: the mod, for the 2026-11-17 game update. Import it in the Mod Manager (it replaces `Dynasty-Extensions-0.5.0`: remove that one from the list).
- `For the 2026-10-29 game update\Dynasty-Extensions-0.5.0.fbmod`: the same mod for a game still at the 2026-10-29 update (the file of 0.5.0 to 0.6.1). Import only one of the two.
- `Manual install\Plugins\`: the plugin (**required**; replace your old one). Copy the `Plugins` folder into your Mod Manager folder.
- `INSTALL.md`: the steps, including updating and removing.
- `CHANGELOG.md`: what changed in each version.

There are no patch files in 0.6.4.

## What's new in 0.6.4

- **Works on the 2026-11-17 game update.** The update moved the game code Dynasty Extensions works with. On it, 0.6.1 turns Weekly Strategy, the spring game, the spring game kits and the runtime merge off (safely: they do nothing, the game runs), and its mod file no longer fits the update's game data. 0.6.4 knows the new game build and still knows the 2026-10-29 one, so the same Plugins folder works on both.
- **A new mod file: `Dynasty-Extensions-0.6.4.fbmod`.** The same screens as the 0.5.0 file, rebuilt for the 2026-11-17 update (one reference to the game's data changed in the update). Import it and remove `Dynasty-Extensions-0.5.0` from the Mod Manager list. If your game is still at the 2026-10-29 update, keep `Dynasty-Extensions-0.5.0.fbmod` (it is in the zip too, in `For the 2026-10-29 game update`).
- **Spring game kits that work** (the 0.6.3 fix, which was not released on its own). In the spring game your second string (the stand-in, at home) wears your school's white kit and your starters its dark kit, on team select and on the field. The 0.6.1 kit swap did not work on the field. See "What came in 0.6.3".
- **Updating from 0.6.1 (or 0.5.0, 0.5.1, 0.6.0):** close the Mod Manager and the game, copy the new `Plugins` folder over the old one and keep your ini (the plugin adds the two new kit lines for you). Start the Mod Manager, remove `Dynasty-Extensions-0.5.0` from the list, import `Dynasty-Extensions-0.6.4.fbmod` and turn it on. If you set `spring_kits = 0` yourself, change it back to `1` to get the kits.
- Everything else is the same as 0.6.1, with the same supported setups. Changed files: the mod file, `wsdata.dll`, `demerge.dll`, `anygame.dll`, the plugin, its `README.txt` and the default `dynasty-extensions.ini`. `de-expr.pack` is the same file (the game's own dynasty logic did not change in the update).

## What came in 0.6.3 (not released on its own; part of 0.6.4)

- **Spring game kits now work.** The kit swap added in 0.6.1 did not work on the field: the stand-in kept its own FCS kit and only your side changed, to your school's dark kit, so the spring game was dark against dark. The 0.6.1 notes said it was checked in game; that check was wrong. In 0.6.3 the stand-in (your second string, at home) wears your school's white kit and your starters its dark kit, on team select and on the field. The scorebug still shows the stand-in's name and logo (for example DUKES): only the uniforms change. Every other game is unchanged.
- **The 2026-10-29 title update** (from 0.6.4 also the 2026-11-17 update). On the 2026-10-13 update the spring game kits stay stock (the stand-in in its own kit), with nothing to set.
- **On by default.** `spring_kits = 1` in the `[Weekly Strategy]` part of `dynasty-extensions.ini`; set it to `0` to turn it off. Two new lines under the test switches, `spring_kits_teamrow = 1` and `spring_kits_teamrow_dry = 0`, are part of the kits: leave them as they are.
- In a league where a mod replaced the five stock FCS teams, the stand-in can keep its own kit (nothing breaks).
- Keep your ini when you update: a kept 0.6.1 ini has `spring_kits = 1`, which now works, and the plugin adds the two new lines. An ini from 0.6.0 or older has no kit lines, so the plugin uses the defaults: the kits are on.
- 0.6.2 was not released.

## What came in 0.6.1

- **Spring game kits (did not work; fixed in 0.6.3, released in 0.6.4).** Meant to dress your second string in your school's away kit and your starters in its home kit in the spring game. On the field only your side changed.
- Everything else was the same as 0.6.0.

## What came in 0.6.0

- **Dynasty Extensions fits other dynasty mods while the game runs, with no per-version data.** In 0.5.0 and 0.5.1 it carried a ready-made fit for each known version of Playoff Customizer, Dynasty Customizer and the AIO dynasty mod. Now it works out the fit from the files the game loaded, so a new version of those mods does not need a new Dynasty Extensions first. If it can't fit a file safely it turns itself Off for that session (safe, the merge file says why).
- **Same mod file, same settings.** `Dynasty-Extensions-0.5.0.fbmod` is unchanged, so you don't import it again. Only the files in the Plugins folder changed (the helper `demerge.dll` and its data file `de-expr.pack`).
- **Checked in game** on the game alone, DRI+ 3.0, Playoff Customizer 1.3.0, Dynasty Customizer 1.1.0, the AIO dynasty mod 1.4.1, and ZEO 1.0.1 + Playoff Customizer 1.3.0 + DRI 3.0.
- **Updating from 0.5.0 or 0.5.1:** copy the new `Plugins` folder over the old one. Keep your ini.
- Everything else is the same as 0.5.1 (Instant Replay while you watch a CPU game, and the separate Press Box mod being retired).

## What came in 0.5.1

- **Instant Replay while you watch a CPU game.** Leave the controller in the middle, press Start after the whistle or before the snap, and the pause menu offers Instant Replay. B goes back to the pause menu and Resume keeps watching. During a play there is no Instant Replay, the same as the game's own rule. Your own games are not changed. It is on by default; `watch_replay` in `[Press Box]` (1 = on, 0 = off) turns it off. An older ini gets the setting from the plugin.
- **The separate Press Box mod is retired.** Dynasty Extensions has everything it had. See INSTALL.md, "Coming from the separate Press Box mod".
- **Updating from 0.5.0:** copy the new `Plugins` folder over the old one. The mod file is the same, so you don't import it again.
- Everything else is the same as 0.5.0.

## What came in 0.5.0

- **No patch files.** The game alone, DRI+ 3.0, Playoff Customizer 1.3.0, Dynasty Customizer 1.1.0 and the AIO dynasty mod 1.4.1 all work with this one download. The Dynasty Extensions rows, screens and logic are added while the game runs, on top of whatever the game or another mod loaded. You don't pick a patch for your version.
- **League Settings rows are added while the game runs.** Spring Game, Weekly Strategy and Press Box appear on the League Settings screen of the game or of the mod you use. That mod's own rows (for example Playoff Customizer's bracket and sites rows) stay where they were.
- **View button and Press Box on every supported base.** The Weekly Strategy View button and the Press Box popup work on Playoff Customizer, Dynasty Customizer and the AIO dynasty mod with no extra file.
- **Two "Take this game" picks in one week now work.** Each Play Game card opens its own game (before, the second card could open the first game's teams).
- **Dynasty Extensions' requests stay out of the dynasty hub's card list** on every base (they used to show as cards on some setups).
- **The main mod no longer replaces League Settings**, so it can sit anywhere in your Mod Manager list.
- **The plugin is new:** replace your old `Plugins` folder (keep a copy of your `dynasty-extensions.ini` first).
- **Only want Press Box?** Set Spring Game and Weekly Strategy to Off in League Settings (once per dynasty, in the preseason).
- **Not supported any more:** Conference Customizer and older versions of the mods above. Dynasty Extensions may read Off with them (safe).
- **Everything else was the same as 0.4.0:** Spring Game, Spring Practice, Weekly Strategy, practice drills and Press Box work as before.

## What came in 0.4.0

- **Works with other mods that change the dynasty logic, with no copy of that logic in its own file.** A helper in the plugin adds it while the game runs, each time you load a dynasty, on top of whatever the game or another mod loaded.
- **`dynasty-extensions-merge.txt`** (in `Plugins\DynastyExtensions`) says in one line whether Dynasty Extensions is ON this session, and why not if it is OFF.
- **Nothing breaks when it can't run.** In a session where Dynasty Extensions is OFF, the Spring Game, Weekly Strategy and Press Box rows read "Off this session", and the Weekly Strategy View button and "Take this game" are not shown.

## What came in 0.3.0

- **Practice drills in your dynasty.** Weekly Strategy > Team Profile > START TRAINING opens Road to Glory's practice drills. X on a focus player picks who plays them. Bronze / silver / gold pay +100 / +250 / +500 XP, once per player per week (adjustable, see "Practice drills").

## What came in 0.2.3

- **Spring game in leagues where a mod replaced the five stock FCS teams.** Your second string now plays as one of your real FCS schools, which is put back exactly after the spring.
- **Spring restore fixed on saves with lots of other mods' data.** The stand-in school is now put back even when your save is full of other mods' rows (for example Playoff Customizer's).
- **Uninstall-crash fix.** Removing Dynasty Extensions no longer crashes saves at a stage end. Old entries are converted at your first Advance after updating.

## What came in 0.2.0

- **Spring Practice (beta).** A fifth Spring Game choice: three practice weeks with a graded drill game each, then the normal spring game (above). It is off
  unless you pick it; the default is still Game + Practice, and the other four choices work exactly as before.
- **Drill grades on the scorebug** as they happen.

## Good to know

- With Playoff Customizer, Dynasty Customizer or the AIO dynasty mod, all three parts work, Spring Game and Spring Practice included.
  The three rows sit on that mod's own League Settings screen, right after Quarter Length; its own rows stay where they were.
- The spring game's second string plays on a stand-in team (one of your real FCS schools if a mod replaced the five stock FCS teams), so it carries your school's nickname (for example the Dukes against James Madison) and you can tell the two sides apart. From 0.6.3 it wears your school's white kit (`spring_kits`, see "What's new in 0.6.3"). It's put back exactly as it was at the next Advance. The post-game screen shows a 1-0 / 0-1 record, but it doesn't stick: you start week 0 at 0-0.
- Don't use this together with the separate Press Box, Weekly Strategy or Preseason Weeks mods. This replaces them.
- Another mod that also ships `common/ui/adapterenum_cfm/scriptpod.ast` (none found among 501 mods) would take over from Dynasty Extensions; only one of the two loads.
- Back up your dynasty save before you try it.

## Before you remove it

Update to 0.2.3 or later and Advance once; after that it is safe to remove. If a save already crashes after removing an older version: turn Dynasty Extensions back on, load the save, Advance once, then remove it. The steps are in INSTALL.md (Uninstall / going back, in the zip).

## Checksums (sha256)

The zip's checksum is on the release page (`Dynasty-Extensions-0.6.4.sha256.txt`). The mod files inside the zip are listed in `Dynasty-Extensions-0.6.4.fbmod.sha256.txt` and `For the 2026-10-29 game update\Dynasty-Extensions-0.5.0.sha256.txt` in the zip too.
