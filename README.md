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
  Your players also get four weeks of practice XP before it. Records and stats don't count. Play it from the hub like any other game.

## What's new in 0.1.8

- **Watching a game after taking control of the opponent could crash. Fixed.**
- **No longer conflicts with mods that change the controller/options menu file.** Dynasty Extensions doesn't replace that file any more, so it works alongside such mods with no patch. The AIO Broadcast mod, for example, works next to it as it is: its settings (the scorebug included) work, and you can take a game and watch it.
- New Compatibility patch for the AIO dynasty mod 1.4.1 (now in the zip too).

## Turning things on and off

Open **League Settings** in your dynasty (the screen is titled Dynasty Settings). Three rows sit right after Quarter Length, under Clock Management:

| Row | Choices |
|---|---|
| Spring Game | Off / Game Only / Game + Practice / All Teams Practice |
| Weekly Strategy | On / Off |
| Press Box | On / Off |

Spring Game choices:

- **Off**: no extra week.
- **Game Only**: the extra week and the spring game, with game XP. No practice XP.
- **Game + Practice** (default): the same, plus four weeks of practice XP for your team before the game (roughly one to two skill points a player).
- **All Teams Practice**: the same as Game + Practice, and every CPU team gets the four weeks of practice XP too. CPU teams never play a game.

- In a brand-new dynasty these rows are greyed out until your first Advance. Until then everything runs at its default (all on, Game + Practice).
- Weekly Strategy and Press Box change right away. The Spring Game choice counts at the next preseason Advance.
- Turning one off leaves the other two alone.

More detail settings (watch pause, the controller screen, which Weekly Strategy panels fill in, the Call Sheet file) are in
`Plugins\DynastyExtensions\dynasty-extensions.ini`. You don't need to touch it.

## What's in the download

Extract the zip first. You import the `.fbmod` files in the Mod Manager, not the zip.

- `Dynasty-Extensions-0.1.8.fbmod`: the mod. Import it in the Mod Manager.
- `Manual install\Plugins\`: the plugin (required). Copy the `Plugins` folder into your Mod Manager folder.
- `Compatibility patches\`: only if you use one of these mods. Import only the ONE patch for the base mod you have, and load it last (see INSTALL).
  There are three AIO dynasty mod patches: pick the one that matches your AIO version (1.3.1, 1.4.0 or 1.4.1).

See **INSTALL.md** for the steps and the load order.

## Compatibility patches

Each patch is also a separate download. Use only the one for your base mod, and load it last.

| You use | Patch file |
|---|---|
| Playoff Customizer 1.3.0 | [`Dynasty-Extensions-x-Playoff-Customizer-1.3.0-patch.fbmod`](https://github.com/sdmart3/dynasty-extensions-releases/releases/latest/download/Dynasty-Extensions-x-Playoff-Customizer-1.3.0-patch.fbmod) |
| Dynasty Customizer 1.1.0 | [`Dynasty-Extensions-x-Dynasty-Customizer-1.1.0-patch.fbmod`](https://github.com/sdmart3/dynasty-extensions-releases/releases/latest/download/Dynasty-Extensions-x-Dynasty-Customizer-1.1.0-patch.fbmod) |
| Conference Customizer 1.0.2 | [`Dynasty-Extensions-x-Conference-Customizer-1.0.2-patch.fbmod`](https://github.com/sdmart3/dynasty-extensions-releases/releases/latest/download/Dynasty-Extensions-x-Conference-Customizer-1.0.2-patch.fbmod) |
| AIO Dynasty Mod v1.3.1 | [`Dynasty-Extensions-x-AIO-Dynasty-1.3.1-patch.fbmod`](https://github.com/sdmart3/dynasty-extensions-releases/releases/latest/download/Dynasty-Extensions-x-AIO-Dynasty-1.3.1-patch.fbmod) |
| AIO Dynasty Mod v1.4.0 | [`Dynasty-Extensions-x-AIO-Dynasty-1.4.0-patch.fbmod`](https://github.com/sdmart3/dynasty-extensions-releases/releases/latest/download/Dynasty-Extensions-x-AIO-Dynasty-1.4.0-patch.fbmod) |
| AIO Dynasty Mod v1.4.1 | [`Dynasty-Extensions-x-AIO-Dynasty-1.4.1-patch.fbmod`](https://github.com/sdmart3/dynasty-extensions-releases/releases/latest/download/Dynasty-Extensions-x-AIO-Dynasty-1.4.1-patch.fbmod) |

If a base mod updates before a new release, a new patch may be added here as a separate download.

## Good to know

- With Playoff Customizer, Dynasty Customizer or the AIO dynasty mod (1.3.1, 1.4.0 or 1.4.1), all three parts work through their patch, Spring Game included.
  The three rows sit on that mod's own League Settings screen, right after Quarter Length; its own rows stay where they were.
- With those mods, every playoff field size they offer works with all three parts, 64 teams included (the AIO dynasty mod
  stops at 16). A dynasty has room for 150 of these mods' save rows (the game's limit); a 64-team field with everything on uses 147. So with 64 teams,
  leave Playoff Sites at their defaults or change only one or two (each custom site you save takes one more row).
- A 64-team field needs a dynasty with room for the extra playoff games: one started with Playoff Customizer on, or one widened
  with the CFB 27 Playoff Room app. That is Playoff Customizer's own rule, not this mod's.
- The spring game's second string plays on a stand-in team for that one week, so it carries your school's nickname (for example the Dukes against James Madison) and you can tell the two sides apart. It's put back exactly as it was at the next Advance. The post-game screen shows a 1-0 / 0-1 record, but it doesn't stick: you start week 0 at 0-0.
- DRI+ replaces the same dynasty files as this mod, so it can't be used with Dynasty Extensions (or with a base mod plus its Dynasty Extensions patch).
- Don't use this together with the separate Press Box, Weekly Strategy or Preseason Weeks mods. This replaces them.
- Back up your dynasty save before you try it.
