# NCYPT · 北卡青少年舞蹈团

A bilingual Chinese/English website inspired by the full-screen stage imagery, strong typography, and editorial layout of the Joffrey Ballet site. Original implementation; no Joffrey text, photography, branding, or JavaScript has been copied.

The project folder is **NCYTP**, as requested. The organization’s supplied Information document identifies its official name as **NC Youth Performance Team (NCYPT)**, which is used on the website.

## Run and deploy

```sh
npm run dev
# http://localhost:3002
npm run build
# static output: dist/
```

No package installation is required. Node 24+ is recommended. Import this project into Vercel with the included `vercel.json`: build command `npm run build`, output directory `dist`, Framework Preset Other. No database or serverless function is needed. Deploy only the built `dist/` directory on other static hosts; configure the five page routes to fall back to `index.html`.

## Pages and interactions

- Homepage: stage photography, introduction, performance highlights, dance education.
- `/about`: founding story, mission, team statistics, award-winning works and video links.
- `/performances`: annual recital playlists from 2023–2026 and community performance history.
- `/education`: ages 4–18, Sunday classes, 1–2 hours per class, Apex class address.
- `/gallery`: six selected real photos, category filters, keyboard-accessible image dialog.
- `/join`: contact information and a validated inquiry form that opens the visitor’s email app. Visitors must review and send the email themselves. No submissions or personal information are stored by the website.
- Chinese/English switch retained in localStorage; responsive mobile menu; reduced-motion support.

## Sources and editing

Source folder provided by the user: https://drive.google.com/drive/folders/1xzFoumK9PeIgHXFH0Jo7RqpBYowYurhN

Organization facts and links were transcribed from the supplied **Information** and **Awards** documents. Student/teacher counts refer to the 2026 source materials. The raw documents are not included in the public website. Personal residential registration details and tax identifiers were not used. No invented staff biographies, class prices, new event dates, or ticket availability have been added. The internal note about a potential future NBA collaboration has not been presented as a confirmed public event.

Six downloaded photos have been resized for web use:

- `recital-2026-01.jpg`: Photo2026Recital / Hui Yang / Copy of DSC_0390.JPG
- `recital-2026-02.jpg`: Photo2026Recital / Hui Yang / Copy of DSC_0410.JPG
- `recital-2026-03.jpg`: Photo2026Recital / Hui Yang / Copy of DSC_0430.JPG
- `studio-2026-01.jpg`: Photo2026RecitalInstudio / Ran Liu / Copy of IMG_6634.jpg
- `studio-2026-02.jpg`: Photo2026RecitalInstudio / Ran Liu / Copy of IMG_6651.jpg
- `studio-2026-03.jpg`: Photo2026RecitalInstudio / Ran Liu / Copy of IMG_6671.jpg

These are selected photographs, not a full export of every album. The separate `NCYPT.JPG` shortcut required additional access and was not used. Older recital cards use year artwork, avoiding mislabeling current photos as historical events.

Edit photo metadata and email in `public/content.js`, bilingual page copy in `public/app.js`, and the design in `public/styles.css`. Images live in `public/assets/`. The NCYPT wordmark is a text treatment, not an official logo supplied by the organization. This project has not been pushed to GitHub or publicly deployed.

## Verification

Verified locally: static build, page/deep-link HTTP responses, JavaScript syntax, language switching, gallery category filtering (three studio images), lightbox open/close, mobile menu, and no horizontal overflow at 390px. Inquiry email sending is intentionally left to the visitor’s mail application.
