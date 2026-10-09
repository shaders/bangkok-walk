# Bangkok Walk

A guy in a yellow hoodie drags a red toy scooter on a rope through night Bangkok. Nothing happens. You just walk.

**Play:** https://shaders.github.io/bangkok-walk/

## Controls

- Hold anywhere on the screen (or any key) to walk. Release and he slows down — and so does the music.
- `M` or the speaker icon — mute.
- He smokes, drinks Chang and comments on the street by himself.

## What's in it

- 21 Bangkok districts in a fixed route: Sukhumvit, Silom (Soi 2, Soi 4), Sathorn, Lumpini, Siam, Erawan, Victory Monument, Yaowarat, Hua Lamphong, Khlong Toei, Grand Palace, Wat Pho, Khao San, Chao Phraya, Asiatique, night market, RCA, Thonglor, Nana, Soi Arab, Soi Cowboy.
- Stickman street life: kung fu, muay thai, karaoke, monks, elephants, drag queens, a coat guy selling fake Rolexes, a Gripen flyby.
- Day/night cycle, traffic lights, steps that knock the scooter over, procedural retrowave soundtrack (WebAudio, no audio files).

One self-contained `public/index.html`, no build, no dependencies.

## Debug URL params

- `?time=0600` — start at a given hour (`0600` dawn, `1200` day, `1800` dusk)
- `?seller=1` — coat seller shows up right away
- `?jet=1` — Gripen every 15 seconds
- `?autowalk=1` — walk without holding
- `?debug=1` — audio state overlay
