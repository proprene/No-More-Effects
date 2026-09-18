![GitHub Downloads](https://img.shields.io/github/downloads/proprene/No-More-Effects/total)

##No-More-Effects

A [Nexus](https://raidcore.gg/Nexus) addon for Guild Wars 2: hide
non-essential effects and prioritize essential boons/buffs.

- **Hide the clutter.** Food, utility, boosts, guild and other non-essential
  effects disappear from the effect monitor above your skills with one key.
  Boons, conditions and combat effects stay, and the remaining icons close
  the gap.
- **Prioritize what matters.** Put important boons and buffs (Quickness,
  Alacrity, your profession's key buffs ...) in two extra rows at the top of
  the effect monitor, in your own order. They also keep their normal icon.
- **Other players too.** Hide the same clutter on party frames and the target
  frame, with its own switch and keybind.
- **Paused in PvP and WvW.** Nothing is changed in competitive modes.

```
Row 1        [Quickness][Alacrity]          <- your priorities
Row 2        [Might]
Boons        [Might][Fury][Quickness][Alacrity][Protection]
Effects      [Signet][Stance]               <- food, utility, boosts hidden
Conditions   [Bleeding][Vulnerability]
```

The addon draws nothing of its own: the game's effect monitor does all the
drawing, so icons, timers, stacks and tooltips look and behave as usual.

## Requirements

- Guild Wars 2 (64-bit) on Windows, or on macOS/Linux through Wine/CrossOver
- [Nexus](https://raidcore.gg/Nexus)

## Installation

1. Download `no_more_effects.dll` from the
   [latest release](https://github.com/proprene/No-More-Effects/releases/latest).
2. Put it in `<Guild Wars 2>/addons/`.
3. In game, open Nexus > Addons and enable **No-More-Effects**.

Nexus keeps the addon up to date from then on.

## Getting started

1. Nexus > Binds: bind **Toggle non-essential effects** (there is no default
   key). Optionally bind **Toggle non-essential effects on others** too.
2. Press the key, or click the eye icon in the Nexus quick-access bar,
   to hide or show the non-essential effects. The state is saved.
3. Fine-tune everything in Nexus > Addons > No-More-Effects.

## Options

**Hide non-essential effects** - the same switch as the key.

**Show quick-access icon** - shows or removes the eye icon in the Nexus
quick-access bar.

**Choose boon/buff to prioritize** - give a boon or buff priority **1** or
**2** and it also shows in row 1 or row 2 above your boons (row 1 is the
topmost), even if it is hidden below. The left table has the boons, the
right one the buffs of your current profession (it follows character swaps).
For a prioritized profession buff, **Hide below** hides its normal icon so it
only shows in its priority row (while hiding is on). Under the tables, arrows
set the order inside each row, left to right. Each profession keeps its own
priorities and order; swapping characters switches to theirs. Any other
effect can be given a priority in Active Effects.

**Choose category to hide** - hide whole categories of effects. The game's
own non-essential set (Food, Item, Purchased, Utility, Realtime ...) is the
default; tick or untick any category to make your own selection, or use
**Hide all** / **Hide none**. `seen` marks categories that appeared on your
effect monitor this session. Boons and conditions are never hidden.

**Active Effects** - every effect on your character (except boons and
conditions) with its name, id, category and status. **Hide** hides a single
effect, or keeps one visible while the rest of its category is hidden.
**Priority** puts it in row 1 or 2. Hidden effects that expired are listed
below, so you can still un-hide them.

**Other Players (Party and Target players/NPC)** - hides categories on the
party frames and the target frame. Your own effect monitor is not affected.
Choose a **separate keybind**, or let **the same keybind as your own
effects** switch both.

## Troubleshooting

- **The addon is disabled after a game update.** Nexus turns it off after
  every game update until it is known to work with the new build. Re-enable
  it in Nexus > Addons; if it reports that the build is not supported, wait
  for an update of the addon (Nexus installs it automatically).
- **"Unavailable: this game build is not supported."** The addon found
  nothing it recognises in this game build, so it leaves the game untouched.
  Wait for an update.
- **"Paused in PvP and WvW."** Expected: the addon does nothing in
  competitive modes. Your settings apply again once you leave.
- **The keybind does nothing.** Bind it in Nexus > Binds first. Nexus does
  not allow the same key on two binds; to use one key for yourself and
  others, pick "Same keybind as your own effects" in the Other Players
  section.

## Known limitations

- The profession buff list covers buffs that belong to a single profession
  and are common in play. Rune, sigil and relic effects are left out. Any
  effect missing there can still be prioritized from Active Effects.
- The squad grid shows no effects, so there is nothing to hide there. Party
  frames in compact mode only show boons and conditions anyway.
- A few effects have no name in the game data and show only their id.

## Third-party policy

This addon hooks game functions in memory. It gives no gameplay advantage -
it only hides or rearranges information the game already shows you - but any
third-party program is used at your own risk under ArenaNet's policies.

## Credits

- [Nexus](https://raidcore.gg/Nexus) by Raidcore, the addon loader and its
  API (MIT); the MumbleLink header from
  [gw2-mumble-cpp](https://github.com/RaidcoreGG/gw2-mumble-cpp) (MIT).
- [Dear ImGui](https://github.com/ocornut/imgui) (MIT).
- Effect category names and profession links from the
  [Hardstuck GW2 API](https://gw2-api.hardstuck.gg), cross-checked against
  arcdps combat logs.

## AI Disclosure

Parts of this project were developed with the assistance of AI tools. AI was used for RE, debugging, research, and documentation. All generated content was reviewed, tested, and adapted as necessary by myself.

## License

MIT (see [LICENSE](LICENSE)).

