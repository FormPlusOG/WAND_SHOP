# The Wand Shop: magic mirror wand-testing station (motion version)

A single web page (`index.html`) that turns an iPhone (or any device with a camera) into a magic mirror.
The child waves a stick and leaves a glowing trail of magic. The wand only **chooses the wizard** when they
trace the **secret movement**: a **figure 8** or a **zigzag**. Any other movement and the wand fizzles.

No colours or coloured tape are needed: the mirror follows whatever is *moving*.

## Room setup

1. **The table.** Lay out a few sticks with the printable cards from `wand-labels.html` (Dragon Heartstring,
   Phoenix Feather, Unicorn Mane). Any stick works, because the mirror follows the movement.
2. **The mirror.** Prop the iPhone up **so it cannot move** (a stand, a stack of books). Screen-mirror it to the
   TV (AirPlay). The child stands a few steps back so arm and wand fit in the picture, and sees themselves
   mirrored on the TV.
3. **The magic.** Waving leaves a glowing trail with sounds that react to speed. The magic style
   (fire, ice and lightning, or leaves) changes with each new wave. You can lock one in the grown-up panel.
4. **The wand chooses the wizard.**
   - The grown-up secretly picks the movement (Figure 8, Zigzag, Either, or Random for each new child).
   - Right movement: golden explosion, shockwave rings, light rays, chimes, floating runes and
     "The wand has chosen you!". Gold sparkles and runes keep floating while they wave.
   - Wrong movement: grey smoke, a sad "wah" and "The wand does not choose you...". This happens when they stop
     waving, or after about 5 seconds of waving the wrong way (and they can still win by then doing the right one).
   - Next child? Triple-tap the hidden corner and tap **New wizard**.

## What counts as the secret movement

- **Figure 8:** two smooth loops, one clockwise and one anticlockwise, any size, any tilt, any speed. About one and
  a half figure 8s is the sweet spot; a single one often works.
- **Zigzag:** at least four sharp back-and-forth strokes (like a lightning bolt or a row of mountains) that travel
  across the screen. A single "Z" (three strokes) doesn't count.
- Circles, straight waves, jabs, shaking side to side and wild scribbles don't count.
- A big wavy line can look like a zigzag to the mirror, so treat that as a possible "accident".

## Hidden grown-up controls

Triple-tap the **bottom-left corner** of the screen (or press **A** on a keyboard). You can:
choose the secret movement and re-roll, **Reveal** it (privately), force **Always choose** or **Always reject**,
choose the magic style, switch front/rear camera, flip the mirror, change motion sensitivity and show a debug view
of what the mirror sees. A tiny dot in the bottom-left corner turns grey when "Always reject" is on and white
when "Always choose" is on (hide it with **H** or in the panel).

Keyboard: Space always reject, G always choose, N new wizard, Up/Down sensitivity, D debug, H hide dot,
M mouse wand (draw the shape with the mouse to test), 0/1/2/3 magic style, F full screen.

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
- Use landscape. *Share -> Add to Home Screen* gives a full-screen view. The screen is kept awake while it runs.
- Keep the phone **completely still**. A moving camera looks like everything moving.

## Getting reliable tracking

- Good, even lighting and a plain background help. Avoid TVs, fans or other things moving behind the child.
- Only **one person** in the picture at a time, and make big, clear arm movements (a figure 8 about the size of a
  dinner plate or bigger).
- The mirror follows the moving "blob" (wand plus hand), not the exact wand tip, so use your whole arm rather than
  just wrist flicks.
- If it misses movements, raise **motion sensitivity** in the panel. If it follows the wrong things, lower it.
  The debug view (D) shows the movement the mirror sees.
- Not tested on real cameras yet: do a trial run with a few practice waves before the party, and adjust
  sensitivity as needed.
