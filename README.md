# Deeptest-demo

A Chrome Extension (Manifest V3) project for **internal UI / architecture review and controlled development testing**.

## Project Overview

This repository contains a browser extension with:

* a **service worker** background script
* **content scripts**
* an **options page**
* a **settings page**
* bundled UI/assets and static rules

This README is intentionally limited to **safe development, installation, and project structure** documentation.

## Tech Stack

* **Chrome Extension Manifest V3**
* HTML / CSS / JavaScript
* Background service worker
* Content scripts
* Static assets and bundled chunks

## Project Structure

```text
Deeptest-demo/
├─ assets/                  # icons, fonts, styles, static assets
├─ chunks/                  # bundled JS chunks
├─ content-scripts/         # injected content scripts
├─ ui/                      # UI-specific frontend assets/styles
├─ background.js            # extension background service worker
├─ content-main.js          # main content script entry
├─ disclaimer.html          # disclaimer / informational page
├─ manifest.json            # Chrome extension manifest
├─ options.html             # extension options page
├─ rules.json               # declarative net request rules
└─ settings.html            # extension settings page
```

## Requirements

* Google Chrome or another Chromium-based browser
* Local access to this repository

## Installation (Developer Mode)

1. Clone or download this repository:

   ```bash
   git clone https://github.com/vanle1101/Deeptest-demo.git
   ```

2. Open Chrome and go to:

   ```text
   chrome://extensions
   ```

3. Enable **Developer mode**.

4. Click **Load unpacked**.

5. Select the project folder:

   ```text
   Deeptest-demo
   ```

6. The extension should now appear in your extensions list.

## Development Notes

* Update extension metadata in `manifest.json`
* UI pages can be edited in:

  * `options.html`
  * `settings.html`
  * files under `ui/`
* Background logic lives in:

  * `background.js`
* Content-side logic lives in:

  * `content-main.js`
  * `content-scripts/`

After making changes:

1. return to `chrome://extensions`
2. click **Reload** on the extension card

## Safe Review Scope

Recommended uses for this repo:

* reviewing extension structure
* refactoring UI
* renaming files and assets
* cleaning bundled output
* improving documentation
* preparing the project for legitimate internal testing workflows

## Version

Current manifest version:

* **2.6**

## Repository

GitHub:

* `https://github.com/vanle1101/Deeptest-demo`

## Disclaimer

This repository should only be used in **authorized, lawful, and controlled environments**.
Do not use browser extensions, automation, or network/request tooling against systems, forms, or services without explicit permission from the owner.

## License

Add your preferred license here, for example:

* MIT
* Apache-2.0
* Proprietary / Internal Use Only
