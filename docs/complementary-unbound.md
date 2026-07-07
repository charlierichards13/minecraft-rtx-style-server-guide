# Complementary Unbound

Complementary Unbound r5.8.1 is the recommended shader pack for the full RTX-style look in this guide.

It adds realistic lighting, shadows, bloom, reflections, improved water, atmospheric skies, and stronger night mood while still keeping Minecraft recognizable.

## Download Links

- [Complementary Shaders official site](https://www.complementary.dev/shaders/)
- [Complementary Unbound on Modrinth](https://modrinth.com/shader/complementary-unbound)
- [Complementary Reimagined on Modrinth](https://modrinth.com/shader/complementary-reimagined)

Download shader packs only from official sources. Do not copy shader `.zip` files into this repository.

## Install Location

Shader packs stay zipped.

Put the Complementary Unbound `.zip` file in:

```text
%appdata%\.minecraft\shaderpacks
```

Do not unzip it. Iris reads the shader pack directly from the `.zip`.

## Enable the Shader

1. Launch Minecraft with the Fabric Loader 26.2 profile.
2. Open Options.
3. Open Video Settings.
4. Open Shader Packs.
5. Select Complementary Unbound.
6. Click Apply.

If the shader does not show up, click the button that opens the shaderpacks folder and confirm the `.zip` file is in that exact folder.

## Recommended Visual Direction

Use Complementary Unbound when you want:

- The most realistic lighting in this stack
- Stronger shadows and glow
- Better water and reflections
- A more cinematic night atmosphere
- The closest Java Edition version of an RTX-style presentation

Use Complementary Reimagined when you want:

- Better performance
- A look closer to vanilla Minecraft
- Less intense lighting
- A safer option for laptops and older PCs

## Good Starting Settings

Start with a medium preset, then adjust based on FPS.

Recommended first pass:

- Shader profile: Medium or High
- Shadow Distance: 8 to 12 chunks
- Render Distance: 8 to 12 chunks
- Simulation Distance: 5 to 8 chunks
- Motion Blur: Off
- Depth of Field: Off
- Bloom: On, but reduce it if bright areas feel too strong
- Reflections: Medium or Low on weaker GPUs
- Volumetric Lighting: Low or Medium

If Minecraft feels choppy, lower Shadow Distance first. Shadows are one of the biggest performance costs.

## Server Limitation

Complementary Unbound is a client-side shader pack. The server cannot install or force it for players.

The server can provide Faithful 32x as a resource pack and run Dynamic Lights as a datapack, but real shader lighting happens on each player's computer.
