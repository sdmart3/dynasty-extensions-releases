# Dynasty Extensions

**Download:** https://github.com/sdmart3/dynasty-extensions-releases/releases/latest (the zip has the mod, the plugin, the patches and the install steps).


Three dynasty add-ons in one mod:

- **Press Box.** Play or watch any game of the week. Go to EA SPORTS Network > Scores / Schedules, press A on a game and pick
  **Take this game**. It shows up as a card on your hub. On the controller screen, move your controller to a team to play it, or leave it in the middle to watch.
- **Weekly Strategy.** Press **View** on the dynasty hub. You get the Weekly Strategy screen: pick focus players, see this week's
  coach goal and choose a gameplan focus. They give your players XP each week.
- **Spring Game.** One extra preseason week with a spring game: your starters against your second string. Your players also get
  four weeks of practice XP before it. Records and stats don't count. Play it from the hub like any other game.

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

More detail settings (watch pause, the controller screen, which Weekly Strategy panels fill in) are in
`Plugins\DynastyExtensions\dynasty-extensions.ini`. You don't need to touch it.

## What's in the download

- `Dynasty-Extensions-0.1.4.fbmod`: the mod. Import it in the Mod Manager.
- `Manual install\Plugins\`: the plugin (required). Copy the `Plugins` folder into your Mod Manager folder.
- `Compatibility patches\`: only if you use one of these mods (see INSTALL).

See **INSTALL.md** in the zip for the steps and the load order.

## Good to know

- With Playoff Customizer, Dynasty Customizer or the AIO dynasty mod, all three parts work through their patch, Spring Game included.
  The three rows sit on that mod's own League Settings screen, right after Quarter Length; its playoff rows stay where they were.
- With those three mods, every playoff field size they offer works with all three parts, 64 teams included (the AIO dynasty mod
  stops at 16). A dynasty has room for 150 of these mods' save rows (the game's limit); a 64-team field with everything on uses 147. So with 64 teams,
  leave Playoff Sites at their defaults or change only one or two (each custom site you save takes one more row).
- A 64-team field needs a dynasty with room for the extra playoff games: one started with Playoff Customizer on, or one widened
  with the CFB 27 Playoff Room app. That is Playoff Customizer's own rule, not this mod's.
- The spring game's second string plays on a stand-in team for that one week, so it carries your school's nickname (for example the Dukes against James Madison) and you can tell the two sides apart. It's put back exactly as it was at the next Advance. The post-game screen shows a 1-0 / 0-1 record, but it doesn't stick: you start week 0 at 0-0.
- Don't use this together with the separate Press Box, Weekly Strategy or Preseason Weeks mods. This replaces them.
- Back up your dynasty save before you try it.
