Uses the decoding power from the Originial DCExtractor TMG-DCExtractor-Atlamillia was tested to work on DC1 i'm not sure if it works on DC2 sincei donthave it.

This version fixed the issue the previous version had when it came to exporting animations and rigged models.
All models will be exportedin GLB format with the animations and textures.

This program does have some issues andisn't perfect. its like 98% perfect.  It will extract every model and animated mesh from the game. which  includes Characters houses, and effects.
However the textures on some items may not load.
there is also a problem with some of the animations as the skeletons wouldnt follow the new formular. if you come in contact with an animation or skeleyton that is wonky move down to the next one if they're all wonky thats the breaks unfortunatly.

I cant fx it.

The same goes for textures, i tried my best to correct as many model textures as i could, howver DC1 has 2000-7000+ models and Im just one lady with a fussy baby time is not my friend. So please be understanding.

TMG-DCExtractor-Atlamillia
TMG-DCExtractor-Atlamillia is a user-friendly Dark Cloud model exporter built from DCExtractor. It focuses on one main workflow: scanning an extracted Dark Cloud folder and exporting textured, animated GLB files for use in tools such as Blender and Noesis.

This release is meant to make character model and animation extraction less painful, especially for batch exporting many models at once.

Features
Simple one-window GLB export UI
Batch scans an extracted game folder for .mds models
Exports textured .glb model files
Exports matching .mot animations into GLB when motion sets are available
Supports Dark Cloud character animation sidecars: .mot, .bbp, .wgt, and .cfg
Searches the full extracted game root, even if you choose a folder inside opdat
Includes a texture_packs fallback folder for known missing texture pages
Keeps all animations from a set together in one output folder per model
Includes quick buttons for Ko-fi and the original DCExtractor GitHub page
Download
Download the release zip and extract it somewhere outside your game extraction folder.

Run:

TMG-DCExtractor-Atlamillia.exe
The app includes the required DLLs and the texture_packs folder in the release zip. Keep those files next to the EXE.

Basic Use
Extract your Dark Cloud game files with DCExtractor or another compatible unpacking workflow.
Open TMG-DCExtractor-Atlamillia.exe.
Set Extracted game folder to the root of your extracted game folder.
Set Output folder to an empty or dedicated export folder.
Click Export GLB.
Wait for the progress log to finish.
Open the output folder and import the exported .glb files into Blender, Noesis, or another GLB-compatible tool.
For best results, choose the full extracted game root, for example:

Z:\Users\YourName\Downloads\Dark Cloud (USA)
The exporter can also recover if you select a folder inside opdat, but selecting the full root is still the clearest workflow.

Output Layout
The exporter creates one folder per model.

Example:

output
  01p17a
    01p17a1a.glb
    01p17a1b.glb
    01p17a2a.glb
  01p19a
    01p19a1a.glb
    01p19a1b.glb
    01p19a2a.glb
If a model has no matching animation set, it will still export as a static GLB when possible.

Texture Packs
Some fresh Dark Cloud extractions do not expose every texture page needed by certain models. The release includes a texture_packs folder with known-good texture pages for models that otherwise export with missing or incorrect textures.

The exporter searches for textures in this order:

The selected extracted game folder
A texture_packs folder inside the selected extracted game folder
The texture_packs folder next to the EXE
Texture matching is done by exact material name. This avoids broad fallbacks that can apply unrelated textures to the wrong model.

Do not delete the included texture_packs folder unless you know you do not need those fallback textures.

Notes
This tool exports assets from your own extracted game files. It does not include the game.
This is not a repacker and does not put files back into the original game archives.
Some unusual models may still need special handling.
GLB export is the main supported workflow in this version.
Credits
This project is based on DCExtractor by muddle12:

https://github.com/muddle12/DCExtractor

DCExtractor is a tool for unpacking and converting many file formats used by Level-5 PS2-era games, including Dark Cloud and Dark Cloud 2.

TMG-DCExtractor-Atlamillia builds on that work with a simplified GLB-focused interface, batch animation export fixes, texture fallback support, and quality-of-life improvements for Dark Cloud model extraction.

Support
If this tool helped you, you can support TheMightyGinkgo on Ko-fi:

https://ko-fi.com/themightyginkgo

License
This project is based on DCExtractor, which is licensed under the GPL-3.0 license. Keep the original license and source credit with any redistribution.

Disclaimer
This is a fan-made tool and is not affiliated with or endorsed by Level-5, Sony, or any rights holders. Dark Cloud and related names belong to their respective owners.
