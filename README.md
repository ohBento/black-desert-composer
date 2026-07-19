# Black Desert Composer — Releases

Public installers + auto-updater manifest for **Black Desert Composer**, a desktop app that turns MIDI and audio files into loadable Black Desert Online in-game music. The source repo is private; this repo only hosts the `.msi` installer and the updater's `latest.json`.

## Download

**[⬇ Download the latest version](https://github.com/ohBento/black-desert-composer/releases/latest)**

On the latest release page, download the file ending in **`.msi`** and run it. (The `.sig` and `latest.json` files next to it are for the auto-updater — you don't need them.)

Windows only — Windows 10 (version 1803+) or Windows 11. The WebView2 runtime installs automatically if it's missing. After the first install the app updates itself, so you won't need to come back here.

### Optional: audio stem separation

The Audio-to-MIDI converter works out of the box. To additionally split a song into per-instrument stems before transcription, install [Python](https://www.python.org/) and run `pip install demucs`. The app detects it automatically; without it, stem separation is simply skipped.

## For maintainers

Don't edit releases here by hand — they're published by the source repo's CI on every `v*` tag.
