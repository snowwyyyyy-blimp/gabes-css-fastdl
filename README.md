# gabes-css-fastdl

FastDL content for the **Gabes little deathmatch!** CS:S server (Cloudflare Pages).

Used by the server via:

```
sv_downloadurl "https://gabes-css-fastdl.pages.dev/cstrike"
```

## Contents

| File | Purpose |
|---|---|
| `cstrike/sound/gabesmusic/roundmusic.mp3` | Round-start track (3s countdown + music, 90.65s) |
| `cstrike/sound/gabesmusic/roundmusic_loop.mp3` | Same track from 4s in, used if the round outlives the music |

Both are 44.1 kHz / 192 kbps CBR, which is what Source's sound mixer accepts.
48 kHz files fail on the client with `Invalid sample rate (0)`.

## Adding more custom content

Any file a client has to download must be mirrored here at the same path it
has on the game server, e.g. `cstrike/maps/my_map.bsp` for custom maps.
