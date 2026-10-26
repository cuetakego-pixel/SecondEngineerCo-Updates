# Second Engineer Co – app updates

Static update feeds (Sparkle appcasts) and installers for Second Engineer Co's free Mac apps.
Served by GitHub Pages at https://updates.secondengineerco.com (DNS: CNAME `updates` -> `cuetakego-pixel.github.io`).

One folder per app, containing `appcast.xml` and the installer files:

- `blankaudiosorter/` – Blank Audio Sorter

Each app's feed address is baked into the installed app, so keep these paths stable. Add a new app by adding a
new folder. Releases are published from each app's own project (`publish_update.sh`), which signs the installer
with the Sparkle EdDSA key in the Mac's Keychain and updates the folder here.
