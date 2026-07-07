# Player Quick Start

This page is for players who want to join the server and get the intended RTX-style look without learning every technical detail first.

## What You Need

Basic setup:

- Minecraft Java Edition 26.2
- The server resource pack enabled when you join

Recommended setup:

- Fabric Loader 26.2
- Iris + Sodium
- Complementary Unbound r5.8.1

Lower-performance setup:

- Fabric Loader 26.2
- Iris + Sodium
- Complementary Reimagined

## Step 1: Join the Server

When Minecraft asks whether you want to use the server resource pack, choose yes.

The server resource pack gives you the Faithful 32x texture look. It does not install shaders and it does not create real RTX lighting by itself.

If you skipped the prompt earlier:

1. Open Minecraft.
2. Go to Multiplayer.
3. Select the server.
4. Click Edit.
5. Set Server Resource Packs to Prompt or Enabled.
6. Join again.

## Step 2: Install Iris + Sodium

Download Iris from the official Iris page:

- [Iris installer](https://www.irisshaders.dev/download/)

Use the Iris installer for the Minecraft Launcher. It installs Iris and Sodium together.

On Windows, the Iris installer may need Java installed before it opens. If double-clicking the installer does nothing, install Adoptium Temurin 21 LTS for Windows x64 and try again:

- [Adoptium Temurin 21 LTS for Windows x64](https://adoptium.net/temurin/releases/?version=21&os=windows&arch=x64)

Java.com can still work as an alternate if needed:

- [Java.com download](https://www.java.com/download/)

When the Iris installer says `Completed`, the install is done. You can close the installer window.

## Step 3: Pick the Fabric Profile

Open the Minecraft Launcher and look for the new profile.

It may be named:

```text
Fabric Loader 26.2
```

That is normal. It may not say `Iris & Sodium`, even though Iris and Sodium were installed.

Launch Minecraft using the Fabric Loader 26.2 profile.

## Step 4: Add the Shader Pack

Download the shader from the official Complementary page or Modrinth:

- [Complementary Shaders official site](https://www.complementary.dev/shaders/)
- [Complementary Unbound on Modrinth](https://modrinth.com/shader/complementary-unbound)
- [Complementary Reimagined on Modrinth](https://modrinth.com/shader/complementary-reimagined)

Put the downloaded shader `.zip` file in:

```text
%appdata%\.minecraft\shaderpacks
```

Do not unzip shader packs. They stay zipped.

## Step 5: Enable the Shader

In Minecraft:

1. Go to Options.
2. Open Video Settings.
3. Open Shader Packs.
4. Select Complementary Unbound or Complementary Reimagined.
5. Click Apply.

If the shader does not appear, make sure the `.zip` file is directly inside the `shaderpacks` folder and not inside another folder.

## What the Server Can and Cannot Do

The server can:

- Ask players to use the Faithful 32x resource pack
- Run the Dynamic Lights datapack
- Provide a consistent vanilla+ art direction

The server cannot:

- Force players to install Iris
- Force players to enable shaders
- Force real shader lighting or ray tracing in Minecraft Java
- Make every PC run the same graphics settings

For weaker PCs, start with Complementary Reimagined and see [Performance Settings](performance-settings.md).
