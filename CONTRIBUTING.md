# Contributing

Thanks for helping! Bug reports, ideas and pull requests are all welcome.

## Reporting bugs
Open an issue using the **Bug report** template. Include browser, OS, GPU if known, and steps to reproduce.

## Pull requests
1. Fork the repo and create a branch: `git checkout -b feat/my-change`
2. Keep changes focused and small.
3. Test in at least one Chromium-based browser and one other browser if possible.
4. Do not edit vendored libraries (three.js, howler, lil-gui, Comlink) inside `index.html`.
5. If you touch terrain generation, update **both** the Web Worker copy and the fallback copy.
6. Do not add copyrighted assets you do not have the right to distribute.
7. Open the PR and fill in the template.

## Code style
Plain modern JavaScript, 2-space indentation, descriptive names.

By contributing you agree that your contributions are licensed under the MIT License.
