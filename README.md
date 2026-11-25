# Mugi OS — first website build

A standalone static desktop inspired by cute retro Windows personal websites. No dependencies, accounts, or backend connection.

## Preview on Windows
Extract the ZIP into a NEW folder, separate from Mugi's World. Open a terminal in that folder and run `py -m http.server 8080` (or `python -m http.server 8080`). Open http://localhost:8080. Stop with Ctrl+C. Opening index.html directly also shows the built-in preview, but fetching the JSON may be blocked by the browser.

## GitHub Pages
Create a separate repository on your personal GitHub, upload the contents of this folder to its root, then Settings > Pages > Deploy from a branch > main / (root). The site uses relative URLs. No build step. Do not upload the private Mugi project or database.

## Customize
Replace assets/bear.svg and the seven icon SVGs with your own artwork (or change the paths in app.js). Edit style.css for wallpaper and colors. The current illustrations are original placeholders. Edit data/snapshot.json to publish deliberately selected data. Set published_at to the actual ISO timestamp and mode to published. Activity is a string or null; interests are strings; milestones contain date/title/text; research contains title/text; creations contain title/category/text and optional asset path under assets/. Categories: Drawings, Pixel art, Stories, Music. Use local public assets only. No automated exporter is included. All JSON is public, even fields not displayed. Never copy private letters, photos, tokens, database, internal addresses, or raw memory exports here.

API.exe shows views of the real static snapshot file, not live REST endpoints. The taskbar clock is the visitor's local time. Desktop windows support drag and native resize; mobile uses full-size windows. No live Mugi connection, no automated publication, no desktop pet yet.

## v0.2
Open index.html for the preview. Start menu > Desktop theme switches between strawberry plaid, classic blue and lavender. Mascot and profile artwork supplied by the creator. Music controls remain disabled until a published Music entry with a local assets/ audio file is available. No private backend connection. For loading edited snapshots locally use `python -m http.server 8080` and open http://localhost:8080.
