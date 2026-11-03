# gabes-css-fastdl

FastDL content for the **Gabes little deathmatch!** CS:S server (Cloudflare Pages).

Used by the server via:

```
sv_downloadurl "https://gabes-css-fastdl.pages.dev/cstrike"
```

## Contents

| File | Purpose |
|---|---|
| `cstrike/sound/gabesmusic/countdown.wav` | 3 second countdown (0:00-0:03 of the track) |
| `cstrike/sound/gabesmusic/music.wav` | The music (0:03 to end, 87.6s) |

Both are 44.1 kHz mono PCM WAV. WAV on purpose:

- Source only accepts 11025/22050/44100 Hz - a 48 kHz file fails on the
  client with `Invalid sample rate (0)`.
- MP3 sounds are streamed with "no sound cache", which eats the first seconds
  of the file. That is why the countdown never played. WAV is cached, so it
  starts instantly.

## Adding more custom content

Any file a client has to download must be mirrored here at the same path it
has on the game server, e.g. `cstrike/maps/my_map.bsp` for custom maps.
