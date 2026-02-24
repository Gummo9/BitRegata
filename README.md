# BitRegataStart

`BitRegataStart` is a lightweight start-line briefing tool for regatta race officers.

It focuses on:
- RC (Race Committee) -> Pin start line bearing
- Wind-only line vs compensated line
- Wind / current / wave visual schematic (no map)
- Mark 1 bearings and Rule 3 correction (numeric output)
- Estimated time to Mark 1 (fleet level factor + advanced multiplier + wave factor)

## Files

- `index.html` -> GitHub Pages entry point
- `bitregata.html` -> working copy (same app UI/logic)

## Run Locally

Open `index.html` in a browser.

## Publish on GitHub Pages

1. Create a GitHub repository (for example: `bitregatastart`)
2. Upload these files to the repository root:
   - `index.html`
   - `.nojekyll`
   - `README.md`
   - (optional) `bitregata.html`
3. In GitHub go to `Settings` -> `Pages`
4. Set:
   - `Source`: `Deploy from a branch`
   - `Branch`: `main`
   - `Folder`: `/ (root)`
5. Save

Your app will be available at:

`https://YOUR_USERNAME.github.io/bitregatastart/`

## Notes

- TWD is entered as wind direction **from**
- Current Set is entered as direction **to** (where current flows)
- Wave Direction is entered as direction **from** (where waves come from)
- Total start-line correction is computed as **current correction + wave correction**
- The diagram is schematic (not chart scale)
- RC = Race Committee (formerly CB / Committee Boat)
- `Bearing from RC corrected` is the operational RC reading derived from center-line bearing plus/minus Rule 3 correction
- `Mark 1 Time Multiplier` affects only estimated time to Mark 1 (it does not move Mark 1)
