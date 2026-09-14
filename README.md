# Roost

**All of Git on iOS. Free.**

Roost is a native Git client for iPhone and iPad. Clone, commit, push, branch, merge, and resolve conflicts without leaving the app. Repositories show up as folders in the Files app, and game-development files (Aseprite, textures, 3D models, audio, Unity and Godot scenes) preview in place.

- **Website:** https://singlecoregames.github.io/roost/
- **TestFlight beta:** coming soon <!-- TODO(REL-05): https://testflight.apple.com/join/XXXXXXXX -->
- **Bugs and feedback:** [Issues](https://github.com/singlecoregames/roost/issues)
- **Support:** https://singlecoregames.github.io/roost/support.html
- **Privacy policy:** https://singlecoregames.github.io/roost/privacy.html
- **Sample repository:** [singlecoregames/roost-data](https://github.com/singlecoregames/roost-data) — the Godot project used in the screenshots; clone it from the app with one tap, no sign-in needed

## Features

**Git**
- HTTPS tokens and SSH keys — GitHub and GitLab sign-in, personal access tokens, ed25519 and Secure Enclave keys, host-key fingerprint checks
- Clone from your GitHub, GitLab, Bitbucket, or Gitea account; shallow clones
- Branches, tags, and stashes; merge and rebase with a dedicated merge editor
- History graph with branch rails, merges, and tag chips; commit details and per-file history
- Unified and split diffs with syntax highlighting; image diffs

**Viewing and editing**
- Tree-sitter highlighting for 20+ languages, find in file, automatic reload on external changes
- Markdown preview with tap-to-toggle task checkboxes
- Search file names and contents; jump to function and type declarations
- Files app integration — edit in any app, commit in Roost
- Link an external folder (Logseq, for example) as a repository

**Game development files**
- Aseprite: layers, tags, frame timeline, playback, pixel-perfect zoom
- Images and textures: PNG, JPEG, HEIC, PSD, TGA, DDS, KTX2, EXR, SVG; per-channel view
- 3D models: glTF, GLB, USDZ, FBX, OBJ with normals, base color, and UV modes
- Audio and fonts: WAV and Ogg Vorbis waveforms with playback; font previews
- Unity and Godot: prefab and scene structure, Unity GUID lookup; GLSL, HLSL, and GDScript highlighting

**Platform**
- iPad: three-column layout, full keyboard shortcuts, multiple windows, Stage Manager
- Shortcuts, Home Screen widgets, Live Activities, Spotlight
- Four app palettes, four syntax themes, dark mode, Dynamic Type; English, Korean, Japanese
- Privacy: no data collection, no analytics, no account

## Beta

Roost is in beta. Keep a backup of any repository you can't afford to lose. The app collects nothing, and problem reports never include repository names, paths, or contents.

To report a problem, create a bundle in the app under **Settings → Support → Problem report**, then open an [issue](https://github.com/singlecoregames/roost/issues/new) and attach it. The bundle contains only device model, iOS and app version, app logs, and sync status.

## Q&A

**Will Roost be open source?**

It started out with open source in mind. But now that software is built with AI, publishing this much code gives people very little in return and mostly adds maintenance load, so it's on hold for now.

**Is it really completely free?**

Yes. There are no plans to monetize it. At most, there may be ways to support the developer that don't touch app features, such as a link to other apps or a tip jar.

## About this repository

This repository hosts the website (GitHub Pages) and the issue tracker. The app source is private.

Built with libgit2, libssh2, OpenSSL, Runestone, and other open-source software. Icons by Lucide (ISC).

© 2026 Singlecore Games
