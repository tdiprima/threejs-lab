# Three.js Lab 🧙🏻‍♀️ 🪄

A collection of standalone [three.js](https://threejs.org/) experiments, mostly aimed at image viewing and annotation: drawing, measuring, selecting, zooming, and overlaying data on images.

Each demo is a single HTML file with no build step. Three.js (r160) and its addons are vendored in the repo.

## Running

Demos use absolute paths (`/build/...`, `/jsm/...`), so serve from the repo root:

```sh
python3 -m http.server 8000
```

Then open a demo, e.g. <http://localhost:8000/Code/ruler.html>.

A few demos also load libraries from a CDN (e.g. Leaflet in `three-leaf.html`), so they need a network connection.

## Demos

Everything lives in `Code/`.

| Topic | Files |
| --- | --- |
| Annotation | `annotation-simple.html`, `annotation-tools.html`, `annotations-house.html`, `editable-polygon.html`, `delete-and-edit-rect.html`, `hollow-brush.html`, `free-drawing/` |
| Measurement | `ruler.html`, `dynamic-ruler.html` |
| Selection and transforms | `select/`, `delete-cube.html`, `visibility-toggle.html` |
| Image handling | `bright-contrast.html`, `images-colorize.html`, `magnify.html`, `extract_pixels.html`, `multi-image.html`, `multi-image-controls.html`, `zoom-in-to-roi.html` |
| Labels and UI | `labels-canvas.html`, `labels-sprite.html`, `HUD.html`, `icons.html`, `gui-cube-camera.html`, `smallCameraView.html` |
| Performance | `draw-million-objects.html`, `level-of-detail.html`, `decimate.html` |
| Saving and loading | `serialize-deserialize.html`, `download.html` |
| Integrations | `three-leaf.html` (Leaflet), `cube-with-web-pages.html` (CSS3D), `charts/` (Chart.js, Gridstack) |
| Effects | `postprocess-play.html` |

`Code/threejs-template.js` is a starting point for new demos.

## Layout

| Path | Contents |
| --- | --- |
| `Code/` | Current demos |
| `archive/` | Older experiments and notes (cameras, geometry, shaders, OBJ loading, lazy loading) |
| `build/`, `jsm/` | Vendored three.js core and addons |
| `js/`, `css/`, `dat_gui/`, `es-module-shims-1.3.6/` | Other vendored libraries and styles |
| `images/`, `models/`, `fonts/`, `data/` | Assets used by the demos |

## License

[MIT](LICENSE)

This project includes third-party open-source code, which remains subject to its original licenses. Attribution is provided in the source code where applicable. If you believe there is a licensing issue, please open an issue.
