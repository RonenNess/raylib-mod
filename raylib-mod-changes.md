# Changes from original RayLib:

- Added camera near / far plane.
- Added mesh names to all common 3d formats.
- Added normals and tangets to batch rendering.
- Added options to render rectangles without changing textures.
- Added method to set depth offset (slope and constant).
- Added cylinder mesh generator around center instead of standing on 0,0,0 plane.
- Set support in jpg, bmp and tga by default.
- Added option to instance-render lines only.
- Added option to load OBJ model from memory.
- Added option to bind textures and set filter and wrap mode without immediately drawing them.
- Changed default max active textures to 16.
- Added option to bind texture to a specificl slot.
- Added more options to draw instanced meshes.
- Changed built-in model rendering methods to setup less things by default, which I didn't need for my pipeline. This may mess up rendering models with the built-in shaders.
- When loading gltf animations, if interpolation is not linear instead of letting data be corrupted and printing warning, changed behavior to still print warning but use linear interpolation anyway, so animation won't be completely broken.
- Added smooth model animation.
- Added method to clear model animations.
- Added method to draw mesh / model without prior setup.