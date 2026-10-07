# PropertyLens AI

AI property condition form filler: photos + Google Maps data -> condition report.

## Run in VS Code
1. Unzip, then File > Open Folder and pick this folder.
2. Install the recommended **Live Server** extension.
3. Right-click `index.html` > **Open with Live Server** (http://127.0.0.1:5500).
4. Click **API Keys** and paste your Gemini key (https://aistudio.google.com/apikey) and Google Maps key.

## Google Maps key
Enable: Maps JavaScript, Geocoding, Places, Elevation, Maps Static, Street View Static.
Restrict the key to HTTP referrers `http://127.0.0.1:5500/*` and `http://localhost:5500/*`.

## Notes
- Keys live in the browser's localStorage. For public deployment, move the Gemini call to a backend. Free-tier Gemini may use prompts to improve Google products.
- Output is an AI-assisted draft. Low-confidence fields are flagged "Verify on site"; it does not replace a licensed inspection.
