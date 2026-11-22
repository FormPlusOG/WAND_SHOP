# The Wand Shop: magic mirror wand-testing station

A single web page (`index.html`) that turns an iPhone (or any device with a camera) into a magic mirror.
The child waves a stick with a coloured tip and leaves a glowing trail. The wand secretly "chooses" or
"rejects" them.

## Room setup

1. **The table.** Lay out three sticks, each with a bright coloured tip (red, blue, green tape or an LED).
   Print `wand-labels.html` and put a card beside each wand:
   - Red: *Dragon Heartstring, great for fireballs* (fire and embers)
   - Blue: *Phoenix Feather, master of lightning and ice* (lightning bolts and ice crystals)
   - Green: *Unicorn Mane, keeper of healing and leaves* (emerald leaves and stars)
2. **The mirror.** Prop the iPhone near the TV (landscape) and screen-mirror it to the TV (AirPlay).
   The child stands in front and sees themselves on the TV, mirrored.
3. **The magic.** Waving a wand leaves a glowing trail with sounds that react to speed.
4. **The wand chooses the wizard.**
   - The grown-up secretly sets which colour is "the one" (or leaves it on *Random*).
   - Wrong wand: after a moment of the wand "considering", grey smoke, a dull fizzle and
     "The wand does not choose you...".
   - Right wand: golden explosion, shockwave rings, light rays, chimes, floating runes and
     "The wand has chosen you!". Afterwards the wand keeps golden sparkles and runes while it is waved.
   - Next child? Triple-tap the hidden corner and tap **New wizard** to re-roll.

## Hidden grown-up controls

Triple-tap the **bottom-left corner** of the screen (or press **A** on a keyboard). The panel lets you:
choose the chosen colour (Random / Red / Green / Blue / Free play), re-roll, **force reject**,
switch front/rear camera, mirror on/off, sensitivity, **calibrate** each tip colour and show a debug view.
Settings are remembered on that device.

Keyboard shortcuts: Space force reject, N new wizard, Up/Down sensitivity, D debug, H hide status dot,
M mouse wand (1/2/3 pick colour), F full screen.

## Publish on GitHub Pages

1. Create a GitHub repository and add `index.html` (and `wand-labels.html`) to the root.
2. Repository **Settings -> Pages -> Build and deployment**: Source = *Deploy from a branch*,
   Branch = `main`, folder `/ (root)`. Save.
3. After a minute the site is live at `https://<your-username>.github.io/<repo-name>/`.
   GitHub Pages serves HTTPS, which iPhone Safari requires for camera access.
4. Open the link in Safari on the iPhone, tap **Rear camera** or **Front camera**, and allow camera access.

## iPhone tips

- Switch off the ring/silent switch and turn the volume up. The page also plays a silent loop so iOS lets
  the sounds through.
- Use landscape, and turn off rotation lock if needed.
- *Share -> Add to Home Screen* gives a full-screen view without Safari's toolbars.
- The screen is kept awake while the app runs.
- The rear camera has better quality. The picture is mirrored by default so it behaves like a mirror.

## Getting reliable tip detection

- Use **bright, saturated** colours (neon tape, glossy tape or tiny LEDs) and light the child's area well.
- Keep other saturated colours (red jumpers, green toys) out of frame.
- Run **Calibrate** for each colour in the grown-up panel: hold the tip in the circle for 3 seconds.
- If it misses tips, raise sensitivity. If it picks up the wrong things, lower it. The debug view shows what
  the tracker sees.
