# PDF Page Studio

### Available at <https://alekrutkowski.github.io/PDF-Page-Studio/>

Upload multiple PDFs, then reorder, delete, copy, and move pages across output files. Download one output PDF, one merged PDF, or a ZIP containing all outputs.

All PDF processing runs locally in the browser. Files are not uploaded to a server.

## Export behavior

- Ordinary PDFs are copied losslessly, retaining vector graphics and selectable text.
- Permission-protected or otherwise non-copyable pages automatically use a rendered fallback so visible content is not exported as a blank page. Those fallback pages are flattened and their text is no longer selectable.
- The app requires an internet connection to load `pdf-lib` and PDF.js from cdnjs unless those libraries are hosted locally.

## Usage

Open `index.html` directly, serve the repository with any static web server, or deploy it through GitHub Pages.

<img width="3330" height="2104" alt="PDF Page Studio interface" src="https://github.com/user-attachments/assets/92bdfc53-ed98-4727-9896-f8ca38d907b3" />

<img width="3312" height="2120" alt="PDF Page Studio page workspace" src="https://github.com/user-attachments/assets/b7d577e6-15ee-4bfd-81bc-6681bf1fd436" />
