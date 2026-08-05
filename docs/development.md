# Development

Minecraft: The Other Update is developed against Minecraft Java Edition 1.0.0 with RetroMCP-Java and Java 8.

## Local folders

Keep the editable Minecraft workspace and the Git repository separate:

```text
C:\MinecraftDevelopment\
├── Minecraft-The-Other-Update-RMCP\
└── the-other-update\
```

`Minecraft-The-Other-Update-RMCP` contains the local RetroMCP workspace and decompiled game source.

`the-other-update` is the clean Git repository.

## Required tools

- 64-bit Java Development Kit 8
- RetroMCP-Java GUI
- GitHub Desktop or Git
- Prism Launcher for later distribution testing

The current Java 8 installation is expected at:

```text
C:\Java\zulu8
```

## Development workflow

1. Edit the relevant source inside the local RetroMCP workspace.
2. Run Recompile in RetroMCP.
3. Launch the client through RetroMCP.
4. Test the change in a new or disposable world.
5. Export or reproduce the safe project changes in this repository.
6. Review the GitHub Desktop diff.
7. Commit and push only original files and patches.

The exact patch-export procedure will be documented after the first clean source patch is generated and verified.

## Repository contents

The repository may contain:

- Original source files added by the project
- Patches against Minecraft classes
- Original textures, sounds and other assets
- Documentation
- Launcher metadata and release tooling

## Files that must not be committed

Do not commit:

- Decompiled Minecraft source
- Minecraft client or server JARs
- Mojang assets
- Compiled Minecraft classes
- Local worlds, logs or account data
- The complete RetroMCP workspace

The root `.gitignore` blocks the common generated folders and file types, but every GitHub Desktop change list should still be reviewed before committing.

## Testing notes

Record tests against a clean Minecraft 1.0.0 environment where practical.

For gameplay changes, test at least:

- New world creation
- Save and reload
- Breaking and placing affected blocks
- Inventory and held-item rendering
- Expected behavior after death
- Interaction from all valid directions

Multiplayer and dedicated-server behavior must be listed as untested until verified separately.
