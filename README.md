# ENHANCE Brain Health Study Website

Simple, accessible website for recruiting participants aged 60-80 to the ENHANCE brain health study.

## Quick Start

1. Open `index.html` in a web browser to view the site
2. The site works as a single HTML file - no build process needed
3. All images are in the `assets/` folder

## How to Update the Map

The map shows where ENHANCE is recruiting participants across the UK.

### Step 1: Update the Word Document

1. Open `assets/SitesUKMapWordDoc4FutureUpdates/Map_of_GP_locations.docx`
2. Add or remove sites as needed
3. Make sure site names use **large, readable text** (18-22pt minimum)
4. Save the document

### Step 2: Export to PNG

1. In Word, go to **File → Export → Export as PNG** (or take a high-quality screenshot)
2. Choose these settings:
   - **Width**: 1200-1600 pixels (important for mobile screens)
   - **Quality**: High or Best
3. Save as `UK-ENHANCE-map.png`
4. Place the file in the `assets/` folder

**Recommended PNG size**: 1200-1600px wide, under 500KB file size

### Step 3: Update the Site List in HTML

1. Open `index.html` in a text editor
2. Find the section starting with `<ul class="site-list">` (around line 360)
3. Update the list to match your map:

```html
<ul class="site-list">
  <li><strong>Site Name</strong><span>Postcode</span></li>
  <li><strong>Another Site</strong><span>Postcode</span></li>
  <!-- Add or remove sites as needed -->
</ul>
```

4. Save the file

### Step 4: Test

1. Open `index.html` in a web browser
2. Scroll to "Where we are recruiting"
3. Check that:
   - The map displays correctly
   - Text on the map is readable (test on a phone!)
   - The site list matches the map

## How to Update Contact Details

Contact information appears in two places on the website.

### Phone Number

Find and replace `020 8133 1990` with your actual number.

Also update the clickable link:
- Find: `tel:02081331990`
- Replace with: `tel:YOURNUMBER` (no spaces)

### SMS Number

Find and replace `07800 000000` with your actual SMS number.

### Email Address

Current email is `enhance@ucl.ac.uk` - update if needed.

Find and replace:
- `enhance@ucl.ac.uk` → your email
- `mailto:enhance@ucl.ac.uk` → `mailto:youremail`

## File Structure

```
enhance-webpage/
├── index.html                    # Main website (edit this)
├── coming-soon.html              # Placeholder for sign-up form
├── assets/
│   ├── UCL_lightBlue.png         # UCL logo
│   ├── NLFT.png                  # NHS Trust logo
│   ├── NIHR_Logos_Funded_01_Col_Corp_Blu_RGB.png  # NIHR logo
│   ├── Tablet_ENHANCE.jpg        # Tablet illustration
│   ├── OlderPeopleWithTablets.jpg # People photo
│   ├── UK-ENHANCE-map.png        # Site map (update this)
│   └── SitesUKMapWordDoc4FutureUpdates/
│       └── Map_of_GP_locations.docx  # Editable map source
└── sourcedocs/                   # Reference materials
```

## Publishing the Website

### Option 1: GitHub Pages (Recommended)

1. Commit your changes to git
2. Push to GitHub
3. Go to repository Settings → Pages
4. Select branch to deploy
5. Your site will be live at `https://username.github.io/enhance-webpage/`

### Option 2: Other Web Hosting

Upload these files to your web server:
- `index.html`
- `coming-soon.html`
- `assets/` folder (entire folder)

## Design Notes

- **Font size**: 18px base (17px on mobile) for readability
- **Colors**: Blue accent (#0f6a8d) with high contrast
- **Mobile-first**: All text and buttons sized for easy tapping
- **Accessibility**: Designed for older adults with potential vision/motor challenges

## Support

For questions about updating the website, contact the ENHANCE team.

Last updated: December 2025

