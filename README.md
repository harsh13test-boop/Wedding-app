# Wedding Guest Manager — iPhone Web App (PWA starter)

## What is included
- Marathi and English UI labels
- One guest per voice capture
- Guest fields: name, village, relationship, phone number
- Edit, delete, search, guest counts
- CSV export and share; Excel-compatible UTF-8 CSV
- Local browser storage and basic offline cache after first visit

## Important iPhone setup
This folder is a web app, not an App Store IPA. To install it on the iPhone Home Screen, it must be hosted at an HTTPS address.

### Simple hosting route
1. Upload the contents of this folder to a static HTTPS host (for example, a static site hosting service).
2. Open the published HTTPS link in Safari on the iPhone.
3. Tap Share -> Add to Home Screen -> Add.

## Voice input limitation
The app attempts to use the browser's Web Speech API for `mr-IN` or `en-IN`. iOS Safari support and Marathi availability can vary by iOS version, browser and region. If the app reports that speech recognition is unavailable, tap the microphone/dictation key on the iPhone keyboard while a text field is active and dictate the information. Always review recognized names and phone numbers before saving.

## Data and privacy
Guest records are stored in localStorage in the browser on that iPhone. They are not uploaded to a server by this starter. Clearing Safari website data can erase the list. Export the CSV regularly as a backup. Do not use private browsing for the guest list.

## Excel export
The export is CSV (not native XLSX). Microsoft Excel opens CSV files, and the file includes a UTF-8 BOM to help preserve Marathi characters.
