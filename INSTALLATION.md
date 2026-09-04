# Installation
This guide assumes you already have installed Codium and fundamental system libraries on yuor system, like a file manager.

If you don't want a specific features, the easiest way to remove them is just by not installing the specific extension. Then you should, yet not need, to remove the respective setting of that extension from `setting.json`. The unused setting should never cause errors, as they should just be ignored by the editor, but this is still useful so that the configuration file remains clear and easy to read and modify.

First, go to the User directory in your VS Codium settings (on linux `~/.config/VSCodium/User`) and replace the respective files with those in the `User` directory of this repo. If you want to setup different keybinds, you can open the keybinds menu using `ctrl + k + ctrl + shift + s` of my configuration. I suggest you to look at the `keybinds.json` I gave so that you can find the names of keybinds faster, since Codium (and VS Code) are usually leave old keybind decommented, which makes a lot of mess.

Then open the editor and install the following extension. As I said, you can freely cherry pick between this list and still get a functioning editor. For more precise informations on what do the extensions do, see `EXTENSIONS.md`. All the extensions are avaiable on OpenVSX, which means you can install them directly from the integrated marketplace (`ctrl + shift + x`).

<span style="color:red">

- BasedPyright
- Kylin python
- Ruff
- Jupyter (packet of 4 extensions)
- RenderPage PDF
- Biome
- Auto Close Tag
- Auto Rename Tag
- Live Server (Five Server)
- clangdb
- CodeLLDB
- PDF Viewer
- Haskell
- Haskell Syntax Highlighting (dependent on Haskell but aytomatically installs it)
- Badnesss

</span><br>
<span style="color:blue">

- Rainbow CSV
- Better Comments Next
- Better Todo Tree
- filesize
- P2P Live Share
- PinBoard - Pin Files and Folders
- Project Manager
- Minecraft Schematic Viewer

</span>

The (red) first set of extensions are related to specific languages, while the remaining (blue) ones are utilities.

[//]: <> ( Woo I can do comments now )

These are instead themes I found good to use

- Monokai Dark+ (photos 1, 2, 3)
- vscode-icons (photos 1, 2, 3, 4)
- Dark Castle Theme  (photo 4)

After installing, you can edit `settings.json` to customize most of the extensions. Some of them, instead, have to be configured in another way

- Biome

Biome is a formatter for pretty much everything in the js ecosystem. When installed, the extension will ask you to also install Biome on your system, if you didn't have it yet. You can have a global `biome.json` configuration in you `~/.config/biome` directory (if `/biome` doesn't exist, you can create it). You may also have a configuration for each workspace, which is recommended by [the official documentation.](https://biomejs.dev/guides/configure-biome/)

- clangdb

Clangdb is an all-in-one formatter, linter and language server for c and c++. The only way to customize the formatting in using a .clang-format file in your workspace. In the global snippets you have installed there is a `clang-format` snippet with a minimal configuration that you can edit as you want. The usage of a snippet cuts time setting up a workspace.

- Debugging (Python / Node / CodeLLDB)

To debug natively in Codium you need to set up a `launch.json` file in the `.vscode` directory of your workspace (create the directory if it doesn' exist). Npm may create this file for you in electron / node.js projects, while for python and C/C++ projects you can create the file and then use the `debug-py`/`debug-c` snippets I setted up for you. You may obviusly edit this snippets as you please, insering custom arguments for the debugger.
