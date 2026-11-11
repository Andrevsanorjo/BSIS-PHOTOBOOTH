# BSIS Photo Booth

A responsive, browser-based BSIS maroon-themed photo booth.

## Run locally
1. Extract the ZIP.
2. Open a terminal in this folder.
3. Start a local server:
   - Python: `python -m http.server 8000`
   - Or use VS Code Live Server.
4. Visit `http://localhost:8000`.
5. Allow camera access.

Camera access generally requires HTTPS or localhost. Opening the HTML directly as a `file://` page may prevent camera access in some browsers.

## Included
- Responsive maroon/cream interface
- Browser camera preview and camera switching where supported
- Countdown and 3/4-photo capture
- Retake and clear controls
- Four fixed-size export templates
- Filters, background colors, captions
- PNG/JPEG downloads
- Local browser processing; no photo upload or server required

## Export dimensions
- Classic 3: 600 × 1800 px
- Classic 4: 600 × 2200 px
- Square collage: 1200 × 1200 px
- Two-column: 1200 × 1800 px

The preview is scaled with CSS while the canvas export retains the selected template's exact pixel dimensions.

## Notes
- Camera permissions and available resolutions depend on the browser and device.
- Photos are kept in the current page session only. Refreshing or closing the page clears the session.
- The current implementation is a client-side prototype; it does not include user accounts, a hosted event gallery, or QR-based retrieval.
