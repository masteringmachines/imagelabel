# 🖼 ImageLabel

A zero-dependency, single-file image labeling tool that runs in any browser.  
Drop images in → classify, tag, and draw bounding boxes → export `labels.csv`.

## Quick start

```bash
# Just open the file — no server needed
open index.html       # macOS
start index.html      # Windows
xdg-open index.html   # Linux
```

## Features

| Feature | Detail |
|---|---|
| **Classification** | Single-select label per image (customisable) |
| **Multi-tags** | Any number of attribute tags per image |
| **Bounding boxes** | Draw, label, and delete boxes on the image |
| **CSV export** | One row per bounding box; one row per image if no boxes |
| **Keyboard shortcuts** | Fast navigation with arrow keys, number keys, `S`, `B`, `Del` |
| **Drag & drop** | Drop a folder of images straight onto the canvas |
| **Zero dependencies** | Pure HTML + CSS + JS, no install required |

## CSV format

```
filename, classification, tags, notes, bbox_index, bbox_label, bbox_x, bbox_y, bbox_w, bbox_h
```

Bounding box coordinates are **normalised (0–1)** relative to the image dimensions — compatible with YOLO, COCO, and most ML frameworks.

## Keyboard shortcuts

| Key | Action |
|---|---|
| `← →` | Previous / next image |
| `S` | Save & go to next |
| `1–9` | Quick classification by number |
| `B` | Switch to bounding box draw tool |
| `Esc` | Switch to select tool |
| `Del` | Delete selected bounding box |

## Requirements

Any modern browser (Chrome, Firefox, Safari, Edge). No internet connection needed after opening.
