# inkwell-updates

The update channel for [Inkwell](https://www.inkwellnotes.com), a desktop note
taker for macOS and Windows. This repo is served by GitHub Pages at
<https://loganbradley787.github.io/inkwell-updates/>.

If you want to install Inkwell, go to
[inkwellnotes.com/download](https://www.inkwellnotes.com/download).

## What is here

- `latest.json` is the manifest the app's updater reads. `platforms` holds the
  update payload and signature for each OS; `installers` lists the files people
  download by hand.
- `inkwell-darwin-*.tar.gz` and the `.sig` files are updater payloads. The app
  checks each signature against a public key built into it before installing.
- `.dmg`, `.msi`, `-setup.exe`, `.AppImage`, `.deb` and `.rpm` are installers.
- `index.html` lists the current installers.

## How it is updated

The Inkwell release pipeline writes to this repo. Nothing here is edited by
hand, and a change to `latest.json` reaches every installed copy of the app, so
please do not open pull requests against it.
