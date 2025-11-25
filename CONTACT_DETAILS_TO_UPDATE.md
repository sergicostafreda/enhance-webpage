# ENHANCE Webpage - Contact Details to Update

## Current Placeholder Contact Information

The following contact details are **PLACEHOLDERS** and need to be updated with actual ENHANCE study contacts before going live.

---

## 📞 Phone Number

**Current placeholder**: `020 8133 1990`

**Locations in code:**
- `index.html` line 255 (hero section)
- `index.html` line 364 (contact section)
- `coming-soon.html` line 100

**What to update:**
1. Replace with actual ENHANCE study phone number
2. Confirm and add office hours text (e.g., "Monday-Friday, 9am-5pm")
3. Update the `tel:` link to match the number

**Example replacement:**
```html
<!-- OLD -->
📞 Call <strong>020 8133 1990</strong> (office hours)

<!-- NEW -->
📞 Call <strong>020 XXXX XXXX</strong> (Monday-Friday, 9am-5pm)
```

And update the clickable link:
```html
<a href="tel:020XXXXXXXX">020 XXXX XXXX</a>
```

---

## 📱 SMS Number

**Current placeholder**: `07800 000000`

**Locations in code:**
- `index.html` line 256 (hero section)
- `index.html` line 365 (contact section)
- `coming-soon.html` line 102

**What to update:**
1. Replace with actual ENHANCE study mobile/SMS number
2. Ensure this number can receive and reply to SMS messages
3. Consider if you want to keep "we'll reply to you" language or change to "we'll call you back"

**Example replacement:**
```html
<!-- OLD -->
📱 Send us an SMS at <strong>07800 000000</strong> and we'll reply to you

<!-- NEW -->
📱 Send us an SMS at <strong>07XXX XXXXXX</strong> and we'll reply to you
```

---

## 📧 Email Address

**Current**: `enhance@ucl.ac.uk`

**Locations in code:**
- `index.html` line 257 (hero section)
- `index.html` line 363 (contact section)
- `coming-soon.html` line 101

**Action needed:**
- ✅ Verify this is the correct email
- ✅ Ensure this inbox is monitored regularly
- ✅ Set up auto-reply if needed (e.g., "Thank you for your interest, we'll respond within 2 working days")

**If email needs changing:**
```html
<!-- Replace all instances of -->
<a href="mailto:enhance@ucl.ac.uk">enhance@ucl.ac.uk</a>

<!-- With -->
<a href="mailto:NEW-EMAIL@ucl.ac.uk">NEW-EMAIL@ucl.ac.uk</a>
```

---

## 🔍 How to Update

### Method 1: Search and Replace (Recommended)

Use your code editor's find-and-replace function:

1. **Phone number:**
   - Find: `020 8133 1990`
   - Replace with: `[your actual number]`
   - Also find: `tel:02081331990`
   - Replace with: `tel:[your actual number, no spaces]`

2. **SMS number:**
   - Find: `07800 000000`
   - Replace with: `[your actual SMS number]`

3. **Email (if needed):**
   - Find: `enhance@ucl.ac.uk`
   - Replace with: `[your actual email]`

### Method 2: Manual Update

Open each file and update line by line:

**Files to update:**
- `index.html` (lines 255-257, 363-365)
- `coming-soon.html` (lines 100-102)

---

## ⏰ Office Hours Text

**Current**: "(office hours)"

**Recommended formats:**
- `(Monday-Friday, 9am-5pm)`
- `(Mon-Fri, 9:00-17:00)`
- `(Weekdays, 9am-5pm GMT)`
- `(Office hours: Mon-Fri 9-5)`

Choose format based on:
- Target audience (low SES/education → simpler "Mon-Fri, 9am-5pm")
- Whether you cover phone during holidays
- Time zone clarity if recruiting across UK

---

## ✅ Pre-Launch Checklist

Before making the website public, verify:

- [ ] Phone number is correct and active
- [ ] Phone is staffed during stated office hours
- [ ] SMS number can receive and send text messages
- [ ] SMS inbox is monitored regularly
- [ ] Email address is correct
- [ ] Email inbox is monitored regularly (ideally daily)
- [ ] Team knows to expect calls/texts/emails from website visitors
- [ ] Voicemail message is appropriate if calls missed
- [ ] Auto-reply email set up (optional but recommended)
- [ ] Contact details tested from external phone/email

---

## 📝 Testing After Update

Once you've updated the contact details:

1. **Test phone link on mobile:**
   - Open website on phone
   - Tap the phone number
   - Verify it opens phone dialer with correct number

2. **Test SMS:**
   - Send test SMS to the number
   - Verify it's received
   - Test replying from that number

3. **Test email link:**
   - Click email link
   - Verify correct address appears in "To:" field
   - Send test email
   - Verify it's received in correct inbox

---

## 🔒 Security Note

**Do not commit real phone numbers to public GitHub repository if:**
- Numbers are personal mobile phones (not office lines)
- You're concerned about spam/unwanted calls
- Numbers haven't been publicly shared yet

**Alternative approach:**
- Keep a separate `config.js` file with contact details (not committed to repo)
- Use environment variables
- Or simply update contact details only on production deployment, not in GitHub

---

## Questions?

Contact: Sergi / ENHANCE team

Last updated: 2025-11-25
