# Minecraft RTX-Style Server Guide

This repository documents a Minecraft Java 26.2 visual stack that creates an RTX-style, realistic lighting experience while keeping the game close to a vanilla+ Minecraft look.

It is documentation only. Do not upload shader packs, resource packs, datapacks, or other third-party `.zip` files to this repo. Players and server admins should download those files from the official pages linked below.

## Final Stack

Server:

- Paper 26.2
- Dynamic Lights v1.9.3 datapack
- Faithful 32x server resource pack

Client:

- Fabric Loader 26.2
- Iris + Sodium
- Complementary Unbound r5.8.1 shader pack

Lower-impact shader option:

- Complementary Reimagined

## Setup Levels

### Basic

Accept the server resource pack prompt when joining the server. This applies Faithful 32x and keeps the server's vanilla+ look, but it does not enable real shader lighting.

### Recommended

Install Iris + Sodium with Fabric Loader 26.2, then add Complementary Unbound r5.8.1 to the `shaderpacks` folder. This is the intended RTX-style setup with realistic lighting, shadows, bloom, water, and atmosphere.

### Lower-impact

Use the same Iris + Sodium setup, but choose Complementary Reimagined instead of Complementary Unbound. It keeps the visual upgrade while usually being easier on weaker PCs.

## Important Minecraft Java Note

Shaders in Minecraft Java are client-side. A server can push a resource pack, and a datapack can add server-side gameplay effects such as Dynamic Lights, but the server cannot force real shader lighting, path tracing, or RTX-style rendering for every player. Each player must install and enable shaders on their own client.

## Documentation

- [Player Quick Start](docs/player-quick-start.md)
- [Java and Iris + Sodium](docs/java-and-iris-sodium.md)
- [Complementary Unbound](docs/complementary-unbound.md)
- [Server-Side Setup](docs/server-side-setup.md)
- [Performance Settings](docs/performance-settings.md)
- [Troubleshooting](docs/troubleshooting.md)
- [Admin Server Notes](docs/admin-server-notes.md)

## Official Download Links

- [PaperMC downloads](https://papermc.io/downloads/)
- [Fabric installer](https://fabricmc.net/use/installer/)
- [Iris installer](https://www.irisshaders.dev/download/)
- [Sodium on Modrinth](https://modrinth.com/mod/sodium)
- [Complementary Shaders official site](https://www.complementary.dev/shaders/)
- [Complementary Unbound on Modrinth](https://modrinth.com/shader/complementary-unbound)
- [Complementary Reimagined on Modrinth](https://modrinth.com/shader/complementary-reimagined)
- [Faithful downloads](https://faithfulpack.net/downloads)
- [Tschipcraft Dynamic Lights on Modrinth](https://modrinth.com/datapack/dynamic-lights)
- [Tschipcraft's Dynamic Lights on CurseForge](https://www.curseforge.com/minecraft/data-packs/tschipcrafts-dynamic-lights)
- [Adoptium Temurin 21 LTS](https://adoptium.net/temurin/releases/?version=21&os=windows&arch=x64)
- [Java.com download](https://www.java.com/download/)
- [mc-packs resource pack hosting](https://mc-packs.net/)

## Repository Policy

This repository should store Markdown documentation, screenshots if needed, and small project-owned notes only. Do not commit:

- Shader pack `.zip` files
- Resource pack `.zip` files
- Datapack `.zip` files
- Rehosted third-party assets
- Copyrighted third-party pack contents
