# Bangkok Walk

A guy in a yellow hoodie drags a red toy scooter on a rope through night Bangkok. Nothing happens. You just walk.

**Play:** https://shaders.github.io/bangkok-walk/

## Controls

- Hold anywhere on the screen (or any key) to walk. Release and he slows down — and so does the music.
- `M` or the speaker icon — mute. The other corner buttons: auto-walk toggle, copy link, RU/EN language, restart, about.
- `Enter`/OK on TV remotes turns the sound on, then toggles it.
- He smokes, drinks Chang, spends money, gets into trouble and comments on the street by himself.

## What's in it

- 21 Bangkok districts in a fixed route: Sukhumvit, Silom (Soi 2, Soi 4), Sathorn, Lumpini, Siam, Erawan, Victory Monument, Yaowarat, Hua Lamphong, Khlong Toei, Grand Palace, Wat Pho, Khao San, Chao Phraya, Asiatique, night market, RCA, Thonglor, Nana, Soi Arab, Soi Cowboy.
- A quiet Riverside district (villas, sport club, crickets at night) and a trip to Hua Hin: train there, taxi (or minivan if broke) back.
- 16 more trips out of Bangkok: Ayutthaya, Chiang Mai, Doi Inthanon, Erawan, Isan, Kaeng Krachan, Kanchanaburi, Khao Yai, Ko Chang, Krabi, Lopburi, Nan, Pai, Pattaya, Phuket, Khao Sam Roi Yot. By plane, VIP double-decker, train, van, taxi, car ferry or motorbike over a mountain pass, with cutscenes on the way.
- Stickman street life: kung fu, muay thai, karaoke, monks, elephants, drag queens, a coat guy selling fake Rolexes, a Gripen flyby, selfie scenes.
- Money: ATMs with a 220-baht fee, police shakedowns, tuk-tuk / massage / food / girl / ping-pong offers, 7-Eleven, laundry, stuff thrown from windows.
- MRT stations and malls: up the escalator, along the deck, down again.
- Fate rolls (dogs, pigeons, pickpocket, rain, lotto…), achievements kept in `localStorage`, a monologue that depends on place, time and state.
- Day/night cycle, traffic lights, steps that knock the scooter over, procedural soundtrack per district (retrowave, techno, luk thung, mor lam, Chinese, Arabic, Thai classical; crickets and soft Mozart in Riverside). WebAudio, no audio files.
- Russian and English subtitles (`?lang=ru|en`, remembered in `localStorage`). Swearing is toned down unless `?18` is in the URL.

One self-contained `public/index.html`, no build, no dependencies.

## URL params

- `?18` — uncensored lines
- `?lang=en` / `?lang=ru` — subtitle language
- `?lite` or `?tv` — lighter audio for TVs and weak devices; `?scale=0.75` — render scale
- `?seed=123` — fixed world seed (any debug param below also fixes the seed)

## Debug URL params

- `?time=0600` — start at a given hour (`0600` dawn, `1200` day, `1800` dusk)
- `?seller=1` — coat seller shows up right away
- `?jet=1` — Gripen every 15 seconds
- `?autowalk=1` — walk without holding
- `?offer=seven|tuk|massage|food|girl` — force an offer
- `?fate=dogs|pigeon|splash|pickpocket|rain|window|scooter|pack|police|money|beer|monk|mango|lotto|girl` — force the first fate roll
- `?music=retro|techno|lukthung|morlam|china|arab|thai|riverside` — force a music genre
- `?mall=1` / `?mrt=1` — next structure is a mall / MRT station
- `?drop=1` — stuff falls from windows right away
- `?huahin=1` — Hua Hin trip comes early; `?trip=phuket` — force a trip by id (see list above, lowercase, no spaces)
- `?ride=ferry|moto|train` — force the transport; `?ride=30` — Hua Hin ride length
- `?happy=1` / `?happy=0` — massage cutscene variant; `?wx=rain` — rain in a few seconds
- `?debug=1` — audio state overlay
