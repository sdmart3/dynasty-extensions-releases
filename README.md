# Dynasty Extensions

**Download:** https://github.com/sdmart3/dynasty-extensions-releases/releases/latest (the zip has the mod, the plugin, the patches and the install steps).

Three dynasty add-ons in one mod:

- **Press Box (0.7.3).** Play or watch any game of the week. Go to EA SPORTS Network > Scores / Schedules, press A on a game and pick
  **Take this game**. It shows up as a card on your hub. On the controller screen, move your controller to a team to play it, or leave it in the middle to watch.
- **Weekly Strategy.** Press the **View** button on the dynasty hub (it is not under Practice). You get the Weekly Strategy screen: pick focus players, see this week's
  coach goal and choose a gameplan focus. They give your players XP each week. You start with 3 focus players; each position Whisperer talent your head coach owns
  opens one more, up to 6 (Talent Developer tree in Upgrade Coach Skills: QB, RB, WR/TE, OL, DL, LB, DB and K/P Whisperer). It works with Call Sheet's Weekly Strategy link: your gameplan focus is written to a small
  file that Call Sheet 0.14.1 or later reads, so Call Sheet's suggestions follow it, with nothing to set up.
- **Spring Game.** One extra preseason week with a spring game: your starters against your second string, with attendance set to half the stadium (the empty seats show mostly in the end zones).
  Your players also get four weeks' worth of practice XP before it. Records and stats don't count. Play it from the hub like any other game.
  - **New in 0.2.0: Spring Practice** (beta, off unless you pick it). Four extra preseason weeks instead of one: three practice weeks, each with a drill game
    of five graded situations, then the normal spring game. The grades raise or lower the next week's practice XP. See "Spring Practice" below.

You install two things: the mod (`.fbmod`, imported in the Mod Manager) and the plugin (the `Plugins` folder, copied into your Mod Manager folder). See INSTALL.md in the zip.

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

- `Dynasty-Extensions-0.2.3.fbmod`: the mod. Import it in the Mod Manager.
- `Manual install\Plugins\`: the plugin (required). Copy the `Plugins` folder into your Mod Manager folder.
- `Compatibility patches\`: only if you use one of these mods. Import only the ONE patch for the base mod you have, and put it at the very bottom of the Mod Manager list (see INSTALL).
  There are three AIO dynasty mod patches: pick the one that matches your AIO version (1.3.1, 1.4.0 or 1.4.1).

See **INSTALL.md** (in the zip) for the steps and the load order.

## What's new in 0.2.3

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
  stops at 16). A dynasty has room for 150 of these mods' save rows (the game's limit); a 64-team field with everything on uses 147. So with 64 teams,
  leave Playoff Sites at their defaults or change only one or two (each custom site you save takes one more row). Spring Practice uses no extra row.
- A 64-team field needs a dynasty with room for the extra playoff games: one started with Playoff Customizer on, or one widened
  with the CFB 27 Playoff Room app. That is Playoff Customizer's own rule, not this mod's.
- The spring game's second string plays on a stand-in team (one of your real FCS schools if a mod replaced the five stock FCS teams), so it carries your school's nickname (for example the Dukes against James Madison) and you can tell the two sides apart. It's put back exactly as it was at the next Advance. The post-game screen shows a 1-0 / 0-1 record, but it doesn't stick: you start week 0 at 0-0.
- DRI+ replaces the same dynasty files as this mod, so it can't be used with Dynasty Extensions (or with a base mod plus its Dynasty Extensions patch).
- Don't use this together with the separate Press Box, Weekly Strategy or Preseason Weeks mods. This replaces them.
- Back up your dynasty save before you try it.

## Before you remove it

Update to 0.2.3 and Advance once; after that it is safe to remove. If a save already crashes after removing an older version: turn Dynasty Extensions back on, load the save, Advance once, then remove it. The steps are in INSTALL.md (Uninstall / going back, in the zip).

## Compatibility patches

Each patch is also a separate download. Use only the one for your base mod, and put it at the very bottom of the Mod Manager list.
All of them are new in 0.2.3: use them with the 0.2.3 main mod.

| You use | Patch file | sha256 |
|---|---|---|
| Playoff Customizer 1.3.0 | [`Dynasty-Extensions-x-Playoff-Customizer-1.3.0-patch.fbmod`](https://github.com/sdmart3/dynasty-extensions-releases/releases/latest/download/Dynasty-Extensions-x-Playoff-Customizer-1.3.0-patch.fbmod) | `774f4d315684cd66cf930ce2492a8520253187a4a9ee5835ff3597903f004831` |
| Dynasty Customizer 1.1.0 | [`Dynasty-Extensions-x-Dynasty-Customizer-1.1.0-patch.fbmod`](https://github.com/sdmart3/dynasty-extensions-releases/releases/latest/download/Dynasty-Extensions-x-Dynasty-Customizer-1.1.0-patch.fbmod) | `e3f11cb09243cee778f05b032ce5f22ca1b087d87ef35ae7f8da69490d86b685` |
| Conference Customizer 1.0.2 | [`Dynasty-Extensions-x-Conference-Customizer-1.0.2-patch.fbmod`](https://github.com/sdmart3/dynasty-extensions-releases/releases/latest/download/Dynasty-Extensions-x-Conference-Customizer-1.0.2-patch.fbmod) | `ce9e8fa2406218ab61730dc6c6186284e6be6389e509531c4525b379a0fa091f` |
| AIO Dynasty Mod v1.3.1 | [`Dynasty-Extensions-x-AIO-Dynasty-1.3.1-patch.fbmod`](https://github.com/sdmart3/dynasty-extensions-releases/releases/latest/download/Dynasty-Extensions-x-AIO-Dynasty-1.3.1-patch.fbmod) | `64c416208161735443a135e0af852f764398f59492def58272cabe24ead558f1` |
| AIO Dynasty Mod v1.4.0 | [`Dynasty-Extensions-x-AIO-Dynasty-1.4.0-patch.fbmod`](https://github.com/sdmart3/dynasty-extensions-releases/releases/latest/download/Dynasty-Extensions-x-AIO-Dynasty-1.4.0-patch.fbmod) | `535a8434c31b90071fdd1cd7b50459eafa67f03b580e418b6f6906a406b4cdb4` |
| AIO Dynasty Mod v1.4.1 | [`Dynasty-Extensions-x-AIO-Dynasty-1.4.1-patch.fbmod`](https://github.com/sdmart3/dynasty-extensions-releases/releases/latest/download/Dynasty-Extensions-x-AIO-Dynasty-1.4.1-patch.fbmod) | `b70e6a3780cfc7e40050911de7e8a7528e66e9c3eb7085c1d39b4b4b3ca6e343` |

If a base mod updates before a new release, a new patch may be added here as a separate download.

## Checksums (sha256)

| File | sha256 |
|---|---|
| `Dynasty-Extensions-0.2.3.zip` | `dd6425fa7b9de2da1ba8c46cf458f5bad6ed9c327dd90381ecdac89dc562e7a0` |
| `Dynasty-Extensions-0.2.3.fbmod` (inside the zip) | `36ba69cda05b0ed675ca0b7142dcc1dd97c21f89c85fc2284d596ac84a8bc28f` |

Every file is also attached with its own `.sha256.txt`.
