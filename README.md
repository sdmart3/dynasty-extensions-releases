# Dynasty Extensions

**Download:** https://github.com/sdmart3/dynasty-extensions-releases/releases/latest (the zip has the mod, the plugin, the patches and the install steps).

Three dynasty add-ons in one mod: Press Box, Weekly Strategy and Preseason Weeks (the spring game).

## Install in 4 steps

Extract the zip first. You import the `.fbmod` in the Mod Manager, not the zip. Back up your dynasty save before you try it.

1. Close the game and the Mod Manager. Copy the `Plugins` folder from `Manual install` into your Mod Manager folder (next to `MMCModManager.exe`). **The plugin is required**: without it nothing of Dynasty Extensions runs.
2. Open the Mod Manager, import `Dynasty-Extensions-0.4.0.fbmod` and turn it on.
3. If you also use one of the mods in the table below, import its ONE patch from `Compatibility patches` too, at the very bottom of the Mod Manager list.
4. Start the Mod Manager again (it loads plugins when it starts), launch the game from it and load your dynasty. About 30 seconds after the game starts the plugin's helper is in.

Then open `Plugins\DynastyExtensions\dynasty-extensions-merge.txt`: its first line says `Dynasty Extensions is ON`. If it says `ready`, go back to the main menu and load the dynasty again. If it says `OFF this session because ...`, see "Is it on?" below.

Updating from 0.3.0 or older: see INSTALL.md (replace the mod, the plugin and your patch).

## Which patch do I need?

| You also use | What you need |
|---|---|
| Nothing that changes dynasty logic | Nothing. It works as soon as the mod and the plugin are in. |
| DRI+ 3.0 | Nothing. Load order: DRI+ on top, Dynasty Extensions under it. (Older DRI+ versions are not covered.) |
| Conference Customizer 1.0.2 | The small Conference Customizer patch (screens only). The 0.3.0 patch also works. |
| Playoff Customizer 1.3.0, Dynasty Customizer 1.1.0, AIO dynasty mod 1.3.1 / 1.4.0 / 1.4.1 | The patch for that mod. Import only ONE patch. |
| Playoff Customizer 1.1.0 | No patch. Dynasty Extensions stays off while you use it (see "Playoff Customizer 1.1.0" below). |

**What changed in 0.4.0, in plain words:** Dynasty Extensions no longer carries its own copy of the game's dynasty logic file. A small helper in the plugin adds that logic while the game runs, each time you load a dynasty, on top of whatever the game (or another mod) loaded. That is why DRI+ 3.0 works with no patch and Conference Customizer needs only a small screens patch.

## What it does

- **Press Box (0.7.3).** Play or watch any game of the week. Go to EA SPORTS Network > Scores / Schedules, press A on a game and pick
  **Take this game**. It shows up as a card on your hub. On the controller screen, move your controller to a team to play it, or leave it in the middle to watch.
- **Weekly Strategy.** Press the **View** button on the dynasty hub (it is not under Practice). You get the Weekly Strategy screen: pick focus players, see this week's
  coach goal and choose a gameplan focus. They give your players XP each week. START TRAINING on Team Profile opens Road to Glory's practice drills for your players (see "Practice drills" below). You start with 3 focus players; each position Whisperer talent your head coach owns
  opens one more, up to 6 (Talent Developer tree in Upgrade Coach Skills: QB, RB, WR/TE, OL, DL, LB, DB and K/P Whisperer). It works with Call Sheet's Weekly Strategy link: your gameplan focus is written to a small
  file that Call Sheet 0.14.1 or later reads, so Call Sheet's suggestions follow it, with nothing to set up.
- **Spring Game.** One extra preseason week with a spring game: your starters against your second string, with attendance set to half the stadium (the empty seats show mostly in the end zones).
  Your players also get four weeks' worth of practice XP before it. Records and stats don't count. Play it from the hub like any other game.
  - **Spring Practice** (beta, off unless you pick it). Four extra preseason weeks instead of one: three practice weeks, each with a drill game
    of five graded situations, then the normal spring game. The grades raise or lower the next week's practice XP. See "Spring Practice" below.
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

More detail settings (watch pause, the controller screen, which Weekly Strategy panels fill in, the Call Sheet file, the scorebug text) are in
`Plugins\DynastyExtensions\dynasty-extensions.ini`. You don't need to touch it.


## Is it on? (new in 0.4.0)

Open `Plugins\DynastyExtensions\dynasty-extensions-merge.txt` after you load a dynasty. Its first line says `Dynasty Extensions is ON` or `Dynasty Extensions is OFF this session because ...`, and the next line says what to do. When it is ON you do not have to do anything.

When it is OFF, nothing of Dynasty Extensions runs, and nothing that needs it can be pressed: the Spring Game, Weekly Strategy and Press Box rows in League Settings are greyed and read **Off this session**, Scores / Schedules shows the game's own menu (no "Take this game"), and the dynasty hub has no Weekly Strategy View button. Your dynasty is not harmed: you can play, advance and save, and your settings are kept for the next time it is ON.

If you loaded the dynasty before the helper was in (about 30 seconds after the game starts), the file still says "ready": go back to the main menu and load the dynasty again.

