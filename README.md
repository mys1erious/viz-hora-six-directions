# HORA No.6: one watch, six art directions

One product hero for a fictional hand-wound watch, rendered in six art directions: Swiss poster, amber terminal, clay toy, 1-bit desktop, sumi ink and maison noir. The words are the same on every page. Each page opens with a circular wipe from its dial, and a 6-up grid zooms in and out. Every dial is drawn live in SVG, canvas or CSS, and there are no image files.

Reference post: https://x.com/okapi_fukugyo/status/2116337353904288234 (six AI-designed hero pages that avoid the generic look).

Open: serve this folder (`python3 -m http.server`) and load `index.html`. `?clean` hides the UI, `?play` runs the 25 s demo. Keys: arrows, 1-6, Esc for the grid. On touch: tap a tile, swipe between pages.

Re-record (server on 4330):
`node ../../../x-trend-ideas/_tools/record.mjs "http://127.0.0.1:4330/x-factory/builds/20261102-288234/?clean&play" video/hora-six-directions.mp4 --seconds 25 --fps 30 --w 1080 --h 1350 --warmup 3 --keys video/keys.json`
(`--warmup 3` gives the web fonts time to load; `keys.json` is the cursor path that hovers each button and taps each dial.) Poster: `ffmpeg -ss 0.4 -i video/hora-six-directions.mp4 -frames:v 1 video/poster.png`.
