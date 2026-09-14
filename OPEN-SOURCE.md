# Open-source software in Roost

Roost is built on the projects below. The full license text of each is bundled in the app under **Settings → Support → Open-source licenses**. Versions are the ones shipped in the current beta.

## Git engine and networking

| Project | Version | License | Used for |
| --- | --- | --- | --- |
| [libgit2](https://libgit2.org) | 1.9.7 | GPLv2 with linking exception | Every Git operation: clone, fetch, push, merge, rebase, stash, diff |
| [libssh2](https://libssh2.org) | 1.11.1 | BSD-3-Clause | SSH transport for Git remotes |
| [OpenSSL](https://www.openssl.org) | 3.5.8 | Apache-2.0 | Crypto backend for libssh2 (HTTPS uses the system TLS stack) |

## Code viewing

| Project | Version | License | Used for |
| --- | --- | --- | --- |
| [Runestone](https://github.com/simonbs/Runestone) | 0.5.x | MIT | Code viewer with line numbers, wrapping, and find |
| [tree-sitter](https://tree-sitter.github.io/tree-sitter/) | 0.20.x | MIT | Incremental parsing behind syntax highlighting |
| [TreeSitterLanguages](https://github.com/simonbs/TreeSitterLanguages) | 0.1.x | MIT (per-grammar licenses included) | Grammars for 20+ languages, including Markdown |
| [tree-sitter-glsl](https://github.com/tree-sitter-grammars/tree-sitter-glsl) | 0.2.0 | MIT | GLSL shader highlighting |
| [tree-sitter-hlsl](https://github.com/tree-sitter-grammars/tree-sitter-hlsl) | 0.2.0 | MIT | HLSL shader highlighting |
| [tree-sitter-gdscript](https://github.com/PrestonKnopp/tree-sitter-gdscript) | 6.1.0 | MIT | GDScript highlighting |

## Game-development viewers

| Project | Version | License | Used for |
| --- | --- | --- | --- |
| [GLTFKit2](https://github.com/warrenm/GLTFKit2) | 0.5.15 | MIT | glTF and GLB model loading |
| [ufbx](https://github.com/ufbx/ufbx) | 0.23.0 | MIT / Unlicense | FBX model loading |
| [libogg](https://xiph.org/ogg/) | 1.3.6 | BSD-3-Clause | Ogg container for audio playback |
| [libvorbis](https://xiph.org/vorbis/) | 1.3.7 | BSD-3-Clause | Vorbis audio decoding |

The Aseprite viewer is an independent implementation written from the public [Aseprite file specification](https://github.com/aseprite/aseprite/blob/main/docs/ase-file-specs.md); it does not include Aseprite source code.

## Icons

| Project | Version | License | Used for |
| --- | --- | --- | --- |
| [Lucide](https://lucide.dev) | 1.39.0 | ISC | Repository icons and the website's feature icons |
| [Simple Icons](https://simpleicons.org) | 13.21.0 | CC0 1.0 | Brand icons for repository icons |

## Website

The website is static HTML on GitHub Pages with no third-party scripts, fonts, or analytics.
