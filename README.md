# Manhwa Text-Checker

A small browser-based text formatter for manhwa typesetting workflows.

## Run locally
Open `index.html` in a modern browser. An internet connection is needed to load React, Babel, SweetAlert2, and Google Fonts from their CDNs.

## Publish with GitHub Pages
1. Create a GitHub repository (for example, `manhwa-text-checker`).
2. Upload `index.html` and `README.md` to the repository root.
3. Open **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Select the `main` branch and `/ (root)`, then Save.
6. Wait for GitHub Pages to provide your site URL.

## Features
- Two-pane original/result editor
- Paste from clipboard and copy checked text
- Import `.txt` and export UTF-8 `.txt`
- SweetAlert2 notifications
- Removes trailing spaces/tabs at the end of lines
- Adds one blank line after lines containing Thai characters
- Keeps English/Korean lines adjacent; existing repeated blank lines are normalized

## Notes about formatting
The checker treats each line containing Thai characters as a Thai line/sentence and adds a blank line after it. If a Thai sentence wraps across multiple lines, split/merge the text into one sentence per line before checking for the most predictable result. Text is processed locally in the browser; no text content is sent to a backend.
