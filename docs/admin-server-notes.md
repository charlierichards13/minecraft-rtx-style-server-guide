# Admin Server Notes

These notes are for server admins maintaining the documented Minecraft Java 26.2 visual stack.

## Confirmed Stack

Server side:

- Paper 26.2
- Dynamic Lights v1.9.3
- Faithful 32x hosted as a server resource pack through mc-packs

Client recommendation:

- Fabric Loader 26.2
- Iris + Sodium
- Complementary Unbound r5.8.1, or Complementary Reimagined for weaker PCs

## Server vs Client Responsibility

The server is responsible for:

- Hosting and prompting the Faithful 32x resource pack
- Loading the Dynamic Lights datapack
- Keeping the world and server configuration stable

Players are responsible for:

- Installing Iris + Sodium
- Adding Complementary Unbound or Reimagined to their local `shaderpacks` folder
- Enabling the shader in Video Settings

Minecraft Java shaders are client-side. The server cannot force shader lighting, ray tracing, or RTX-style effects.

## Dynamic Lights Datapack

Datapacks go in:

```text
world/datapacks
```

Confirmed install path:

```text
world/datapacks/dynamiclights-v1.9.3-mc1.17-26.2.9-datapack.zip
```

After updating or replacing the datapack:

1. Restart the server during a maintenance window, or run `/reload` if safe.
2. Run `/datapack list`.
3. Confirm the datapack is enabled.
4. Test a supported light item in-game.

## Server Resource Pack

Faithful 32x is hosted through mc-packs:

- [mc-packs resource pack hosting](https://mc-packs.net/)

The values are configured in `server.properties`.

Important fields:

```properties
resource-pack=
resource-pack-sha1=
require-resource-pack=false
resource-pack-prompt=
```

Recommended approach:

- Set `resource-pack` to the mc-packs URL.
- Set `resource-pack-sha1` to the matching SHA-1 value.
- Keep `require-resource-pack=false` unless the pack is mandatory.
- Use `resource-pack-prompt` to explain that Faithful 32x is the intended vanilla+ look.

## Updating the Resource Pack

When updating Faithful:

1. Download the new Faithful 32x Java pack from the official Faithful site.
2. Upload the new `.zip` to mc-packs.
3. Replace the old `resource-pack` URL in `server.properties`.
4. Replace the SHA-1 value if it changed.
5. Restart the server.
6. Join with a test client and accept the pack prompt.

Do not commit the Faithful `.zip` to this repository.

## Player Support Notes

Common player issues:

- Iris installer does not open: ask the player to install Java for Windows.
- Launcher only says Fabric Loader 26.2: that is normal.
- Shader pack does not appear: confirm the shader `.zip` stayed zipped and is in `%appdata%\.minecraft\shaderpacks`.
- Low FPS: recommend Complementary Reimagined and lower shadow distance first.

Point players to:

- [Player Quick Start](player-quick-start.md)
- [Troubleshooting](troubleshooting.md)
- [Performance Settings](performance-settings.md)
