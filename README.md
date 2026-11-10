# Sparkle editor

A modified build of the [TurboWarp](https://turbowarp.org/) editor that opens with the Sparkle AI helper extension already loaded.

**Student link:** `https://ddabin2.github.io` (opens the editor with Sparkle)

## What was changed from TurboWarp

Built from [TurboWarp/scratch-gui](https://github.com/TurboWarp/scratch-gui) (branch `develop`, commit `96b9b34e741a77bca1de11ac2a7ffaf10ff20a3e`).

1. `src/containers/tw-security-manager.jsx`: the Sparkle extension URL `https://sparkle-1-1jho.onrender.com/extension.js` is added to the trusted list, so it loads without the sandbox.
2. `index.html` and `sparkle.html`: a start page that opens `editor.html?extension=<Sparkle extension URL>`. TurboWarp's original `index.html` (the project player) is kept as `player.html`.
3. The micro:bit firmware file is not included (replaced by a placeholder), so the micro:bit extension cannot flash firmware from this build.

The exact source changes are in `SPARKLE-CHANGES.diff`.

## License

TurboWarp's modifications to Scratch are licensed under the GNU General Public License v3.0. This build and the changes above are distributed under the same license. Source code: https://github.com/TurboWarp/scratch-gui plus `SPARKLE-CHANGES.diff`.

Scratch is a project of the Scratch Foundation. This site is not affiliated with, endorsed by, or sponsored by MIT or the Scratch Foundation, and the Scratch trademarks are property of MIT.
