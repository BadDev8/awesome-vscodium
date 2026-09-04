All of the following extensions are avaiable on OpenVSX.

# Python
- BasedPyright
- Kylin python
- Ruff

BasedPyright is used as the language server, providing errors, hints, hover info et cetera. Ruff is used formatter and linter, occasionally also giving errors.
Kylin python is useful to implement debugging inside vs code, while most of its functionality are disabled.
# Jupyter
- Jupyter (packet of 4 extensions)
- RenderPage PDF

Jupyter by microsoft is pretty much a must-go for jupyter notebooks in Codium. RenderPage PDF is useful to automatically create a .pdf from a .ipynb file.
# JavaScript
- Biome

Codium has an integrated language server for JS/TS, so the only needed extension is Biome fot linting and formatting. Note that biome works with .js and .ts files, but also with .html, .json, .jsonc, .css files aswell, providing complete support for web development.
# Web development
- Auto Close Tag
- Auto Rename Tag
- Live Server (Five Server)

Auto Close Tag and Auto Rename tag are useful extension for faster html 
writing, pretty self.explanatory.

Five server is a fork of the common extension Live Server to locally host a server in a one-click way, providing better support to real-time modifications than the original.
# C / C++
- clangdb
- CodeLLDB

Clangdb is an all-in-one formatter, linter and language server for C and C++. It's part of the LLVM project and based on the clang compiler, but can also support GCC. CodeLLDB adds to Codium the LLDB debugger, also part of the clang ecosystem. Note that you may change your snippets for the `launch.json` file to use the gdb debugger instead of LLDB. 
# Haskell
- Haskell
- Haskell Syntax Highlighting (dependent on Haskell but automatically installs it)

The simplest and most effective way to implement support to Haskell in Codium. Provides formatting, linting and all the useful language server functionalities.
# LaTeX
- Badnesss

Extensions that provides error, linting and formatting for $\LaTeX$ files. It also provides insanely good fast fixes, while being still early in development. But for compiled $\LaTeX$ in pdf you'll need
# PDF
- PDF Viewer

Very simple extension that allows Codium to render pdf files, fundamental for $\LaTeX$, but also useful for normal pdf usage. Does not integrate pdf editing (even though there are extension to do that, they are usually ether slow or with poor features).
# CSV
- Rainbow CSV

It colorizes elements of a CSV file based on their column, to semplify understanding of tables and data.
# Utilities
- Better Comments Next

Allow the user to write coloured and modified (bold, italic, underline) comments using tags.

- Better Todo Tree

Creates a new section in your sidebar to show all comments with certain tags [TODO, FIX, HACK, BUG, ...] to help in the organization of work.
- filesize

Show dimensions of a file in the status bar.
- P2P Live Share

Allows real time collaboration on the same projects (like google docs).
- PinBoard - Pin Files and Folders

Creates a section in the side bar for favourite / often used files. Particularly useful for taking notes or if you have bad memory (like real memory, not computer stuff).
- Project Manager

Allows to switch between projects incredibly fast.
- Minecraft Schematic Viewer

Allows Codium to render .schematic  and .litematic files.