# Troubleshooting

## Iris installer does nothing when clicked

Install Java 21 for Windows, then try again.

Also try:

- Right-click → Run as administrator
- Right-click → Properties → Unblock
- Check Task Manager for a stuck OpenJDK process

## The launcher only shows Fabric Loader, not Iris

That is normal. Iris and Sodium are installed as Fabric mods.

Use the Fabric Loader 26.2 profile.

## My shader pack does not show up

Make sure the shader pack `.zip` is in:

`%appdata%\.minecraft\shaderpacks`

Do not unzip the shader pack.

## The server resource pack looks wrong or did not apply

Go to:

Multiplayer → Edit Server → Server Resource Packs

Set it to Prompt or Enabled.

## My FPS is low

Lower:

- Shadow Distance
- Volumetric Lighting
- Reflections
- Render Distance

Recommended starting point:

- Render Distance: 8–12 chunks
- Simulation Distance: 5–8 chunks
- Motion Blur: Off
- Depth of Field: Off
