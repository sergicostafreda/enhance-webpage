# ENHANCE Webpage - Image Sourcing Checklist

## Why Higher Resolution Images Are Needed

Current images are too small and will appear blurry/pixelated on modern screens (especially retina displays). We need images that are **2-3x larger** than their display size.

---

## 1. UCL Logo

**Current file**: `UCLlogo.png` (155 x 45px) ❌ TOO SMALL
**Required**: 180-240px height minimum (for 60px display size at 3x retina)

### How to Get:
1. **Official UCL Brand Portal**: https://www.ucl.ac.uk/brand/logo
2. Download the **horizontal logo** (UCL + text)
3. Choose **PNG format** with **transparent background**
4. Select **high resolution** version
5. Save as `UCLlogo.png` in `/assets` folder (replacing current file)

**Notes:**
- Must follow UCL brand guidelines
- Transparent background preferred
- Blue version matches our color scheme

---

## 2. NIHR Logo

**Current file**: `NIHRlogo.png` (178 x 45px) ❌ TOO SMALL
**Required**: 180-240px height minimum

### How to Get:
1. **Official NIHR Logo Page**: https://www.nihr.ac.uk/about-us/our-logos.htm
2. Download the **full color NIHR logo**
3. Choose **high resolution PNG** format
4. Save as `NIHRlogo.png` in `/assets` folder (replacing current file)

**Alternative:**
- Contact NIHR communications team: communications@nihr.ac.uk
- Request high-res logo for research study website

**Notes:**
- Ensure you download the "NIHR" logo (not CRN or other variants)
- PNG with transparent background preferred

---

## 3. North London NHS Foundation Trust Logo

**Current file**: `NLFTlogo.png` (110 x 45px) ❌ TOO SMALL
**Required**: 180-240px height minimum

### How to Get:
1. **Contact NLFT Communications Team** directly
   - Email: communications@northlondon-nhs.nhs.uk (verify current contact)
   - Request: "High-resolution logo for ENHANCE study website"
2. **Alternative**: Check NLFT website footer/about page for logo downloads
3. **Specification needed**: Minimum 240px height, PNG, transparent background

**Notes:**
- May need to specify it's for the ENHANCE study (IRAS: 33426)
- Request the standard horizontal logo
- Ensure NHS brand guidelines compliance

---

## 4. Tablet Illustration

**Current file**: `EnhanceTabletPic.png` (127 x 129px) ⚠️ CRITICALLY TOO SMALL
**Required**: 600-800px wide minimum (for hero section display)

### Options:

**Option A: Get Original Source File**
1. Contact whoever created the original illustration
2. Request export at **800px wide** minimum
3. PNG format with transparent background preferred
4. Save as `EnhanceTabletPic.png` (replacing current file)

**Option B: Use Stock/Custom Illustration**
1. Commission new illustration showing:
   - Tablet device
   - Brain health app interface
   - Friendly, modern, accessible design
2. Export at high resolution (800-1000px wide)
3. Style should match ENHANCE brand colors

**Option C: Recreate from Screenshot**
1. If you have the actual ENHANCE app
2. Take high-res screenshot of tablet interface
3. Edit/stylize as needed
4. Export at 800px+ wide

**Notes:**
- This is the MOST IMPORTANT image to fix (currently in hero section)
- Low resolution will make the entire site look unprofessional
- Should look modern, friendly, and trustworthy

---

## 5. Older People with App Image

**Current file**: `OlderPeopleWithAppPic.png` (325 x 129px) - Not currently used
**Required**: 600-800px wide if you want to use it

### Status: OPTIONAL
This image is referenced in assets but not currently displayed on the webpage.

**If you want to add it back:**
1. Get higher resolution version (600-800px wide)
2. Consider where it would appear (perhaps in "What's Involved" section)
3. Ensure it shows:
   - Diverse older adults (60-80 age range)
   - Using digital devices (tablet/phone)
   - Friendly, approachable, not clinical

**Stock photo sources:**
- Pexels (free): https://www.pexels.com
- Unsplash (free): https://unsplash.com
- iStock/Getty (paid): Higher quality, diverse representation

**Search terms:**
- "older adults using tablet"
- "seniors digital health"
- "elderly people smartphone app"
- Age range: 60-80 years old

---

## Image Optimization After Sourcing

Once you have high-resolution images:

### 1. Check File Sizes
```bash
ls -lh assets/
```

**Target sizes:**
- Logos: 10-30KB each
- Tablet illustration: 50-150KB
- Photos: 100-300KB

### 2. Optimize if Needed
Use tools like:
- **TinyPNG**: https://tinypng.com (online, free)
- **ImageOptim** (Mac): https://imageoptim.com
- **Squoosh**: https://squoosh.app (Google, online)

**Settings:**
- JPEG: 80-90% quality
- PNG: Compress with transparency preserved
- Maximum width: 2000px (oversized images waste bandwidth)

### 3. Test on Device
After replacing images:
1. Deploy to GitHub Pages
2. Test on actual mobile phone (iPhone + Android)
3. Verify logos look crisp and authoritative
4. Verify tablet image looks professional and clear
5. Check page load speed isn't too slow

---

## Priority Order

**Must have (critical):**
1. ✅ Tablet illustration (currently 127px → need 800px) - URGENT
2. ✅ UCL logo (currently 155px → need 240px)
3. ✅ NIHR logo (currently 178px → need 240px)
4. ✅ NLFT logo (currently 110px → need 240px)

**Nice to have:**
5. ⭕ Older people image (if you want to use it)
6. ⭕ Additional illustrations/photos

---

## File Organization

```
/Users/sergi/Coding/enhance-webpage/assets/
├── UCLlogo.png (NEW: 240px height)
├── NIHRlogo.png (NEW: 240px height)
├── NLFTlogo.png (NEW: 240px height)
├── EnhanceTabletPic.png (NEW: 800px wide)
├── OlderPeopleWithAppPic.png (OPTIONAL: 800px wide)
├── enhance-sites-map.jpg (TO BE CREATED by MSE students)
└── ascendtrialcoukSitesMap.jpeg (DRAFT - can delete after new map created)
```

---

## Questions?

Contact Sergi or ENHANCE team for:
- Access to brand assets
- Approval to use certain images
- Technical help with image editing/optimization

---

## Accessibility Note

When sourcing images of people:
- Ensure diverse representation (age, ethnicity, gender)
- Show realistic scenarios (not overly posed/stock-photo-looking)
- Reflect the 60-80 age demographic
- Appear warm, friendly, and approachable (matching low SES/education audience needs)
