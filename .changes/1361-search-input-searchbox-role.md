### Fixed

- **`@reticlehq/browser` — `<input type="search">` without `list` now computes role `searchbox` rather than `textbox`.** Per HTML-AAM, search inputs expose the `searchbox` role. `{ role: "searchbox" }` queries match it directly, interactive snapshots include it, and `{ role: "textbox" }` queries continue to match for backward compatibility with recorded flows. Closes [#1361](https://github.com/reticlehq/reticle/issues/1361).
