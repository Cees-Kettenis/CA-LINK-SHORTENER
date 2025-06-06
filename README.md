
# CA-LINK-SHORTENER

A simple, dark-mode URL-shortening tool built with Vanilla JavaScript and SheetJS (XLSX.js).This web app lets you upload an Excel file (with `url`, `alias`, and `tinyurl` headers), automatically hits the TinyURL API to create or reuse links, logs the results in a scrollable console, and then downloads a new Excel containing each row’s final `tinyurl`. It also provides a “Download Template” button to generate an empty Excel file with the correct headers.

> **Note:** You must supply your own TinyURL API key in `index.html` before using this tool.

---

## Features

- **Dark-mode UI** — a sleek, black/dark-gray theme that’s easy on the eyes.
- **Excel Template Generator** — one-click “Download Template” to get an empty `.xlsx` file pre-populated with `url`, `alias`, and `tinyurl` headers.
- **Excel Upload & Processing** — drag & drop (or file selector) to pick any `.xls`/`.xlsx` containing URLs you want to shorten.
- **Automatic TinyURL Integration**
  - Reuses existing aliases if they already exist on TinyURL.
  - Creates new TinyURLs via the [TinyURL API](https://api.tinyurl.com/) for new aliases.
- **Real-time Processing Logs** — live scrolling `<pre>` block shows which rows were skipped (already existed), created, or errored.
- **Automatic Download of Results** — after processing, the app builds a new `.xlsx` file containing each row’s final `tinyurl` and immediately downloads it.

---

## Prerequisites

- A modern web browser (Chrome, Firefox, Edge, Safari, etc.) with JavaScript enabled.
- Internet access (to call the TinyURL API).
- A valid [TinyURL API key](https://tinyurl.com/app/dev) (signup required).
- Basic knowledge of Excel: you’ll need to create or edit files with a header row.

---

## Installation

1. Clone or Download This Repository
   ```
   git clone https://github.com/cees-kettenis/ca-link-shortener.git
   cd ca-link-shortener
   ```
2. Open index.html in an editor and enter your API_KEY.
3. Open index.html in your browser.
