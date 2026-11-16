# Home by Dusk: backlog

Updated 2026-11-16. BC decides the order. Pick ideas by number.

## Done

- v0.5.0 (the whip in hand): stage 2 of the motion plan. Between strikes the whip hangs from Wren's hand as a coil and a short tail moved by rope physics. It hangs from her belt while she holds another weapon. A painted braided lash and wrapped grip from Gemini. A tip hit deals 6 in place of 4 (BC, 2026-11-16). The whip and its hit box stop at rock. Presses are remembered for 0.1 s. Hand spots on every frame of every move. A new headless `--whip` test.
- v0.4.0 (the whip and the run): stage 1 of the motion plan. The Leather Whip, drawn live on every screen frame, is Wren's main weapon. The rusty sword is the second weapon. The run has 16 frames at 30 a second with bigger swings, a bounce and a lean. A feel pass: steps follow speed, a softer start and stop, dust at each footfall and a pinch on a fast turn. A phone test page shows Wren drawn live in 3D with a frame counter.
- v0.3.0 (sound and strikes): fixed the silent browser builds. Three dark music tracks from Patch.gg with fades. Every strike redone with a wind-up, swing, follow-through and recovery (52 frames in place of 22), a gliding weapon, a swing streak, a hit pause and a motion for abilities. New tests for strikes and for real sound output.
- v0.2.0 (painted look): the whole game redrawn as a painted storybook in HD after BC found v0.1.0 too low in resolution. Gemini-painted scenery, props, foes and gear cut into game art by `tools/make_painted.py`. Wren's Meshy model shown at 192 pixel frames with an ink outline. Painted ground, a dusk forest in three misty rows, fog, glows, fireflies, smoke and soft shadows. A new painted icon.
- v0.2.0: a short gear list for the first releases. 4 weapons and 4 abilities drop and sell. The rest wait in the data and Tester tools.
- v0.1.0 (first beta): one small level, the Dusk Hollow. Wren walks, runs, jumps, double jumps, rolls, climbs ledges and drops through wooden ledges.
- Two weapon slots and two ability slots, each on its own button. 20 weapons in 7 types and 20 abilities in 10 types, all data in `data/items.json`.
- Gear from four places: lying in the hollow, dropped by foes, in the secret chest behind the cracked wall and on Pip's cart at the end of the level. Full hands ask which slot to swap. The old item drops where you stand.
- Coins from foes and chests. Coins and keepsakes always stay.
- Energy instead of lives. Energy at zero, or Head home, ends the trip: gear back to the rusty sword. The door past the cart starts another run with your gear, new items and new stock.
- Three foes that telegraph: mossling (lunge), puffcap (hop), moth (swoop). Burn, slow, freeze, stun and root.
- Six keepsakes, one secret, a journal and personal records.
- Five save slots, the kit Settings with Camera, Foe hits (Normal, Gentle, None), Damage numbers and Ledge climb. Tester tools.
- Hero made through the Claude, Gemini and Meshy workflow (front, side and back views, image to 3D, texture, remesh, rig), rendered into 57 pixel art frames: run from Meshy's run clip, every other move posed on its skeleton.
- G8.5 added to the standards: the sprite workflow.

## Now

- BC's numbers from the phone test page (https://bclark10121-cloud.github.io/home-by-dusk/live3d-test/): the three Result lines. They pick stage 3 of the motion plan: more sprite frames, or Wren drawn live in 3D.
- BC's feel pass on the whip: reach (4 tiles), wind-up speed, hold to repeat and the crack sound.
- BC's look at the whip in hand (v0.5.0): the coil, the tail, the belt during sword swings and the painted leather. Too lively, too still, too long or too short?
- BC's feel pass on the tip bonus (6 in place of 4, the last quarter of the reach) and the 0.1 s button memory.
- BC's look at the new run, lean and dust at full speed.
- BC's pass on the other strikes: which weapons still feel stiff, and whether the hit pause is the right length.
- BC's listen to the three dark music tracks. Swap any by naming the mood you want.
- Keep the dark, spooky mood in everything new (BC, 2026-11-15).
- BC's look pass on the painted art: anything that reads wrong, too dark, too busy or too soft.
- BC's feel pass on jump height, run speed, starts and stops and the strike timings. The debug Feel tools switch them live.
- A speed check on a real phone. The HD art is heavier to draw than the pixel art was.

## Asked for by BC, not built yet

- More levels after the feel is tuned. One level until then.

## Ideas to choose from (BC picks by number)

From the Dead Cells review, reshaped for a calm game:

