# AD&D 1e Character Sheet for Owlbear Rodeo

Traditional white-paper, black-border AD&D 1st Edition character sheet, with Race/Class dropdowns and **two** class columns with separate levels and XP.

## Install

1. Upload the **contents of this folder** to a static HTTPS host (e.g. GitHub Pages, Netlify or Cloudflare Pages). The `manifest.json`, `index.html`, `app.js`, `style.css` and `icon.svg` must all be at the same public URL directory.
2. In Owlbear Rodeo, open the extension manager and choose to add a custom extension by URL.
3. Paste the publicly hosted **manifest.json URL**, such as `https://your-site.example/adnd-character-sheet/manifest.json`.
4. Open a room and click the **AD&D Character Sheet** extension action.
5. Select a token on the CHARACTER layer from the dropdown, edit its sheet, then click **Save to Token**. Changes are also automatically saved shortly after edits to a linked token.

## Features

- Traditional paper look, bold black borders, printable layout.
- Race, alignment, and two class dropdowns (Class 2 may be None).
- Separate level and XP fields for each class; supports Fighter/Magic-User and other multiclass combinations.
- All six attributes, exceptional strength, descending AC, HP, THAC0, five AD&D saving throws.
- Weapons, class abilities, spells, equipment, coins, notes.
- Data stored in Owlbear Rodeo **scene item metadata** on the selected token, shared according to scene access. **Do not store secret player notes in token sheets**.
- JSON import/export as portable backups.

## Limitations

- This is a manually editable character sheet, **not** a rules engine. It does not automatically calculate class progression, saves, legal race/class combinations, multiclass HP or spell slots.
- Sheets live on tokens **in a particular scene**. If you delete a token, its attached sheet is deleted with it. Export JSON regularly; copying a token to another scene may preserve metadata depending on the copy operation.
- An unlinked draft is not persistent. Export it or select a token and save.
- Requires Owlbear Rodeo 2.x, an open scene and an internet connection to load the Owlbear SDK from esm.sh.
- This release is not yet verified by a live Owlbear Rodeo installation.

## Files

`manifest.json` is the extension entry point. `index.html` and `style.css` render the sheet; `app.js` uses the Owlbear Rodeo SDK to read/write token metadata.
