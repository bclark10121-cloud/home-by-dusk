# Home by Dusk: backlog

Updated 2026-11-15. Brian decides the order. Pick ideas by number.

## Done

- v0.1.0 (first beta): one small level, the Dusk Hollow. Wren walks, runs, jumps, double jumps, rolls, climbs ledges and drops through wooden ledges.
- Two weapon slots and two ability slots, each on its own button. 20 weapons in 7 types and 20 abilities in 10 types, all data in `data/items.json`.
- Gear from four places: lying in the hollow, dropped by foes, in the secret chest behind the cracked wall and on Pip's cart at the end of the level. Full hands ask which slot to swap. The old item drops where you stand.
- Coins from foes and chests. Coins and keepsakes always stay.
- Energy instead of lives. Energy at zero, or Head home, ends the trip: gear back to the rusty sword. The door past the cart starts another run with your gear, new items and new stock.
- Three foes that telegraph: mossling (lunge), puffcap (hop), moth (swoop). Burn, slow, freeze, stun and root.
- Six keepsakes, one secret, a journal and personal records.
- Five save slots, the kit Settings with Camera, Foe hits (Normal, Gentle, None), Damage numbers and Ledge climb. Tester tools.
- Hero model made through the Claude, Gemini and Meshy workflow (front, side and back views, image to 3D, texture, remesh, rig).

## Now

- Render the Meshy model into the 48 x 48 hero sprite sheet and swap it in for the drawn Wren (same frame layout, `hero.json` keeps the hand positions).
- Brian's feel pass on jump height, run speed and the strike timings. The debug Feel tools switch them live.

## Asked for by Brian, not built yet

- G8.5 in `GAME_STANDARDS.md`: the Claude, Gemini and Meshy sprite workflow as a standard, after the hero is done.
- More levels after the feel is tuned. One level until then.

## Ideas to choose from (Brian picks by number)

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

## Later

- Real device check on a phone, a tablet, the Retroid and an Xbox controller (G7.10).
- Hit pause and more juice on strikes after the hero sprite swap.

## Not planned (they break the pillars)

- Bosses.
- Permanent death or losing coins and keepsakes.
- Cursed chests that kill on one hit. A gentle version is idea 9.
- Leaderboards or anything against other players.

## Decisions from Brian

- 2026-11-15: name Home by Dusk. The trip ends through the energy meter. Hybrid carry-over: coins and keepsakes stay, gear resets on the trip home. 2D pixel art in Godot 2D.
- 2026-11-15: two weapons and two abilities at once, support 20 of each, gear from secrets, foes and the merchant at the end of each level, foes drop coins, one small level until the gameplay is tuned, the player can jump, the hero through the Claude, Gemini and Meshy workflow.
- 2026-11-15: the Dead Cells files on Drive are the game's own files. Reference only. Nothing from them goes into this game.
