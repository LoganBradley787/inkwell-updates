# inkwell-updates

The update channel for [Inkwell](https://www.inkwellnotes.com), a desktop note
taker for macOS, Windows and Linux. This repo is served by GitHub Pages at
<https://loganbradley787.github.io/inkwell-updates/>.

If you want to install Inkwell, go to
[inkwellnotes.com/download](https://www.inkwellnotes.com/download).

## What is here

- `latest.json` is the manifest the app's updater reads. `platforms` holds the
  update payload and signature for each OS; `installers` lists the files people
  download by hand.
- `index.html` lists the current installers.
- The installers and update payloads themselves are attached to each
  [GitHub Release](https://github.com/LoganBradley787/inkwell-updates/releases)
  of this repo, starting with 2.0.2. The app checks each payload's signature
  against a public key built into it before installing.

## How it is updated

The Inkwell release pipeline writes to this repo. Nothing here is edited by
hand, and a change to `latest.json` reaches every installed copy of the app, so
please do not open pull requests against it.
