# Java and Iris + Sodium

Iris is the shader loader. Sodium is the performance mod that helps Minecraft run better with modern rendering changes. The Iris installer can install both together for the normal Minecraft Launcher.

## Download Links

- [Iris installer](https://www.irisshaders.dev/download/)
- [Fabric installer](https://fabricmc.net/use/installer/)
- [Sodium on Modrinth](https://modrinth.com/mod/sodium)
- [Java download](https://www.java.com/download/)

Most players should start with the Iris installer because it is simpler than manually installing Fabric mods.

## Why Java May Be Needed on Windows

Minecraft includes its own Java runtime for launching the game, but that does not always help Windows open separate `.jar` installers.

If the Iris installer does not open when you double-click it, install Java for Windows, then try the Iris installer again.

You may also need to:

- Right-click the installer and choose Open.
- Right-click the installer, choose Properties, and click Unblock if Windows shows that option.
- Try the Windows `.exe` Iris installer instead of the universal `.jar`.

## Installing with the Iris Installer

1. Download the Iris installer from the official Iris page.
2. Run the installer.
3. Select Minecraft version `26.2`.
4. Choose the Minecraft Launcher install option.
5. Make sure Fabric mod support is enabled if the installer shows that option.
6. Click Install.

When the installer says `Completed`, the installation is finished. You can close the installer.

## Selecting the Correct Launcher Profile

Open the Minecraft Launcher after the install finishes.

The new profile may be named:

```text
Fabric Loader 26.2
```

That is expected. The launcher may show the Fabric profile name instead of `Iris & Sodium`.

Use that Fabric Loader 26.2 profile when you want to play with shaders.

## Confirming Iris Is Working

Launch Minecraft with the Fabric profile, then open:

```text
Options > Video Settings > Shader Packs
```

If the Shader Packs menu exists, Iris is installed correctly.

If the menu is missing, check that you launched the Fabric profile instead of the normal vanilla Minecraft profile.

## Manual Install Notes

Manual installs are possible, but they are more error-prone for new players.

Manual install basics:

1. Install Fabric Loader for Minecraft 26.2.
2. Download matching Iris and Sodium `.jar` files.
3. Put both `.jar` files in `%appdata%\.minecraft\mods`.
4. Launch the Fabric Loader 26.2 profile.

Do not put Iris, Sodium, or shader packs in the server folder. Iris and Sodium are client mods.
