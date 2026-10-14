Optional 3D models for Riftline
===============================

The game already builds detailed sci-fi props by itself (textured metal crates, ribbed pillars, piped walls,
grated platforms, window-lit buildings). If you would rather use your own models, drop a .glb file in this
folder with one of these names:

  crate.glb      pillar.glb      wall.glb      building.glb
  platform.glb   deck.glb        ceiling.glb

- Binary glTF (.glb) works best. To use .gltf or another path, edit CONFIG.models near the top of riftline/index.html.
- Size and origin do not matter. The game centres the model, sits it on the ground and stretches it to fill the
  object's collision box, so the look always matches where you can walk and shoot. Model a wall as a long thin slab,
  a pillar as a tall column, and so on.
- Any file that is missing is fine. That kind of object keeps the built-in look.
- Models are visual only. Collisions, hit detection and spawning never use them.
- Keep each file small (under about 2 MB, a few thousand triangles), because every player downloads them.
