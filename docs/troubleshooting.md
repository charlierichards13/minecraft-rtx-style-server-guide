# Troubleshooting

## Iris Installer Does Nothing When Clicked

Install Adoptium Temurin 21 LTS for Windows x64, then try again:

- [Adoptium Temurin 21 LTS for Windows x64](https://adoptium.net/temurin/releases/?version=21&os=windows&arch=x64)

Java.com can still work as an alternate if needed:

- [Java.com download](https://www.java.com/download/)

Also try:

- Use the Windows `.exe` Iris installer.
- Right-click and choose Open.
- Right-click, choose Properties, and click Unblock if Windows shows that option.
- Check Task Manager for a stuck OpenJDK process.

## The Launcher Only Shows Fabric Loader, Not Iris

That is normal. The Minecraft Launcher may show:

```text
Fabric Loader 26.2
```

It may not say `Iris & Sodium`. Iris and Sodium are installed as Fabric mods under that profile.

Use the Fabric Loader 26.2 profile.

## The Shader Pack Does Not Show Up

Make sure the shader pack `.zip` is in:

```text
%appdata%\.minecraft\shaderpacks
```

Do not unzip the shader pack.

Also check:

- The file is still a `.zip`.
- The `.zip` is not inside another folder.
- You launched the Fabric profile.
- Iris is installed and the Shader Packs menu exists.

## The Server Resource Pack Looks Wrong or Did Not Apply

Go to:

```text
Multiplayer > Edit Server > Server Resource Packs
```

Set it to Prompt or Enabled.

Then rejoin the server and accept the pack prompt.

## My FPS Is Low

Lower:

- Shadow Distance
- Volumetric Lighting
- Reflections
- Render Distance

Recommended starting point:

- Render Distance: 8 to 12 chunks
- Simulation Distance: 5 to 8 chunks
- Motion Blur: Off
- Depth of Field: Off

If performance is still poor, switch from Complementary Unbound to Complementary Reimagined and use the Low or Medium shader profile.

## Shaders Work in Singleplayer but Not on the Server

Shaders are client-side. If shaders work in one world, they should also work when connected to a server unless a client setting changed.

Check:

- You launched the Fabric Loader 26.2 profile.
- The shader is still enabled in Video Settings.
- The server resource pack did not disable or conflict with another local resource pack.
- Your FPS did not drop so low that Minecraft appears frozen while loading.

## The Server Cannot Force RTX Lighting

Minecraft Java servers cannot force real shader lighting or ray tracing.

The server can push a resource pack and run datapacks. Real shader lighting comes from Iris and the shader pack on each player's computer.

## Datapack Is Not Working

For admins, check that the datapack is in:

```text
world/datapacks
```

Then run:

```text
/datapack list
```

If it is missing, confirm the datapack `.zip` is in the active world folder, not just the server root.
