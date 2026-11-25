# PDF to PNG Converter

A single-file, offline PDF to PNG converter that runs in any modern web browser.

It was made for interactive whiteboards (for example Pardus smart boards), whose drawing apps save drawings as PDF instead of PNG. That makes the drawings hard to use as backgrounds or images.

## Features

- **No installation and no internet needed.** Everything, including the PDF engine, is inside one HTML file.
- **Cross-platform.** Works on Linux (Pardus, Ubuntu, …), Windows and macOS: anywhere Firefox or Chrome runs.
- **Multi-page and multiple files.** Every page becomes its own PNG.
- **Background options:** white, transparent, or *remove white background* (keeps only the drawing).
- **Quality options:** Normal, High or Very high resolution.
- Large, touch-friendly buttons for smart boards.

## Usage

1. Download or copy `pdf-to-png.html` to the computer or smart board.
2. Double-click it to open it in a browser. If it doesn't open, right-click → *Open with* → Firefox or Chrome.
3. Drag a PDF onto the page, or click **Choose PDF File**.
4. Click **Download PNG** or **Download All Pages**. Files go to the browser's Downloads folder.

To change a setting after converting, adjust it and click **Convert Again With Settings**.

## How it works

The page uses [PDF.js](https://mozilla.github.io/pdf.js/) (v3.11.174, legacy build) to render each page onto a canvas, then exports the canvas as PNG. The PDF.js library and its worker are embedded inline, so the file works straight from disk (`file://`) with no server.

## License

PDF.js is © Mozilla and contributors, licensed under the [Apache License 2.0](https://github.com/mozilla/pdf.js/blob/master/LICENSE).