## Playoff Customizer 1.1.0

There is no Dynasty Extensions patch for Playoff Customizer 1.1.0. If you use it, Dynasty Extensions turns itself off while you play: the three League Settings rows are greyed and read **Off this session**, there is no spring game, no Weekly Strategy View button and no "Take this game". That is on purpose, not a bug. Your dynasty is not harmed and Playoff Customizer works exactly as it did. The merge file says `Dynasty Extensions is OFF this session because another mod changed the same dynasty logic and no matching patch is loaded`.

To get Dynasty Extensions working, update to Playoff Customizer 1.3.0 and use the Playoff Customizer 1.3.0 patch from this download (load order: Playoff Customizer on top, Dynasty Extensions under it, the patch at the very bottom). Or just keep playing as you are.
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
- **Dynasty Midgame Save:** you don't need it. If you already use it, update it to 0.2.4
  (https://github.com/sdmart3/dynasty-midgame-save-releases/releases/latest) so the two work together: Midgame Save then starts each drill game, with nothing
  to set up. With an older Midgame Save the drill game plays as a normal game (no situations, normal practice XP that week).


## What's in the download

Extract the zip first. You import the `.fbmod` files in the Mod Manager, not the zip.

- `Dynasty-Extensions-0.4.0.fbmod`: the mod. Import it in the Mod Manager.
- `Manual install\Plugins\`: the plugin (**required**; new in 0.4.0, so replace your old one: it now also holds `demerge.dll` and `de-expr.pack`). Copy the `Plugins` folder into your Mod Manager folder.
- `Compatibility patches\`: six patch files, only if you use one of those mods (table below). Import only the ONE patch for the base mod you have, and put it at the very bottom of the Mod Manager list (see INSTALL).
  There are three AIO dynasty mod patches: pick the one that matches your AIO version (1.3.1, 1.4.0 or 1.4.1).

See **INSTALL.md** (in the zip) for the steps and the load order.

## What's new in 0.4.0

- **Works with other mods that change the dynasty logic, with no copy of that logic in its own file.** A helper in the plugin adds it while the game runs, each time you load a dynasty, on top of whatever the game or another mod loaded.
- **DRI+ 3.0 works with Dynasty Extensions with no patch.** Conference Customizer 1.0.2 needs only a small screens patch.
- **`dynasty-extensions-merge.txt`** (in `Plugins\DynastyExtensions`) says in one line whether Dynasty Extensions is ON this session, and why not if it is OFF.
- **Nothing breaks when it can't run.** In a session where Dynasty Extensions is OFF, the Spring Game, Weekly Strategy and Press Box rows read "Off this session", and the Weekly Strategy View button and "Take this game" are not shown.
- **The plugin is required now, and it is new:** replace your old `Plugins` folder (keep a copy of your `dynasty-extensions.ini` first).
- **Playoff Customizer 1.1.0** has no patch: Dynasty Extensions stays off and says so; your dynasty is not affected.
- **Everything else is the same as 0.3.0:** Spring Game, Spring Practice, Weekly Strategy, practice drills and Press Box work as before. The Playoff Customizer 1.3.0, Dynasty Customizer 1.1.0 and AIO dynasty mod patches carry the same content as the 0.3.0 ones.

## What came in 0.3.0

- **Practice drills in your dynasty.** Weekly Strategy > Team Profile > START TRAINING opens Road to Glory's practice drills. X on a focus player picks who plays them. Bronze / silver / gold pay +100 / +250 / +500 XP, once per player per week (adjustable, see "Practice drills").

## What came in 0.2.3

- **Spring game in leagues where a mod replaced the five stock FCS teams.** Your second string now plays as one of your real FCS schools, which is put back exactly after the spring.
- **Spring restore fixed on saves with lots of other mods' data.** The stand-in school is now put back even when your save is full of other mods' rows (for example Playoff Customizer's).
- **Uninstall-crash fix.** Removing Dynasty Extensions no longer crashes saves at a stage end. Old entries are converted at your first Advance after updating.
- **Every compatibility patch is new** (Playoff Customizer 1.3.0, Dynasty Customizer 1.1.0, Conference Customizer 1.0.2, AIO dynasty mod 1.3.1 / 1.4.0 / 1.4.1). Replace your patch too (one patch only, at the very bottom of the list).

## What came in 0.2.0

- **Spring Practice (beta).** A fifth Spring Game choice: three practice weeks with a graded drill game each, then the normal spring game (above). It is off
  unless you pick it; the default is still Game + Practice, and the other four choices work exactly as before.
- **Drill grades on the scorebug** as they happen.
- **Every compatibility patch is new.** They carry Spring Practice, so replace your patch too (one patch only, at the very bottom of the list).

## Good to know

- With Playoff Customizer, Dynasty Customizer or the AIO dynasty mod (1.3.1, 1.4.0 or 1.4.1), all three parts work through their patch, Spring Game and Spring Practice included.
  The three rows sit on that mod's own League Settings screen, right after Quarter Length; its own rows stay where they were.
- With those mods, every playoff field size they offer works with all three parts, 64 teams included (the AIO dynasty mod
  stops at 16). Your dynasty has room for 150 rows of these mods' settings (the game's limit); a 64-team field with everything on uses 147. So with 64 teams,
  leave Playoff Sites at their defaults or change only one or two (each custom site you save takes one more row). Spring Practice uses no extra row.
- A 64-team field needs a dynasty with room for the extra playoff games: one started with Playoff Customizer on, or one widened
  with the CFB 27 Playoff Room app. That is Playoff Customizer's own rule, not this mod's.
- The spring game's second string plays on a stand-in team (one of your real FCS schools if a mod replaced the five stock FCS teams), so it carries your school's nickname (for example the Dukes against James Madison) and you can tell the two sides apart. It's put back exactly as it was at the next Advance. The post-game screen shows a 1-0 / 0-1 record, but it doesn't stick: you start week 0 at 0-0.
- DRI+ 3.0 works with Dynasty Extensions with no patch (older DRI+ versions are not covered).
- Don't use this together with the separate Press Box, Weekly Strategy or Preseason Weeks mods. This replaces them.
- Back up your dynasty save before you try it.

## Before you remove it

Update to 0.2.3 or later and Advance once; after that it is safe to remove. If a save already crashes after removing an older version: turn Dynasty Extensions back on, load the save, Advance once, then remove it. The steps are in INSTALL.md (Uninstall / going back, in the zip).

## Compatibility patches

Each patch is also a separate download. Use only the one for your base mod, and put it at the very bottom of the Mod Manager list. Use them with the 0.4.0 main mod and the 0.4.0 plugin.
Five of the six carry the same content as the 0.3.0 patches (Playoff Customizer 1.3.0, Dynasty Customizer 1.1.0, AIO dynasty mod 1.3.1 / 1.4.0 / 1.4.1): they are labelled 0.4.0 now. The Conference Customizer 1.0.2 patch is new in 0.4.0 (screens only; the 0.3.0 one also works).

| You use | Patch file | sha256 |
|---|---|---|
| Playoff Customizer 1.3.0 | [`Dynasty-Extensions-x-Playoff-Customizer-1.3.0-patch.fbmod`](https://github.com/sdmart3/dynasty-extensions-releases/releases/latest/download/Dynasty-Extensions-x-Playoff-Customizer-1.3.0-patch.fbmod) | `d6a65b8e75800d477a628de8676912973b5cf5f6bd8d3c6365ac1d2b9c719861` |
| Dynasty Customizer 1.1.0 | [`Dynasty-Extensions-x-Dynasty-Customizer-1.1.0-patch.fbmod`](https://github.com/sdmart3/dynasty-extensions-releases/releases/latest/download/Dynasty-Extensions-x-Dynasty-Customizer-1.1.0-patch.fbmod) | `ab8dfa2e05ee92ad15c0b185db04839080f6dcba72a3256b449a54e716a716d7` |
| Conference Customizer 1.0.2 | [`Dynasty-Extensions-x-Conference-Customizer-1.0.2-patch.fbmod`](https://github.com/sdmart3/dynasty-extensions-releases/releases/latest/download/Dynasty-Extensions-x-Conference-Customizer-1.0.2-patch.fbmod) | `1eedf1ac04149aa88df0e3c92d2da4e3e52e6381ce39e4abd2a5f1886757bf06` |
| AIO Dynasty Mod v1.3.1 | [`Dynasty-Extensions-x-AIO-Dynasty-1.3.1-patch.fbmod`](https://github.com/sdmart3/dynasty-extensions-releases/releases/latest/download/Dynasty-Extensions-x-AIO-Dynasty-1.3.1-patch.fbmod) | `db04b4afc81c852356549aa65fceb62068ff42710544e13ddca49056d4f710e3` |
| AIO Dynasty Mod v1.4.0 | [`Dynasty-Extensions-x-AIO-Dynasty-1.4.0-patch.fbmod`](https://github.com/sdmart3/dynasty-extensions-releases/releases/latest/download/Dynasty-Extensions-x-AIO-Dynasty-1.4.0-patch.fbmod) | `a0f16a6d7f35da5ed39c6639e1094fd046a853abfe601eafcda40cdf70a1b8da` |
| AIO Dynasty Mod v1.4.1 | [`Dynasty-Extensions-x-AIO-Dynasty-1.4.1-patch.fbmod`](https://github.com/sdmart3/dynasty-extensions-releases/releases/latest/download/Dynasty-Extensions-x-AIO-Dynasty-1.4.1-patch.fbmod) | `2f3d4cfc4982d4d0daaca3c2c2498ee49b6763da1fdee523b151815ffdd4e66f` |

If a base mod updates before a new release, a new patch may be added here as a separate download.

## Checksums (sha256)

| File | sha256 |
|---|---|
| `Dynasty-Extensions-0.4.0.fbmod` (inside the zip) | `c42a0ce0a5c27129ecd5e894d2422ffcd484318a22ddc3aead63c1563536039f` |

The zip's own checksum is on the release page (`Dynasty-Extensions-0.4.0.sha256.txt`). Every file is also attached with its own `.sha256.txt`.
