# Dear Postcard – AR

AR postcards and stickers by Anamika Shrivastava. Scan the QR code, then point your phone at the card.

## Files

| File | What it does |
|---|---|
| `index.html` | The AR page people open from the QR code |
| `ar.js` | Every card's animation |
| `preview.html` | Plays each animation over its card image in a browser, no phone needed |
| `make-targets.html` | Builds `targets.mind`, the file that lets phones recognise the cards |
| `targets/` | One image per printed card or sticker (the names must match exactly) |
| `assets/` | Extra layers (the cat's hands) |

## Images that go in `targets/`

Already included: `torii-portrait.png`, `sticker-cat.png`, `sticker-fah.png`.

Export these from the Dear Postcard design canvas as PNG, use exactly these names, and upload them into `targets/`:

1. `moon.png` – Moon Confession front
2. `csmt.png` – CSMT Taxi front
3. `diwali.png` – Happy Diwali front
4. `christmas.png` – Merry Christmas front
5. `newyear.png` – Happy New Year front
6. `torii-landscape.png` – Sakura Torii landscape
7. `sticker-mumbai.png` – Made it to Mumbai sticker
8. `sticker-navi.png` – Made it to Navi Mumbai sticker

Each target image must be the same artwork that gets printed. If a design changes, re-export it and rebuild `targets.mind`.

## One-time setup

1. Upload everything in this folder to the repository: **Add file → Upload files → Commit changes**.
2. Upload the 8 exported PNGs into `targets/` the same way.
3. On a laptop, open `https://YOUR-USERNAME.github.io/dear-postcard-ar/make-targets.html`, wait until all 11 images show ✓, and click **Build targets.mind**.
4. Upload the downloaded `targets.mind` to the main folder of the repository.
5. On your phone, open `https://YOUR-USERNAME.github.io/dear-postcard-ar/`, tap **Start camera**, allow camera access and point it at a card.