1. Keepsake doors. Each keepsake opens a small new path for good, the way runes open new routes. The owl feather could give a wall jump, the iron key opens a locked gate.
2. Blueprints. Rare foes drop a sketch of a new weapon or ability. Bring it home and it can show up on later trips. The set of gear grows over time.
3. Pip's workbench at home. Spend coins between trips on lasting upgrades: a bigger energy bar, a third ability slot, tea that heals more, a lantern that shows secrets.
4. Gear levels. Items roll a tier (plain, fine, fancy) with more damage or a bonus effect. Higher runs roll better gear.
5. Scrolls of courage. A few hidden scrolls per run raise energy or damage for that trip only.
6. Charms. Pick one of three small passive perks at the cart each run, such as coins pull from farther away or rolls leave a spark.
7. Choose one of three. A shrine in a hidden room offers three items, you keep one.
8. Dusk doors. A door that stays open if you reach it within a few minutes. Behind it: coins and a better item. Never a penalty for missing it.
9. Calm streak rooms. Clear a small room without being touched for a bonus chest. Failing costs nothing.
10. Elite foes. A glowing foe carries an item and more coins. Still low risk.
11. A minimap and a journal map that fills in as you explore, with marks for found secrets.
12. Shuffled rooms. The level is built from handmade rooms in a new order each run, as Dead Cells mixes handmade tiles with a generated layout.
13. A second biome reached through the door after a few runs (after the feel is tuned).
14. Outfits for Wren bought with coins. Looks only.
15. A Christmas theme toggle (G4.5).
16. Daily walk. One fixed seed per day with a personal best for coins gathered.

## Unfinished standards items (2026-11-15)

From the Open items in `STANDARDS_OVERRIDES.md`, plus what has not been tried on a real device. Each line comes off when it is done. BC picks when.

- E5.4: touch buttons are 84 to 124 pixels across at 1280 x 720. Try them on a small phone.
- E6.5: time how long a browser save takes to reach the browser store on a real phone.
- E1.3: the main loop, the HUD and the effects run each frame while playing. Check on a phone whether any of them needs to sleep.
- E3.3: the 2D sprites are stored lossless (about 30 MB of textures). Check on a low memory phone.
- Real device check: the speed of the HD art on a real phone, a tablet, the Retroid and an Xbox controller. The test browser drew 3 to 4 frames a second.

## Later

- Whip, more ideas: a soft trail on the tip during the crack, a coil that unrolls into the wind-up in place of a quick swap, aim it up and at a slant, swing from hooks, pull small items toward Wren and wrap a foe to hold it for a moment.
- Start, stop and turn frames for Wren, and more jump, fall and land frames (stage 3, if the phone test says stay on pictures).
- Strikes, next steps if they still feel stiff: leg and hip movement in each swing, a painted smear frame at the fastest point, a short dash step on the combo finisher, strike sounds matched to each weapon type, and run and jump strikes with their own poses.
- Ambient sound for the hollow: wind in the pines, an owl, creaking branches and the torch crackle.
- More spooky touches in the art, for BC to pick from: thicker ground mist, bare twisted trees, will-o'-the-wisps, eyes that blink in the dark, crows on the arches, a pale moon and cobwebs in the hidden room.
- Real 2D lights with normal maps on Wren and the props, so torchlight falls on them. This release uses additive glows only.
- More animation in the painted art: foes have two painted poses each and move by squash and tilt. Paint more poses, or build them as cut-out puppets.
- Paint Pip a talk pose and a wave.
- A mossy stone edge for towers and ruins (strip B is already painted, see `art_src/gemini/README.md`).
- Sway on plants and trees in the wind.
- A higher detail render of Wren for close camera settings.
- Grow the release gear list as each weapon type gets its feel pass.
- Pose polish for the Meshy hero: a richer idle, a clearer climb and a bigger wind-up on heavy swings.
- Render Pip and the foes through the same Meshy workflow, one new element per release (BC, 2026-11-15).
- Real device check on a phone, a tablet, the Retroid and an Xbox controller (G7.10).
- Hit pause and more juice on strikes after the hero sprite swap.

## Not planned (they break the pillars)

- Bosses.
- Permanent death or losing coins and keepsakes.
- Cursed chests that kill on one hit. A gentle version is idea 9.
- Leaderboards or anything against other players.

## Decisions from BC

- 2026-11-15: name Home by Dusk. The trip ends through the energy meter. Hybrid carry-over: coins and keepsakes stay, gear resets on the trip home. 2D pixel art in Godot 2D.
- 2026-11-15: two weapons and two abilities at once, support 20 of each, gear from secrets, foes and the merchant at the end of each level, foes drop coins, one small level until the gameplay is tuned, the player can jump, the hero through the Claude, Gemini and Meshy workflow.
- 2026-11-15: the Dead Cells files on Drive are the game's own files. Reference only. Nothing from them goes into this game.
- 2026-11-15: v0.1.0 is too low in resolution. Back to design. Of five directions BC chose number 4, the painted storybook: Gemini-painted scenery and props, Wren rendered in HD to match.
- 2026-11-15: after v0.2.0, the next release adds music from Patch.gg and improves the motion of using weapons, which felt very stiff. BC heard no music in v0.2.0.
- 2026-11-15: keep a dark, spooky vibe to the game.
- 2026-11-15: after v0.3.0 the character's animation and the weapon still feel too stiff. Maybe switch to a whip as the main weapon. BC asked for a review with several agents on how to animate a whip and how to smooth the run and the movement.
- 2026-11-15: yes to both decisions from the motion review. Stage 1 ships as v0.4.0 (the whip as main weapon, the new run and the feel pass) and a separate phone test link shows Wren drawn live in 3D.
- 2026-11-15: always replace the Game Shelf picture with a new game picture on every release.
- 2026-11-15: keep the first releases to a small first level and limited weapons until the gameplay is in order. Keep every Gemini picture in the handoff zip for later use. Make only one of each element in Meshy per release.
- 2026-11-16: build stage 2 of the motion plan as v0.5.0. A tip hit deals 6 in place of 4.
