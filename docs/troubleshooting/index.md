---
sidebar_position: 1
---

# Troubleshooting

## Quick Reference

Running into issues with ShootPath? This section covers common problems and their solutions, from login difficulties to email delivery problems. Most issues can be resolved quickly by following the troubleshooting steps below.

**Common Issue Categories:**
- [Login Issues](./login-issues) - Can't log in, password problems, locked accounts
- [Payment Problems](./payment-problems) - Client payments failing, Stripe connection issues
- [Email Delivery](./email-delivery) - Emails not sending or going to spam
- [Sync Issues](./sync-issues) - Calendar sync problems, mobile app issues

**Quick Troubleshooting Steps:**
1. Clear your browser cache and cookies
2. Try a different browser (Chrome recommended)
3. Check if your internet connection is stable
4. Verify you're using a supported browser version
5. Check our [Status Page](https://status.shootpath.com) for known outages

**Getting Help:**
- **Help Documentation:** You're reading it! Use the search bar to find specific topics
- **Email Support:** [support@shootpath.com](mailto:support@shootpath.com) - Response within 24 hours
- **Live Chat:** Available in your ShootPath dashboard (click the chat icon)
- **Video Tutorials:** [YouTube Channel](https://youtube.com/shootpath)
- **Community Forum:** [community.shootpath.com](https://community.shootpath.com)

:::tip Quick Fixes for Common Issues
Before diving into detailed troubleshooting, try these universal fixes that solve 80% of problems:
- **Hard refresh the page:** Ctrl+Shift+R (Windows) or Cmd+Shift+R (Mac)
- **Clear browser cache:** Settings → Privacy → Clear browsing data
- **Log out and log back in:** Click your profile → Log out → Log in again
- **Update your browser:** Help → About → Check for updates
:::

---

## Detailed Guide

### Troubleshooting Workflow

When something isn't working, follow this systematic approach to identify and resolve the issue:

**Step 1: Identify the Problem**
- What were you trying to do?
- What happened instead?
- Did you see an error message? (Screenshot it!)
- When did the problem start?
- Has this ever worked before?

**Step 2: Check the Basics**
- Are you connected to the internet?
- Is ShootPath experiencing an outage? (Check [status.shootpath.com](https://status.shootpath.com))
- Are you using a supported browser?
- Is your browser up to date?

**Step 3: Try Simple Fixes**
- Refresh the page (Ctrl+R or Cmd+R)
- Hard refresh to clear cache (Ctrl+Shift+R or Cmd+Shift+R)
- Log out and log back in
- Try a different browser
- Try on a different device (phone, tablet, another computer)

**Step 4: Consult Documentation**
- Search this help documentation for your specific issue
- Check the relevant section (Login, Payments, Email, etc.)
- Follow the troubleshooting steps exactly

**Step 5: Gather Information**
If you need to contact support, collect:
- Screenshot of error message
- Steps to reproduce the problem
- Your browser and version (find this at [whatismybrowser.com](https://whatismybrowser.com))
- Your account email
- Date and time when problem occurred

**Step 6: Contact Support**
Email [support@shootpath.com](mailto:support@shootpath.com) with the information from Step 5.

### Browser Requirements

ShootPath is a modern web application that requires an up-to-date browser for optimal performance.

**Supported Browsers:**

| Browser | Minimum Version | Recommended Version |
|---------|----------------|---------------------|
| Google Chrome | 90+ | Latest |
| Safari | 14+ | Latest |
| Firefox | 88+ | Latest |
| Microsoft Edge | 90+ | Latest |

**Not Supported:**
- Internet Explorer (any version) - Microsoft ended support in 2022
- Opera Mini - Limited JavaScript support
- Very old browsers (Chrome < 90, Safari < 14, Firefox < 88)

**Recommended Browser: Google Chrome**
ShootPath is developed and tested primarily on Chrome, so it offers the best experience:
- Fastest performance
- Best compatibility
- Fewest bugs
- First to receive new features

**How to Check Your Browser Version:**

**Chrome:**
1. Click the three dots in the top right
2. Go to **Help → About Google Chrome**
3. Chrome shows current version and auto-updates

**Safari:**
1. Click **Safari → About Safari**
2. Version is shown in the popup

**Firefox:**
1. Click the hamburger menu (three lines)
2. Go to **Help → About Firefox**
3. Firefox shows current version and auto-updates

**Edge:**
1. Click the three dots in the top right
2. Go to **Help and feedback → About Microsoft Edge**
3. Edge shows current version and auto-updates

**Updating Your Browser:**
Most modern browsers auto-update, but if you're on an old version:
- Chrome: Help → About Google Chrome → Relaunch to update
- Safari: Update via macOS Software Update in System Preferences
- Firefox: Help → About Firefox → Restart to update
- Edge: Help → About Microsoft Edge → Restart to update

### System Requirements

**Operating System:**
ShootPath works on any modern operating system:
- **Windows:** Windows 10 or newer
- **macOS:** macOS 10.14 (Mojave) or newer
- **Linux:** Any modern distribution with a supported browser
- **ChromeOS:** Fully supported (Chromebooks work great!)

**Internet Connection:**
- **Minimum:** 1 Mbps download, 0.5 Mbps upload
- **Recommended:** 5+ Mbps download, 2+ Mbps upload (especially for photo uploads)
- **Type:** Any (WiFi, Ethernet, 4G/5G mobile)

**Hardware:**
ShootPath is lightweight and doesn't require powerful hardware:
- **Processor:** Any processor from the last 10 years
- **RAM:** 2 GB minimum, 4 GB recommended
- **Storage:** No local storage required (everything is cloud-based)
- **Screen:** Works on any size (optimized for 1280x720 and above)

**Mobile Devices:**
- **iOS:** iOS 13 or newer (iPhone, iPad)
- **Android:** Android 8.0 or newer

**Not Required:**
- You don't need to install anything (ShootPath is browser-based)
- No plugins or extensions needed
- No special software

### Known Issues

We maintain a list of known issues and their current status. If you're experiencing one of these, we're already working on a fix.

**Current Known Issues (Updated February 2026):**

**Issue: Gallery Upload Slow on Safari**
- **Affects:** Safari browser only
- **Description:** Gallery photo uploads are slower than on Chrome
- **Workaround:** Use Chrome for large gallery uploads
- **Status:** Investigating optimization

**Issue: Email Templates Not Saving on Firefox Mobile**
- **Affects:** Firefox browser on Android/iOS
- **Description:** Saving email template edits sometimes fails
- **Workaround:** Use Firefox Desktop or Chrome Mobile
- **Status:** Fix in development

**Issue: Calendar Sync Delay**
- **Affects:** Google Calendar sync
- **Description:** New events may take up to 15 minutes to appear in Google Calendar
- **Workaround:** None (sync happens in background)
- **Status:** This is a Google Calendar API limitation, not a bug

**Issue: Mobile App Push Notifications Delay (iOS)**
- **Affects:** iOS app only
- **Description:** Push notifications sometimes delayed by 5-10 minutes
- **Workaround:** None
- **Status:** Investigating with Apple Push Notification Service

**Check Current Status:**
For up-to-date information on outages and known issues:
- **Status Page:** [status.shootpath.com](https://status.shootpath.com)
- **Twitter:** [@ShootPathStatus](https://twitter.com/shootpathstatus)
- **In-App Notifications:** We display banner alerts for major issues

### Common Quick Fixes

These solutions resolve many common issues without needing to dig deeper:

**Problem: Page Won't Load or Displays Incorrectly**

**Solution 1: Hard Refresh**
- Windows/Linux: Press **Ctrl + Shift + R**
- Mac: Press **Cmd + Shift + R**

This clears cached files that might be outdated.

**Solution 2: Clear Browser Cache**
- Chrome: Settings → Privacy and security → Clear browsing data → Choose "Cached images and files" → Clear
- Safari: Safari → Settings → Privacy → Manage Website Data → Remove All
- Firefox: Settings → Privacy & Security → Cookies and Site Data → Clear Data

**Solution 3: Disable Browser Extensions**
Browser extensions (ad blockers, privacy tools) can interfere:
1. Open a private/incognito window (Ctrl+Shift+N or Cmd+Shift+N)
2. Go to ShootPath
3. If it works, an extension is the problem
4. Disable extensions one-by-one to find the culprit

**Problem: "Session Expired" Error**

**Solution:**
You've been logged out due to inactivity (4-hour timeout). Simply log back in.

To avoid this:
- ShootPath auto-saves most changes (you won't lose work)
- Keep your session active by clicking something every few hours
- Use "Remember Me" when logging in (stays logged in for 30 days)

**Problem: Changes Not Saving**

**Solution 1: Check for Error Messages**
Look for a red error message at the top of the screen. It will tell you what's wrong (missing required field, validation error, etc.).

**Solution 2: Check Internet Connection**
If your internet drops briefly:
1. ShootPath can't save changes to the server
2. Look for a "Reconnecting..." message
3. Once reconnected, try saving again

**Solution 3: Refresh and Try Again**
Sometimes a temporary glitch prevents saving:
1. Refresh the page (you may lose unsaved changes)
2. Re-enter your changes
3. Try saving again

**Problem: Slow Performance**

**Solution 1: Close Unused Tabs**
Having many browser tabs open (especially other apps like Gmail, Facebook) uses memory and slows everything down. Close tabs you're not using.

**Solution 2: Restart Your Browser**
Browsers can get sluggish after running for days:
1. Close all browser windows
2. Wait 10 seconds
3. Open browser and go to ShootPath

**Solution 3: Check for Background Processes**
Other programs using CPU/memory can slow your browser:
- Windows: Ctrl+Shift+Esc → Task Manager → Check CPU/Memory columns
- Mac: Cmd+Space → Activity Monitor → Check CPU/Memory tabs

Close unnecessary programs.

**Problem: Can't Upload Photos**

**Solution 1: Check File Size**
ShootPath limits individual file uploads to 50 MB:
- Most JPEGs from cameras are 5-15 MB (fine)
- RAW files can be 50+ MB (too large)
- Compress large files or export as JPEG before uploading

**Solution 2: Check File Format**
Supported formats: JPG, JPEG, PNG, GIF, WEBP, HEIC
Not supported: PSD, TIFF, RAW, CR2, NEF, ARW

Convert unsupported formats to JPEG first.

**Solution 3: Check Browser Permissions**
Your browser may be blocking file access:
- Chrome: Click the icon in the address bar → Allow ShootPath to access files
- Safari: Safari → Settings → Websites → Files → Allow
- Firefox: Site permissions → Check "Access files"

**Problem: Buttons Not Clickable**

**Solution 1: Zoom Level**
If your browser is zoomed in/out too far, buttons may be cut off:
- Windows/Linux: Ctrl+0 (zero) to reset zoom
- Mac: Cmd+0 (zero) to reset zoom

**Solution 2: Overlay Stuck**
Sometimes a modal or overlay gets stuck on screen:
- Press **Esc** to close overlays
- Refresh the page
- Try clicking the darkened background area

**Problem: Mobile App Not Working**

**Solution 1: Update the App**
- iOS: App Store → Updates → Update ShootPath
- Android: Google Play → My apps & games → Update ShootPath

**Solution 2: Clear App Cache**
- iOS: Delete and reinstall the app
- Android: Settings → Apps → ShootPath → Storage → Clear cache

**Solution 3: Check Internet Connection**
- Mobile apps require internet connection (no offline mode yet)
- Try switching between WiFi and cellular
- Turn airplane mode on, wait 10 seconds, turn it off

### Getting Help

If you've tried the troubleshooting steps and still have issues, we're here to help.

**Before Contacting Support:**
Gather this information to speed up resolution:
1. **What were you trying to do?** (e.g., "Send a quote email to a client")
2. **What happened instead?** (e.g., "Got an error message saying 'Email failed'")
3. **Error message** (take a screenshot if possible)
4. **Browser and version** (find at [whatismybrowser.com](https://whatismybrowser.com))
5. **Account email** (so we can look up your account)
6. **When it happened** (date and approximate time)

**Contact Options:**

**Email Support** (Best for non-urgent issues)
- Email: [support@shootpath.com](mailto:support@shootpath.com)
- Response time:
  - Starter plan: Within 48 hours
  - Professional plan: Within 24 hours
  - Studio plan: Within 12 hours
- Include all information listed above
- Attach screenshots if relevant

**Live Chat** (For urgent issues)
- Available in your ShootPath dashboard
- Click the chat icon in the bottom right
- Live during business hours (9am-5pm ET, Monday-Friday)
- After hours: Leave a message and we'll respond via email

**Phone Support** (Studio plan only)
- Available for Studio plan customers
- Schedule a call: [calendly.com/shootpath-support](https://calendly.com/shootpath-support)
- 30-minute troubleshooting sessions

**Community Forum**
- [community.shootpath.com](https://community.shootpath.com)
- Search existing discussions
- Post your question for community + staff responses
- Good for "how do I" questions and feature requests

**What to Expect from Support:**

**Response Times:**
- First response within stated timeframe (12-48 hours based on plan)
- Complex issues may take multiple emails to resolve
- We'll keep you updated on progress

**How We Help:**
1. Acknowledge your issue and confirm we're looking into it
2. Ask clarifying questions if needed
3. Provide step-by-step solution or workaround
4. Confirm the issue is resolved
5. If it's a bug, we'll escalate to engineering and notify you when fixed

**What We Can Do:**
- Troubleshoot technical issues
- Explain how features work
- Provide workarounds for known issues
- Escalate bugs to engineering
- Adjust billing/account settings
- Manually fix data issues (if something got corrupted)

**What We Can't Do:**
- Implement custom features for individual accounts (unless on Enterprise plan)
- Recover data deleted more than 90 days ago
- Provide design or photography business advice
- Access your Stripe or Gmail account directly (you need to handle integrations on those platforms)

### Video Tutorials

Prefer watching over reading? We have video tutorials for most features:

**YouTube Channel: [youtube.com/shootpath](https://youtube.com/shootpath)**

**Popular Tutorial Playlists:**
- **Getting Started** (10 videos, 45 minutes total) - Complete walkthrough for new users
- **Workflows** (8 videos, 30 minutes) - Setting up automation
- **Galleries** (6 videos, 25 minutes) - Client proofing and delivery
- **Troubleshooting** (12 videos, 60 minutes) - Fixing common issues

**Most Watched Troubleshooting Videos:**
- "Why Aren't My Emails Sending?" (5 minutes)
- "Connecting Stripe for Payments" (8 minutes)
- "Google Calendar Sync Setup" (6 minutes)
- "Fixing Login Issues" (4 minutes)

**Subscribe:** Get notified when we publish new tutorials and feature updates.

### System Status

**Real-Time Status:** [status.shootpath.com](https://status.shootpath.com)

Our status page shows:
- **Operational** (green) - Everything working normally
- **Degraded Performance** (yellow) - System is slow but functional
- **Partial Outage** (orange) - Some features down
- **Major Outage** (red) - System unavailable

**Incident History:**
View past outages and how they were resolved:
- What happened
- How long it lasted
- What we did to fix it
- Steps we took to prevent recurrence

**Subscribe to Updates:**
Get email or SMS notifications when we post status updates:
1. Go to [status.shootpath.com](https://status.shootpath.com)
2. Click **Subscribe to Updates**
3. Enter your email or phone number
4. You'll be notified of any incidents

**Current Uptime:**
ShootPath maintains 99.9% uptime (about 40 minutes of downtime per month, mostly planned maintenance).

**Planned Maintenance:**
- Scheduled during off-peak hours (3am-5am ET, usually Sundays)
- Announced at least 48 hours in advance via:
  - Status page
  - Email to all users
  - In-app banner notification
- Rarely exceeds 30 minutes

---

## Common Questions

**How do I know if the problem is on my end or ShootPath's end?**
1. Check [status.shootpath.com](https://status.shootpath.com) first
2. If status shows "Operational," the issue is likely on your end
3. Try accessing ShootPath from a different device or network
4. Search community forum to see if others report the same issue

**Will ShootPath support help me with Stripe or Gmail issues?**
We can help with:
- Connecting Stripe to ShootPath
- Troubleshooting the integration
- Explaining error messages

We cannot:
- Access your Stripe account directly (you need to contact Stripe support)
- Fix Gmail SMTP settings (you need to contact Google)

However, we'll guide you on what to ask their support teams.

**Can I get a refund if ShootPath was down and I couldn't work?**
- For extended outages (48+ hours), we may offer prorated refunds or credits
- For brief outages (under 4 hours), no refund per our SLA
- Outages are extremely rare (99.9% uptime)
- Contact [billing@shootpath.com](mailto:billing@shootpath.com) if you believe you're entitled to a credit

**How long does support take to respond?**
- Starter: Within 48 hours
- Professional: Within 24 hours
- Studio: Within 12 hours
- These are maximums; average response time is much faster (3-6 hours)

**Can I call someone for urgent help?**
- Live chat during business hours (9am-5pm ET) for all plans
- Phone support available for Studio plan customers
- For critical issues (account locked, payment emergency), email [support@shootpath.com](mailto:support@shootpath.com) with "URGENT" in subject line - we monitor 24/7 for urgent issues

**Do you have a bug bounty program?**
Yes! If you discover a security vulnerability:
1. Email [security@shootpath.com](mailto:security@shootpath.com) (do not post publicly)
2. Include steps to reproduce
3. We'll investigate and respond within 24 hours
4. Bounties range from $50-$1,000 depending on severity

For non-security bugs, just use regular support channels.

---

## Need More Help?

**Search This Documentation:**
Use the search bar at the top to find specific topics. Try searching for:
- Specific error messages
- The feature you're having trouble with
- Keywords like "login," "email," "payment," etc.

**Browse by Category:**
Use the navigation on the left to explore:
- [Login Issues](./login-issues)
- [Payment Problems](./payment-problems)
- [Email Delivery](./email-delivery)
- [Sync Issues](./sync-issues)

**Still Stuck?**
Contact [support@shootpath.com](mailto:support@shootpath.com) and we'll help you resolve the issue.
