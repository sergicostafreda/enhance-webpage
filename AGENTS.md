# ENHANCE Website - AI Agent Context

## Project Overview

Simple, accessible recruitment website for the ENHANCE brain health study. Target audience: adults aged 60-80, including those with lower digital literacy and potential sensory challenges.

## Key Design Principles

1. **Simplicity**: Single HTML file, no build process, minimal dependencies
2. **Accessibility**: Large text (18px base), high contrast, mobile-optimized
3. **Plain English**: Clear, friendly language avoiding medical jargon
4. **Trust**: Prominent NHS/UCL/NIHR logos, professional but warm tone

## Technical Stack

- **Pure HTML/CSS**: No JavaScript frameworks
- **Inline styles**: All CSS in `<style>` tag for portability
- **Responsive**: Mobile-first design with `clamp()` for fluid typography
- **File-based**: Works via `file://` protocol (no server required for testing)

## File Structure

```
/
├── index.html              # Main page (409 lines)
├── coming-soon.html        # Placeholder for sign-up form
├── assets/                 # All images
│   ├── UCL_lightBlue.png
│   ├── NLFT.png
│   ├── NIHR_Logos_Funded_01_Col_Corp_Blu_RGB.png
│   ├── Tablet_ENHANCE.jpg
│   ├── OlderPeopleWithTablets.jpg
│   ├── UK-ENHANCE-map.png  # Site map (needs creation)
│   └── SitesUKMapWordDoc4FutureUpdates/
│       └── Map_of_GP_locations.docx
└── sourcedocs/             # Reference materials (HOME trial examples, etc.)
```

## Content Sections (index.html)

1. **Hero** (lines 251-278): Logo, headline, CTA button, contact info
2. **What's Involved** (lines 280-317): Study details, benefits, randomization
3. **Image Section** (lines 319-323): Photo of older adults with tablets
4. **Who Can Join** (lines 325-334): Eligibility criteria
5. **Sites Map** (lines 336-374): UK map + site list
6. **Contact** (lines 376-395): Multiple contact methods
7. **Footer** (lines 397-405): Logos, funding acknowledgment

## Accessibility Features

- **Font size**: 18px base (larger than standard 16px)
- **Line height**: 1.6 (increased from typical 1.5)
- **Button size**: Minimum 48px height (WCAG touch target)
- **Focus states**: 3px outline on all interactive elements
- **Color contrast**: 4.5:1+ ratio throughout
- **Link styling**: Underline with 2px offset, thicker on hover

## Color Palette

```css
--accent: #0f6a8d        /* Blue - primary brand color */
--accent-light: #e2f2f8  /* Light blue - backgrounds */
--text: #1f1f1f          /* Near-black - body text */
--muted: #4d4d4d         /* Gray - secondary text */
--card: #ffffff          /* White - card backgrounds */
--bg: #f7f8f9            /* Off-white - page background */
```

## Current Issues / TODOs

1. **Map image missing**: `assets/UK-ENHANCE-map.png` needs to be created
   - Should show all 10 recruiting sites
   - Text must be 18-22pt (readable on mobile)
   - Export from Word doc at 1200px+ width
   
2. **Contact placeholders**: 
   - Phone: `020 8133 1990` (verify/update)
   - SMS: `07800 000000` (placeholder - needs real number)
   - Email: `enhance@ucl.ac.uk` (verify active)

3. **Pre-screen form**: `coming-soon.html` is placeholder (needs actual form)

## Site List (10 locations)

Must be kept in sync between:
- Word doc map (`assets/SitesUKMapWordDoc4FutureUpdates/Map_of_GP_locations.docx`)
- HTML site list (`index.html` lines 360-371)

Current sites:
1. North London NHS Foundation Trust - London NW5 3EG
2. Humber NHS Teaching Trust - Hull HU10 6FE
3. The Rise Group Practice - London N19 3YU
4. Mathukia Surgery - Ilford IG1 2SF
5. Knutsford Medical Partnership - Knutsford WA16 0LY
6. Coquet Medical Group - Morpeth NE65 9SF
7. Widdrington (Northumbria Primary Care) - Morpeth NE65 9PR
8. Living Well Partnership - Hampshire SO19 9GH
9. The Practice of Health - Barry CF63 1BA
10. Llan Healthcare - Cardiff CF23 9PF

## Update Workflows

### Adding/Removing a Site

1. Update Word doc (`assets/SitesUKMapWordDoc4FutureUpdates/Map_of_GP_locations.docx`)
2. Export as PNG (1200px+ wide) → save as `assets/UK-ENHANCE-map.png`
3. Update HTML site list in `index.html` (lines 360-371)
4. Test on mobile device

### Changing Contact Info

1. Find and replace in both `index.html` and `coming-soon.html`
2. Update both display text and `href` attributes (tel:, mailto:)
3. Test links on mobile device

## Design References

- **HOME trial website**: See `sourcedocs/HomeTrial/*.pdf` for style inspiration
- **Target audience**: Low SES, lower education, older adults (60-80)
- **Tone**: Friendly, reassuring, non-clinical, respectful

## Mobile Optimization

- Base font: 18px desktop, 17px mobile
- All padding/margins use `clamp()` for fluid scaling
- Grid layouts with `auto-fit` for responsive columns
- CTA button: Full width on mobile (<600px)
- Touch targets: Minimum 48px height/width

## Browser Support

Designed for modern browsers (Chrome, Safari, Firefox, Edge). Uses:
- CSS Grid
- CSS Custom Properties (variables)
- `clamp()` for fluid typography
- No polyfills needed (target audience uses recent devices)

## Deployment

- **GitHub Pages**: Recommended (free, easy updates)
- **Alternative**: Any static hosting (Netlify, Vercel, etc.)
- **No build step**: Just upload HTML + assets folder

## AI Agent Instructions

When making changes:
1. **Preserve accessibility**: Don't reduce font sizes, contrast, or touch targets
2. **Keep it simple**: Avoid adding JavaScript or build complexity
3. **Test assumptions**: Contact details are placeholders - flag if they look wrong
4. **Mobile-first**: Always consider how changes look on small screens
5. **Plain English**: Avoid medical/technical jargon in content
6. **Maintain tone**: Friendly, warm, trustworthy (not clinical or corporate)

## Reference Materials

- `sourcedocs/HomeTrial/`: Example study website (similar audience)
- `sourcedocs/ENHANCE_Social_Media_Advertising_v1.0_20.10.2025.docx`: Approved messaging
- `sourcedocs/ENHANCE_Coaching_Manual_V.5_21.11.25_SCG.docx`: Study details

Last updated: December 2025
