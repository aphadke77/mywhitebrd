# WhiteBoard

A fully featured, single-file browser-based whiteboard application — no installation, no server, no dependencies to install. Just open `whiteboard.html` in your browser and start drawing.

---

## Features

### Drawing Tools

| Tool | Shortcut | Description |
|---|---|---|
| ✏️ Pen | `P` | Freehand drawing with smooth strokes |
| 🖊️ Highlighter | `H` | Semi-transparent overlay for emphasis |
| 🧹 Eraser | `E` | Erase parts of the canvas |
| 🔤 Text | `T` | Click anywhere to place and type text |
| 📝 Post-it | `N` | Drop draggable sticky notes on the board |

### Shapes

Click and drag to draw any of these:

- **Line** — straight line between two points
- **Rectangle** — outlined rectangle
- **Circle / Ellipse** — outlined ellipse
- **Arrow** — line with arrowhead

### Colour & Style

- 7 preset colour swatches (black, orange, blue, green, purple, red, amber)
- Custom colour via native colour picker
- **Brush size** slider — 1 to 40 px
- **Opacity** slider — 10% to 100%

### Post-it Notes

- 7 note colours: yellow, green, blue, red, purple, pink, white
- Colour palette appears in the toolbar when the Post-it tool is active
- Notes are **draggable** — grab the header bar and move them anywhere
- Each note has a subtle random rotation for a natural look
- Delete any note with the **✕** button on its header
- Post-its are **flattened into the canvas** when exporting to PNG or PDF

### History

- **Undo** — `Ctrl + Z`
- **Redo** — `Ctrl + Y`
- Full stroke-level history

### View Controls

- **Zoom In / Out** — `+` / `−` buttons in toolbar
- **Reset View** — returns canvas to 100% scale
- **Clear All** — 🗑️ button (asks for confirmation)

---

## Exporting

### Save as PNG

1. Click **⬇ PNG** in the top-right
2. Enter a file name
3. Click **Browse…** to choose a save folder (Chrome/Edge) — or leave blank to save to your default Downloads folder
4. Click **Save PNG**

### Save as PDF

1. Click **📄 Save as PDF** in the top-right (or `Ctrl + S`)
2. Configure options:
   - **File name**
   - **Save location** — Browse to pick a specific folder (Chrome/Edge)
   - **Page size** — A4, A3, US Letter, US Legal
   - **Orientation** — Landscape or Portrait
   - **Background** — White, Cream, or Transparent
3. Click **Export PDF**

> **Folder picker support:** The native OS save-location dialog (`showSaveFilePicker`) works in **Chrome and Edge**. In Firefox and Safari the file saves to the default Downloads folder automatically.

---

## Keyboard Shortcuts

| Shortcut | Action |
|---|---|
| `P` | Pen tool |
| `H` | Highlighter tool |
| `E` | Eraser tool |
| `T` | Text tool |
| `N` | Post-it tool |
| `Ctrl + Z` | Undo |
| `Ctrl + Y` | Redo |
| `Ctrl + S` | Open PDF export dialog |
| `Enter` | Commit text (while typing) |
| `Shift + Enter` | New line in text box |
| `Escape` | Cancel text input |

---

## Using the Text Tool

1. Select the **🔤 Text** tool or press `T`
2. Click anywhere on the canvas — a text input box appears at that position
3. Type your text; use **Shift + Enter** for multiple lines
4. Press **Enter** to stamp the text onto the canvas
5. Press **Escape** or click outside to cancel without committing

The text size follows the **Size** slider. The text colour follows the active colour swatch.

---

## Getting Started

No build step or server required.

```bash
# Simply open the file in your browser
open whiteboard.html          # macOS
start whiteboard.html         # Windows
xdg-open whiteboard.html      # Linux
```

Or drag and drop `whiteboard.html` directly into any modern browser window.

---

## Browser Compatibility

| Browser | Drawing | Post-its | Folder Picker |
|---|---|---|---|
| Chrome 86+ | ✅ | ✅ | ✅ |
| Edge 86+ | ✅ | ✅ | ✅ |
| Firefox | ✅ | ✅ | ⚠️ Downloads folder only |
| Safari | ✅ | ✅ | ⚠️ Downloads folder only |

---

## Dependencies

All dependencies are loaded from CDN — no `npm install` needed.

- **[jsPDF 2.5.1](https://github.com/parallax/jsPDF)** — PDF generation
- **[Syne](https://fonts.google.com/specimen/Syne)** — UI font (Google Fonts)
- **[DM Mono](https://fonts.google.com/specimen/DM+Mono)** — monospace labels (Google Fonts)

---

## File Structure

```
whiteboard.html    # The entire application — HTML, CSS, and JS in one file
README.md          # This file
```

---

## License

MIT — free to use, modify, and distribute.
