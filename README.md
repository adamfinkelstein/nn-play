# nn-play: a simplified Playground for COS 126

A trimmed copy of [A Neural Network Playground](https://github.com/tensorflow/playground)
for Princeton's COS 126 (Precept 19). Live at <https://adamfinkelstein.github.io/nn-play/>.

* Opens ready for the precept: XOR as four corner clusters (the `corners` dataset, as on
  the worksheet), sigmoid activation, learning rate 0.3, noise 5%, no hidden layers.
* Shows only play/reset, activation (ReLU, sigmoid, linear), hidden layers and neurons,
  the X1 and X2 features, and "Show test data". No header text, article, or analytics.
* Every hidden control can be shown again from the URL, e.g. `#noise_hide=false`, and any
  setting can be preset, e.g. `#noise=50&showTestData=true`.
* `npm ci && npm run build` builds `dist/`; pushing to the `cos126` branch publishes it.

The original README follows.

---

# Deep playground

Deep playground is an interactive visualization of neural networks, written in
TypeScript using d3.js. We use GitHub issues for tracking new requests and bugs.
Your feedback is highly appreciated!

**If you'd like to contribute, be sure to review the [contribution guidelines](CONTRIBUTING.md).**

## Development

To run the visualization locally, run:
- `npm i` to install dependencies
- `npm run build` to compile the app and place it in the `dist/` directory
- `npm run serve` to serve from the `dist/` directory and open a page on your browser.

For a fast edit-refresh cycle when developing run `npm run serve-watch`.
This will start an http server and automatically re-compile the TypeScript,
HTML and CSS files whenever they change.

## For owners
To push to production: `git subtree push --prefix dist origin gh-pages`.

This is not an official Google product.
