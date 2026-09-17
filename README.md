No-More-Effects

A Nexus addon for Guild Wars 2. It hides the non-essential effects (food, utility enhancements, boosts, gear procs and the like) from the effect monitor above your utility skills. One keybind switches them off and on.

Boons, conditions, stances, signets, auras, transformations and every other effect stay where they are. The remaining icons close the gap, so the row actually gets shorter.

visible:   [food][utility][guild][might][fury][quickness][stance]
hidden:    [might][fury][quickness][stance]
           [Heal][Utility][Utility][Utility][Elite]

The addon does not draw anything. The game's own effect widget rebuilds its list without those categories, following the same rule the game already uses for other players' effect lists.
Requirements

    Guild Wars 2 (64-bit), Windows or Wine/CrossOver
    Nexus with API version 6
    The game build must match the signatures. The addon is marked volatile, so Nexus disables it after every game update until it has been checked.

Installation

    Download no_more_effects.dll from a release or from the artifacts of a successful Actions run, or build it yourself (see below).
    Copy the DLL to <Guild Wars 2>/addons/.
    In game, open Nexus > Addons and enable No-More-Effects.

Usage

    Nexus > Binds: bind Toggle non-essential effects. There is no default key.
    Press it to hide or show the non-essential effects. The state is saved.

The options panel is in Nexus > Addons > No-More-Effects:

    Hide non-essential effects: the same switch as the key.
    Hidden categories: by default, the game's own non-essential set (categories 5, 7, 9, 14, 16 and 18 on the current build). Untick "Use the game's non-essential categories" to choose your own. Boons and conditions cannot be hidden.
    Diagnostics: skill id and category of every icon currently shown.

Settings are stored in <Guild Wars 2>/addons/No-More-Effects/settings.ini.
