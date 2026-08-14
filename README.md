# PDF Page Studio

### Available at https://alekrutkowski.github.io/PDF-Page-Studio/

Upload multiple PDFs, then reorder, delete, copy, and move pages across output files. Download one output PDF, one merged PDF, or a ZIP containing all outputs.

All PDF processing runs locally in the browser. Files are not uploaded to a server.

## Export behavior

- Ordinary PDFs are copied losslessly, retaining vector graphics and selectable text.
- Permission-protected or otherwise non-copyable pages automatically use a rendered fallback so visible content is not exported as a blank page. Those fallback pages are flattened and their text is no longer selectable.
- The desktop interface requires an internet connection to load `pdf-lib` and PDF.js from cdnjs unless those libraries are hosted locally. The integrated mobile interface also loads JSZip from cdnjs for ZIP downloads.

## Usage

Open `index.html` directly, serve the repository with any static web server, or deploy it through GitHub Pages.

## Responsive interface

`index.html` contains both interface implementations. On a viewport no wider than 820 CSS pixels, or on a coarse-pointer device with a short landscape viewport, the page selects the touch-friendly mobile interface in place. There is no redirect to a second HTML page, so the GitHub Pages URL stays unchanged.

The mobile interface replaces drag-dependent actions with touch controls for selecting, reordering, moving, copying, splitting, deleting, and downloading pages.

Use `index.html?view=desktop` to keep the desktop interface on a small screen. Use `index.html?view=mobile` to force the mobile interface.

<img width="3330" height="2104" alt="PDF Page Studio interface" src="https://github.com/user-attachments/assets/92bdfc53-ed98-4727-9896-f8ca38d907b3" />

<img width="3312" height="2120" alt="PDF Page Studio page workspace" src="https://github.com/user-attachments/assets/b7d577e6-15ee-4bfd-81bc-6681bf1fd436" />
