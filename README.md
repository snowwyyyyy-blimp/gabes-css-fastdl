# gabes-css-fastdl

FastDL content for the **Gabes little deathmatch!** CS:S server.

Served by GitHub Pages, used via `sv_downloadurl`:

```
sv_downloadurl "https://snowwyyyyy-blimp.github.io/gabes-css-fastdl/cstrike"
```

## Contents

| File | Purpose |
|---|---|
| `cstrike/sound/gabesmusic/jingle.mp3` | Round-start track (3s countdown + music, 90.67s) |
| `cstrike/sound/gabesmusic/jingle_loop.mp3` | Same track starting at 4s, used if the round outlives the music |

## Adding more custom content

Any file a client has to download must be mirrored here at the same path it
has on the game server, e.g. `cstrike/maps/my_map.bsp` for custom maps.
