# Minecraft Monster Resource Pack

This repository hosts the public Minecraft server resource pack and editable source assets for custom monsters. It is separate from the user's other application repositories.

## Published pack

`MonsterPack.zip` is the compiled pack delivered by the Paper server to players over HTTPS.

- Download URL: https://raw.githubusercontent.com/Seonggun1206/minecraft-monster-resourcepack/main/MonsterPack.zip
- Current pack SHA-1: `17712c909e4facecd2caa09a4ae58b65767743c1`

The Paper server's `resource-pack` URL points to this file. After replacing it, update `resource-pack-sha1` in `server.properties` to the SHA-1 of the exact ZIP bytes.

## Source layout

- `source/monsters/<faction-or-species>/` — editable model, textures, RP Engine definitions, and source notes.
- `source/weapons/<family>/` — reserved for future custom weapon models and textures.
- `MonsterPack.zip` — compiled release consumed by the server.

New monsters should get their own source folder and texture atlas; do not overwrite vanilla textures. Keep server AI scripts in the server plugin project, separate from resource-pack assets. Custom drop tables and loot are not part of this pack.

## Current content

The first source asset is the Goblin Scout prototype. Its model and animation source is included under `source/monsters/goblins/`. The resource pack was compiled by RP Engine. Final in-game visual and animation verification is still pending.
