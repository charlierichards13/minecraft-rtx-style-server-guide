# Server-Side Setup

This page covers the server pieces of the visual stack:

- Paper 26.2
- Dynamic Lights v1.9.3 datapack
- Faithful 32x server resource pack hosted through mc-packs

The server-side setup improves the shared experience, but it does not replace client-side shaders.

## Paper 26.2

Download Paper from the official PaperMC downloads page:

- [PaperMC downloads](https://papermc.io/downloads/)

Use the build that matches Minecraft Java 26.2.

## Dynamic Lights Datapack

Download Tschipcraft Dynamic Lights from the official Modrinth page:

- [Tschipcraft Dynamic Lights on Modrinth](https://modrinth.com/datapack/dynamic-lights)
- [Tschipcraft's Dynamic Lights on CurseForge](https://www.curseforge.com/minecraft/data-packs/tschipcrafts-dynamic-lights)

Datapacks go inside the active world folder:

```text
world/datapacks
```

Example:

```text
world/datapacks/dynamiclights-v1.9.3-mc1.17-26.2.9-datapack.zip
```

Do not unzip datapacks unless the datapack author specifically tells you to. Most datapacks can stay zipped.

After adding a datapack:

1. Restart the server, or run `/reload` if appropriate.
2. Run `/datapack list`.
3. Confirm Dynamic Lights appears in the enabled datapack list.

## Faithful 32x Server Resource Pack

Download Faithful from the official Faithful site:

- [Faithful downloads](https://faithfulpack.net/downloads)

Do not commit the Faithful `.zip` file to this repository.

To let the server offer the resource pack to players, host the pack externally and configure `server.properties`.

This setup uses mc-packs:

- [mc-packs resource pack hosting](https://mc-packs.net/)

Basic flow:

1. Download the correct Faithful 32x Java pack.
2. Upload the resource pack `.zip` to mc-packs.
3. Copy the generated resource pack URL.
4. Copy the generated SHA-1 hash if mc-packs provides one.
5. Add both values to `server.properties`.

Example `server.properties` fields:

```properties
resource-pack=https://download.mc-packs.net/pack/example-pack-url.zip
resource-pack-sha1=example_sha1_hash
require-resource-pack=false
resource-pack-prompt={"text":"This server uses Faithful 32x for the intended vanilla+ look.","color":"gold"}
```

Use the real URL and SHA-1 from mc-packs. The values above are placeholders.

## Should the Pack Be Required?

Recommended:

```properties
require-resource-pack=false
```

This lets players join even if their download fails or they want to troubleshoot. For a private server where the visual style is mandatory, admins can set it to `true`, but that may block players with resource pack download issues.

## What Players See

When players join, Minecraft should ask whether they want to download the server resource pack.

If they accept, Faithful 32x applies automatically for that server session.

Players still need Iris and a shader pack on their own computer for realistic lighting.
