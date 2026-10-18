# WorldOrbDynVars

A [ResoniteModLoader](https://github.com/resonite-modding-group/ResoniteModLoader) mod for [Resonite](https://resonite.com/) to attach a `DynamicVariableSpace` to a child slot of `WorldOrb` components that relay info for them.

# How It Works

- Whenever your local client attaches a `WorldOrb` component to a slot, an impersistent child slot will be created. This child slot will be named `WorldOrbDynVars.<Your User ID>` and destroyed when you leave the session.
- This slot will have a `DynamicVariableSpace` named `WorldOrbDynVars` created inside it.
- This space will contain the following variables:
	- `WorldOrbDynVars/Url` which is a `ValueCopy` of the `WorldOrb` component's world `URL` field.
	- `WorldOrbDynVars/SessionId.<i>` which is a `ValueCopy` of every entry in the `WorldOrb` component's `ActiveSessionIDs` list. `i` is 0 indexed and as many entries will exist as there are `ActiveSessionIDs`.

Use this to access `WorldOrb` data until https://github.com/Yellow-Dog-Man/Resonite-Issues/issues/152 is closed.

## Installation
1. Install [ResoniteModLoader](https://github.com/resonite-modding-group/ResoniteModLoader).
1. Place [WorldOrbDynVars.dll](https://github.com/Cyberboss/WorldOrbDynVars/releases/latest/download/WorldOrbDynVars.dll) into your `rml_mods` folder. This folder should be at `C:\Program Files (x86)\Steam\steamapps\common\Resonite\rml_mods` for a default install. You can create it if it's missing, or if you launch the game once with ResoniteModLoader installed it will create this folder for you.
1. Start the game. If you want to verify that the mod is working you can check your Resonite logs.
