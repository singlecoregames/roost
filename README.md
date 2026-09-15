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
- HTTPS tokens and SSH keys — Sign in with GitHub or GitLab, use a personal access token, or keep an SSH key in the Secure Enclave.
- Clone from your accounts — Pick a repository from your GitHub, GitLab, Bitbucket, or Gitea account and clone it. Large repositories can be cloned shallowly.
- Branches, tags, and stashes — Create and switch branches, push tags, and set work aside in a stash.
- Merge, rebase, and conflicts — Resolve conflicts in a dedicated editor by choosing a side for each hunk or editing it yourself.
- History graph — View branches, merges, and tags in the commit history, and follow the history of a single file.
- Diffs — Read changes unified or side by side, and compare images before and after.

**Viewing and editing**
- Code viewer and editor — View and edit code with syntax highlighting for over 20 languages. Files changed outside the app reload automatically.
- Markdown — Read Markdown rendered, and tick task checkboxes with a tap.
- Search and symbols — Search file names and contents, and jump straight to function and type declarations.
- Files app integration — Repositories appear as folders in the Files app. Edit files in compatible apps, then commit your changes in Roost.
- Link an external folder — Connect another app's folder, such as a Logseq graph, as a repository and commit in place.

**Game development files**
- Aseprite — Preview Aseprite files with animation playback, layers, and tags.
- Images and textures — Open textures such as PSD, TGA, DDS, KTX2, and EXR, and inspect them channel by channel.
- 3D models — Turn glTF, USDZ, FBX, and OBJ models around, and check normals and UVs.
- Audio and fonts — Play WAV and Ogg Vorbis files with a waveform view, and preview fonts.
- Unity, Godot, and shaders — Read the structure of Unity prefabs and Godot scenes, and view GLSL, HLSL, and GDScript with highlighting.

**Platform**
- iPad — Work in three columns on iPad, with keyboard shortcuts, multiple windows, and Stage Manager.
- Shortcuts, widgets, and Spotlight — Automate pull, push, and commit with Shortcuts, and see your repositories in widgets and Spotlight.
- Themes and languages — Choose an app palette and a syntax theme, with dark mode and Dynamic Type. Available in English, Korean, and Japanese.
- Privacy — No analytics or tracking. No separate Roost account required. Problem reports leave your device only when you send them.

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

Built with libgit2, libssh2, OpenSSL, Runestone, and other open-source software. Icons by Lucide (ISC). The full list with versions, licenses, and links: [Open-source software in Roost](OPEN-SOURCE.md).

© 2026 Singlecore Games
