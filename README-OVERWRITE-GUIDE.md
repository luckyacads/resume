# Lucky I. Ampalayohan — Digital Resume Refresh V3

This package is the third black-and-white portfolio revision. It keeps the monochrome interface/effects while preserving **all photographs and certificate images in full color**.

## V3 changes

- Simplified the hero so `DIGITAL RESUME` appears above **Lucky I. Ampalayohan** as the main heading.
- Removed the large slogan and metrics from the opening screen to reduce visual crowding.
- Kept the portrait in full color.
- Moved the `AUTOMATION` floating tag to the top of the portrait frame so it cannot cover the name or profile text.
- Kept `SOFTWARE` and `HARDWARE` as peripheral visual tags.
- Extended the timeline through the complete education history currently documented in the resume:
  - University of San Jose-Recoletos — BS Computer Engineering — 2021–2026
  - Mother Mary’s Children School — Junior & Senior High School — 2015–2021
  - Mother Mary’s Children School — Elementary — 2011–2015
  - St. Catherine’s College — Primary Education — 2010–2011
  - St. Cecilia’s College — Early Education / Kindergarten — 2007–2010
- Siemens S7-1500 certificate is now displayed in its original color.
- The OJT timeline continues to emphasize the Siemens PLC training and the Coursera `ChatGPT for Work: Productivity & Automation` course. The Coursera certificate remains marked as pending until it is available.

## Files to overwrite in the GitHub repository

Copy these into the root of the existing `luckyacads/resume` repository:

- `index.html`
- `styles.css`
- `script.js`
- `images/`

Keep the folder structure exactly as supplied.

## Local preview

Open the folder in VS Code and use **Live Server**, or run:

```bash
python -m http.server 8000
```

Then visit `http://localhost:8000`.

## Coursera certificate later

When the certificate arrives, add the image to `images/` and replace the pending Coursera credential block with the certificate image and, if available, its public verification link.
