# Study Buddies

A 5–8 player online social-deduction game set over one CMU semester. See [spec.md](spec.md) for the full design.

## Requirements

- **Godot 4.7.2 stable** (pinned). Don't open the project in a different version; upgrade only by deliberate decision and update this line.
- Git LFS (`git lfs install` once per machine) for images, audio and Aseprite files.

On macOS:

```sh
brew install git-lfs
brew install --cask godot
git lfs install
```

## Running

Open the project in Godot and press F5, or from the repo root:

```sh
godot --path .
```

To test multiplayer on one machine, run several instances (Debug → Customize Run Instances in the editor, or launch `godot --path .` in multiple terminals).

## Balance values

All tunable numbers live in [config/game_balance.tres](config/game_balance.tres). Edit them between playtests; there is no in-game settings menu.

## Local config

Machine-specific settings such as the relay server address go in `config/local.cfg`, which is git-ignored. Never commit server addresses or keys.

## Controls

| Key | Action |
| --- | --- |
| WASD / arrows | Move |
| E | Interact / collaborate |
| Tab | Task list |
| Enter | Open chat (dinners) |
| Esc | Menu |
| F11 | Toggle fullscreen |
