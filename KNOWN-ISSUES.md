# Known issues

These directories are faithful snapshots of their source repositories, not repaired editions. Some source projects already referenced files or site routes that were absent at migration time.

The migration check found these unresolved local references:

- `templates/desktops/win98-homepage/index.html`: `/api/placeholder/80/80`, `/api/placeholder/16/16`, `/api/placeholder/24/24`
- `templates/profiles/fruitiger-aero/index.html`: `styles.css`, `pfp.png`, `floating1.gif`
- `templates/publishing/retro-newsroom/index.html`: `assets/retro-tv.png`, `assets/screenshots/screenshot1.png`, `assets/screenshots/screenshot2.png`, `assets/book-covers/book1.jpg`, `assets/book-covers/book2.jpg`, `assets/avatar.png`

Repeated references are listed once. An intentional `about:blank` iframe is not considered an error.

External fonts, images, iframes, and APIs may also disappear or behave differently over time. The preview images record how each template rendered during consolidation.

These findings were preserved rather than silently changing the original artifacts. See `provenance/quality-report.json` for machine-readable details.
