# Credits

Home by Dusk is an original game. No personal names here (G1.11).

## Music (found through the Patch.gg asset library)

All three tracks are by Juhani Junkala, from JRPG Pack 3: Evil. https://opengameart.org/content/jrpg-pack-3-evil
Licensed CC0 1.0 Universal. https://creativecommons.org/publicdomain/zero/1.0/
Changes to each: re-encoded to Ogg Vorbis at 32 kHz and about 96 kbps, loudness matched, loops.

- "Whispers from beyond". Plays on the title card.
- "Witch's lair". Plays in the hollow.
- "Catacombs". Plays at Pip's cart.

v0.1.0 and v0.2.0 carried "Grasslands" by the same maker (JRPG Pack 1: Exploration, CC0). It is no longer in the game.

## Made for this game

- Painted art (from v0.2.0): the scenery, props, foes, weapons, abilities, keepsakes, coin, ground textures and the whip leather (v0.5.0) were painted for this game with Google Gemini (an AI image tool) from original prompts and the hero's own reference art, then cut into game art by `tools/make_painted.py`. The source sheets are in `art_src/gemini/`.
- Animation clips (from v0.6.0): Wren's idle, jumps, landing, hit and pick up, and the mixes for her start, stop and turn, use clips from KayKit Character Animations 1.1 by Kay Lousberg (www.kaylousberg.com), CC0. Credit is not required. The clips were copied onto Wren's skeleton and rendered to pictures. `tools/wren/kaykit/` in the private source holds the files and their licence.
- Hero model: made for this game from original reference art through Gemini (concept views) and Meshy (image to 3D, texture, remesh and rig). Rendered into sprites with Blender (`tools/wren/`).
- The sky, fog, glows, shadows and the icon layout: made in code (`tools/make_painted.py`, `tools/make_icon_master.py`).
- Every sound effect: a small synth in code (`tools/make_sounds.py`).

## Inspiration

- The run loop is inspired by Dead Cells (Motion Twin and Evil Empire). Ideas only. No art, sound, names, data or code from it (G8.4).

## Tools

- Godot Engine 4.6. https://godotengine.org (MIT licence)
- Blender (the bpy module). https://www.blender.org (GPL. Used as a tool only)
- Title font: Pirata One, SIL Open Font License 1.1. Start screen, game page and Game Shelf card name (G5.21 Title, 2026-11-18). License text in `FONT-LICENSE-PirataOne.txt`.
