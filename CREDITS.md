# Credits

Home by Dusk is an original game. No personal names here (G1.11).

## Music (found through the Patch.gg asset library)

- "Grasslands" by Juhani Junkala, from JRPG Pack 1: Exploration. https://opengameart.org/content/jrpg-pack-1-exploration
  Licensed CC0 1.0 Universal. https://creativecommons.org/publicdomain/zero/1.0/
  Changes: re-encoded to Ogg Vorbis, loops.

## Made for this game

- Painted art (from v0.2.0): the scenery, props, foes, weapons, abilities, keepsakes, coin and ground textures were painted for this game with Google Gemini (an AI image tool) from original prompts and the hero's own reference art, then cut into game art by `tools/make_painted.py`. The source sheets are in `art_src/gemini/`.
- Hero model: made for this game from original reference art through Gemini (concept views) and Meshy (image to 3D, texture, remesh and rig). Rendered into sprites with Blender (`tools/wren/`).
- The sky, fog, glows, shadows and the icon layout: made in code (`tools/make_painted.py`, `tools/make_icon_master.py`).
- Every sound effect: a small synth in code (`tools/make_sounds.py`).

## Inspiration

- The run loop is inspired by Dead Cells (Motion Twin and Evil Empire). Ideas only. No art, sound, names, data or code from it (G8.4).

## Tools

- Godot Engine 4.6. https://godotengine.org (MIT licence)
- Blender (the bpy module). https://www.blender.org (GPL. Used as a tool only)
