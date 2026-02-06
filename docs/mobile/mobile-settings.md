---
sidebar_position: 4
---

# Mobile Settings

## Quick Reference

Configure your ShootPath mobile app for optimal performance, relevant notifications, and secure access. This guide covers all mobile-specific settings, preferences, troubleshooting steps, and best practices for keeping your mobile experience smooth.

**Key Settings Categories:**
- **Notifications** - Control what alerts you receive
- **Data & Sync** - Manage cache, auto-refresh, and data usage
- **Calendar** - Sync with device calendar and configure preferences
- **Security** - Biometric login and session management
- **Appearance** - Dark mode and visual preferences
- **About & Support** - App version, help resources, privacy

**Access Settings:**
Tap **More** tab (bottom right) → **Settings** (gear icon or listed option)

---

## Detailed Guide

### Accessing Mobile Settings

**From the main app:**

1. Tap the **More** tab at the bottom right (usually an ellipsis "..." icon or "More" label)
2. Tap **Settings** (gear icon or text label)
3. Settings screen opens with all configuration options

**Alternative (on some versions):**

Settings might be grouped under **Profile** or accessed via a menu icon in the top navigation bar. Look for a gear icon anywhere in the More tab.

### Notification Settings

Control what push notifications you receive on your mobile device. Smart notification configuration keeps you informed without overwhelming you.

#### Notification Categories

**New Leads**

**What it does:** Alerts you when a new inquiry comes in through your contact form or lead capture.

**Example notification:**
> "New Lead: Sarah Johnson inquired about a wedding on June 15, 2025"

**Recommendation:** **Turn ON** if you want to respond quickly to leads. Fast responses increase booking rates.

**Turn OFF if:** You check leads on your own schedule and don't want interruptions.

---

**Session Reminders**

**What it does:** Reminds you of upcoming photo sessions.

**Timing options:**
- **1 day before** - "Session Tomorrow: Smith Wedding at 2:00 PM"
- **1 hour before** - "Session in 1 hour: Thompson Family Portraits"
- **Both** - Get both reminders (recommended)
- **Off** - No session reminders

**Recommendation:** **Turn ON both**. The 1-day reminder helps you prepare equipment and review details. The 1-hour reminder ensures you're on time.

**Turn OFF if:** You use a separate calendar system for reminders and don't want duplicates.

---

**Payments Received**

**What it does:** Notifies you when clients pay invoices or deposits.

**Example notification:**
> "Payment Received: $1,500 deposit from Smith Wedding"

**Recommendation:** **Turn ON**. Immediate payment notifications let you know when cash flow happens, which is useful for financial tracking and peace of mind.

**Turn OFF if:** You review payments on desktop daily and don't need real-time alerts.

---

**Contracts Signed**

**What it does:** Alerts you when a client signs their contract.

**Example notification:**
> "Contract Signed: Johnson Wedding - Contract fully executed"

**Recommendation:** **Turn ON**. Contract signing is a critical milestone that unlocks next workflow steps. Knowing immediately is valuable.

**Turn OFF if:** You only care about this when you log into the app, not as an interrupt.

---

**Gallery Activity**

**What it does:** Notifies you when clients view or interact with their galleries.

**Example notifications:**
> "Gallery Viewed: Davis Newborn Session gallery opened by client"
> "Client Downloaded 12 Photos from Thompson Family Portraits gallery"

**Recommendation:** **Turn ON if you want to track client engagement.** This is useful for knowing when to follow up ("Hey! Saw you viewed the gallery—let me know if you have any questions!").

**Turn OFF if:** Gallery activity doesn't require immediate attention and you check it manually.

---

**Overdue Payments**

**What it does:** Alerts you when payments become overdue.

**Example notification:**
> "Payment Overdue: $2,000 balance due 3 days ago for Smith Wedding"

**Recommendation:** **Turn ON**. Overdue payment alerts help you follow up promptly with clients, improving cash flow.

**Turn OFF if:** You have a separate system for tracking overdue invoices.

---

**Task Reminders**

**What it does:** Notifies you when workflow tasks are due or approaching deadlines.

**Example notification:**
> "Task Due Today: Send Edited Gallery to Thompson Family"

**Recommendation:** **Turn ON if you want accountability for task deadlines.** This keeps your workflow on track.

**Turn OFF if:** You manage your task list manually and don't want push reminders.

---

#### Notification Timing

**Quiet Hours**

Set specific times when notifications are silenced.

**Use case:** If you don't want notifications during sleep hours (e.g., 10:00 PM - 7:00 AM), enable quiet hours.

**How to configure:**
1. Tap **Quiet Hours** toggle
2. Set start time (e.g., 10:00 PM)
3. Set end time (e.g., 7:00 AM)
4. Save

**What happens:** Notifications still arrive, but they won't make a sound or vibration during quiet hours. You'll see them when you check your phone.

**Exception:** Session reminders within 1 hour might override quiet hours (depending on configuration) to ensure you don't miss a shoot.

---

**Notification Sound**

**Options:**
- Default notification sound
- Custom sound (if supported)
- Silent (notifications appear but make no sound)

**Recommendation:** Use a distinct sound so you recognize ShootPath alerts vs. other app notifications.

---

**Badge Count**

**What it does:** Shows a red number on the app icon indicating unread notifications or pending actions.

**Recommendation:** **Turn ON** if you want a visual reminder to check the app.

**Turn OFF if:** Badge counts stress you out or you prefer to check the app on your own schedule.

---

#### Managing Existing Notifications

**Clear all notifications:**

From the Notifications settings screen, tap **Clear All** to dismiss all past notifications.

**View notification history:**

Some versions allow you to see a list of recent notifications within the app (More > Notifications > History). This is useful if you dismissed a notification but want to reference it later.

### Data & Sync Settings

Control how the app syncs data with the server and manages storage on your device.

#### Auto-Refresh Interval

**What it does:** Sets how often the app automatically fetches new data from the server when open.

**Options:**
- **Every 30 seconds** - Near real-time (uses more battery/data)
- **Every 1 minute** - Balanced (recommended)
- **Every 5 minutes** - Low-frequency updates (saves battery/data)
- **Manual only** - No auto-refresh (you must pull to refresh manually)

**Recommendation:** **Every 1 minute** for most users. This keeps data current without excessive battery drain.

**Use "Manual only" if:** You're on a limited data plan or want maximum battery conservation.

---

#### Pull to Refresh

**What it does:** This setting is typically always enabled, allowing you to manually refresh any list screen by pulling down.

**Why it exists:** Even with auto-refresh, sometimes you want to force an immediate sync (e.g., you just booked a job on desktop and want to see it on mobile right now).

---

#### Cache Size

**What it does:** Shows how much storage the app is using for cached data (jobs, photos, client info).

**View cache size:**
- Settings > Data & Sync > Cache Size: "142 MB"

**Why cache?** Cached data allows you to view recently accessed jobs and clients even when offline.

**Typical cache size:** 50-300 MB depending on how many jobs you have and how many galleries you've viewed.

---

#### Clear Cache

**What it does:** Deletes all cached data and forces the app to re-download everything from the server.

**When to clear cache:**
- App feels sluggish or slow
- You suspect stale data is being displayed
- App is using too much storage on your device
- You've encountered sync errors

**How to clear cache:**
1. Settings > Data & Sync
2. Tap **Clear Cache**
3. Confirm "Clear Cache?"
4. App clears cache and refreshes data

**What happens:**
- Cached jobs, client info, and thumbnails are deleted
- Next time you open a job, it re-downloads from the server
- Sync may take longer immediately after clearing cache

**You will NOT lose:**
- Your login credentials
- Notification preferences
- App settings

---

#### Data Usage Settings

**Download Limit for Galleries**

**What it does:** Limits how many photos are downloaded when viewing galleries on cellular data.

**Options:**
- **No limit** - Download full-resolution gallery photos (uses lots of data)
- **Thumbnails only** - Only download small preview images (saves data)
- **Wifi only** - Only download full images when on wifi

**Recommendation:** **Wifi only** if you have a limited data plan. Full-resolution photos are large (2-10 MB each), and viewing a 100-photo gallery could use 200-1000 MB of data.

**No limit** if you have unlimited data and want immediate full-resolution access.

---

**Auto-Sync on Cellular**

**What it does:** Controls whether the app syncs data when on cellular (not wifi).

**Options:**
- **Enabled** - Sync on cellular and wifi (default)
- **Wifi only** - Only sync when connected to wifi

**Recommendation:** **Enabled** for most users. The app's data usage is minimal for syncing job details, tasks, and timeline updates.

**Wifi only** if you have a very limited data plan.

---

#### Offline Mode

**The app automatically enters offline mode when you lose internet connection.**

**What works offline:**
- Viewing recently accessed jobs and clients
- Browsing cached calendar dates
- Reviewing screenshots or cached gallery thumbnails

**What doesn't work offline:**
- Loading new jobs or leads
- Marking tasks complete (changes won't sync until online)
- Sending messages or emails
- Recording payments
- Refreshing data

**No manual toggle:** You can't manually enable/disable offline mode—it's automatic based on connectivity.

### Calendar Settings

Configure how the mobile calendar displays and syncs with your device's native calendar app.

#### Sync with Device Calendar

**What it does:** Copies your ShootPath sessions to your iPhone/iPad Calendar (iOS) or Google Calendar (Android).

**Benefits:**
- See ShootPath sessions in your native calendar app
- Get reminders from both apps
- View ShootPath sessions alongside personal events (dentist appointments, kid's soccer games, etc.)

**How to enable:**
1. Settings > Calendar
2. Toggle **Sync with Device Calendar** ON
3. Grant calendar permission when prompted
4. ShootPath creates a calendar called "ShootPath Sessions"

**What syncs:**
- Job session dates and times
- Mini session event slots
- Blocked time (if configured)

**What doesn't sync:**
- Tasks or workflow deadlines
- Payment due dates
- Gallery delivery dates

**Two-way or one-way?** Typically one-way (ShootPath → Device Calendar). Changes you make in ShootPath update the device calendar, but you cannot edit sessions from your device calendar.

---

#### Default Calendar View

**What it does:** Sets which view opens when you tap the Calendar tab.

**Options:**
- **Week View** - 7-day horizontal scroll with time slots
- **Month View** - Full month at a glance with session dots

**Recommendation:** Choose whichever you prefer. The app remembers your preference.

**Week view** is great for detail (see exact times and durations).
**Month view** is great for broad planning (see the full month's bookings).

---

#### First Day of Week

**What it does:** Sets whether weeks start on Sunday or Monday.

**Options:**
- **Sunday** (US standard)
- **Monday** (International standard)

**Recommendation:** Match your regional preference or personal habit.

---

#### Time Zone Handling

**What it does:** Controls how session times are displayed when you travel across time zones.

**Options:**
- **Use session time zone** - Sessions always display in the time zone they were created in (e.g., a New York wedding always shows Eastern Time)
- **Use device time zone** - Sessions convert to your current time zone

**Recommendation:** **Use session time zone** for most photographers. If you shoot a destination wedding in Hawaii, you want the session to show Hawaii time, not your home time zone.

**Use device time zone** if you frequently travel and want all times converted to your current location.

---

#### Calendar Color Coding

**What it does:** Assigns colors to different job types for visual distinction.

**Typical color scheme:**
- Weddings: Red
- Portraits: Blue
- Corporate: Green
- Mini-sessions: Purple

**Can you customize colors on mobile?** No—color configuration is done on desktop (Settings > Job Types). Mobile displays the colors you've set.

### Security Settings

Protect your account and control access to sensitive client data.

#### Biometric Login

**What it does:** Allows you to log in using Face ID (iOS) or Fingerprint / Face Unlock (Android) instead of typing your password every time.

**How to enable:**
1. Settings > Security
2. Toggle **Enable Biometric Login**
3. Authenticate with Face ID / Touch ID / Fingerprint to confirm
4. From now on, the app opens with biometric authentication

**Benefits:**
- Faster login (no typing password)
- More secure than a short/simple password
- Convenient for quick checks

**Fallback:** If biometric fails (e.g., you're wearing a mask, sensor doesn't recognize you), you can tap "Use Password" and type your password manually.

---

#### Session Timeout

**What it does:** Logs you out automatically after a period of inactivity.

**Default:** 14 days of inactivity

**Why?** If your phone is lost or stolen weeks later, the app won't allow access to your account without re-authentication.

**Can you customize?** Not on mobile—this is a system-wide security setting configured on desktop.

---

#### Change Password

**Access:** Settings > Security > Change Password

**How to change:**
1. Tap **Change Password**
2. Enter current password
3. Enter new password (8+ characters, mix of letters/numbers)
4. Confirm new password
5. Save

**Why change on mobile?** Rare—most users change passwords on desktop. But if you suspect your account was compromised while traveling, you can change it immediately on mobile.

---

#### Revoke All Mobile Sessions

**What it does:** Logs out all mobile devices currently logged into your account (useful if your phone is lost/stolen).

**Access:** Desktop only (not available on mobile for security reasons)

**How to do it from desktop:**
1. Log in to ShootPath on desktop
2. Go to Settings > Security
3. Click **Revoke All Mobile Sessions**
4. All mobile devices are logged out remotely

**When to use:** Your phone is stolen and you want to ensure the thief cannot access your account.

---

#### Two-Factor Authentication (2FA)

**What it does:** Requires a verification code (from an app like Google Authenticator) in addition to your password.

**Currently supported?** Check your ShootPath instance. Some self-hosted instances support 2FA; others may not yet.

**If supported:**
1. Enable on desktop (Settings > Security > Two-Factor Authentication)
2. On mobile, you'll be prompted for a verification code after entering your password

**Recommendation:** **Enable 2FA** if available. It significantly improves account security.

### Appearance Settings

Customize the visual experience of the mobile app.

#### Light / Dark Mode

**What it does:** Changes the app's color scheme.

**Options:**
- **Light Mode** - Light backgrounds, dark text (default)
- **Dark Mode** - Dark backgrounds, light text (easier on eyes at night)
- **Follow System** - Match your device's system-wide appearance setting (recommended)

**Recommendation:** **Follow System** so the app automatically switches when your device switches (e.g., dark mode at night, light mode during the day).

---

#### Color Scheme Preferences

**What it does:** Some versions allow you to customize accent colors.

**Typical options:**
- Default brand colors (amber/stone for ShootPath)
- Custom accent color picker

**Note:** This is rare on mobile—most color customization happens on desktop.

---

#### Text Size

**What it does:** Adjusts font size for better readability.

**Options:**
- Small
- Medium (default)
- Large
- Extra Large

**Who should adjust?** Users with visual impairments or anyone who prefers larger text for easier reading.

**Where to find:** Settings > Appearance > Text Size (or use device-wide accessibility settings)

### About & Support

Access app information, legal documents, and support resources.

#### App Version

**What it shows:** Current version number (e.g., "ShootPath Mobile v2.4.1")

**Why check?** When contacting support, they'll ask for your app version to diagnose issues.

**Where to find:** Settings > About > App Version

---

#### Check for Updates

**What it does:** Checks if a newer version is available.

**How it works:**
- **iOS:** App Store handles updates automatically (if auto-update is enabled)
- **Android:** Google Play Store handles updates automatically (if enabled)

**Manual update:**
1. Open App Store (iOS) or Play Store (Android)
2. Search "ShootPath"
3. Tap **Update** if available

**Should you update?** Yes—updates include bug fixes, performance improvements, and new features.

---

#### Privacy Policy

**What it is:** Link to ShootPath's privacy policy explaining how your data is handled.

**Where to find:** Settings > About > Privacy Policy

**When to read:** Before signing up, or if you have concerns about data usage.

---

#### Terms of Service

**What it is:** Legal agreement between you and ShootPath.

**Where to find:** Settings > About > Terms of Service

---

#### Help & Support

**What it does:** Opens support resources.

**Options:**
- **Help Center** - Link to docs.shootpath.com (this documentation site)
- **Contact Support** - Opens email composer to support@shootpath.com
- **Live Chat** (if available) - Opens help widget for real-time chat

**When to use:** If you encounter a bug, have a feature request, or need technical assistance.

---

#### Send Feedback

**What it does:** Allows you to submit feedback about the mobile app directly from within the app.

**How to send feedback:**
1. Settings > About > Send Feedback
2. Describe your feedback (feature request, bug report, general comment)
3. Optionally attach a screenshot
4. Submit

**Your feedback helps improve the app!** The team reviews all submissions.

### Account Management

Manage your logged-in account and switch between studios (if multi-tenant).

#### Switch Studio / Tenant

**What it does:** If you belong to multiple photography studios (e.g., you assist for another photographer or run two businesses), you can switch between them.

**How to switch:**
1. Tap **More**
2. Tap **Switch Studio** (or **Switch Tenant**)
3. Select the studio you want to access
4. The app refreshes with that studio's data (jobs, leads, calendar, etc.)

**Data isolation:** Each studio's data is completely separate. Switching studios does NOT merge or mix data.

---

#### Log Out

**What it does:** Logs you out of the mobile app.

**When to log out:**
- Selling or giving away your device
- Letting someone else use the app temporarily (not recommended—use separate accounts instead)
- Troubleshooting login issues

**How to log out:**
1. Tap **More**
2. Scroll to bottom
3. Tap **Log Out**
4. Confirm

**What happens:**
- You're logged out
- Cached data remains (but cannot be accessed without logging back in)
- Notification settings are preserved

**To fully clear data:** Log out, then uninstall and reinstall the app.

---

#### Delete Account

**Can you delete your account from mobile?** No—account deletion requires desktop access (Settings > Account > Delete Account).

**Why?** Account deletion is a destructive action that requires careful confirmation on a full-screen interface.

### Troubleshooting Mobile Issues

Common problems and how to resolve them using settings or other actions.

#### Problem: App is Slow or Laggy

**Possible causes:**
- Large cache
- Old app version
- Low device storage

**Solutions:**

**1. Clear cache:**
- Settings > Data & Sync > Clear Cache

**2. Update the app:**
- Check App Store / Play Store for updates

**3. Free up device storage:**
- Delete unused apps, photos, or videos from your device (not ShootPath-related)

**4. Restart the app:**
- Force close and reopen

**5. Restart your device:**
- Power off and power on your phone

---

#### Problem: Sync is Failing

**Symptoms:**
- Red "Sync failed" indicator on Dashboard
- Data not updating after pulling to refresh
- Changes not syncing to desktop

**Solutions:**

**1. Check internet connection:**
- Open Safari (iOS) or Chrome (Android) and load a website to confirm connectivity

**2. Switch networks:**
- If on wifi, try switching to cellular (or vice versa)
- Some public wifi networks block certain ports ShootPath uses

**3. Re-login:**
- Log out and log back in to refresh authentication tokens

**4. Clear cache and force refresh:**
- Settings > Data & Sync > Clear Cache
- Pull down on Dashboard to force refresh

**5. Contact support:**
- If sync fails persist, the server might be down or experiencing issues
- Check status.shootpath.com (if available) or contact support

---

#### Problem: Notifications Not Appearing

**Symptoms:**
- You expect a notification (new lead, payment received) but don't receive it

**Solutions:**

**1. Check notification settings in ShootPath:**
- Settings > Notifications
- Ensure the notification type is enabled (e.g., "New Leads" is ON)

**2. Check device notification permissions:**

**iOS:**
1. Device Settings > ShootPath
2. Ensure "Notifications" is enabled
3. Check "Allow Notifications" is toggled ON

**Android:**
1. Device Settings > Apps > ShootPath > Notifications
2. Ensure notifications are enabled

**3. Disable Quiet Hours:**
- If you have Quiet Hours enabled, notifications are silenced during those times

**4. Test notifications:**
- On desktop, create a test lead or record a test payment
- Check if notification appears on mobile within 30 seconds

---

#### Problem: Biometric Login Not Working

**Symptoms:**
- Face ID / Touch ID / Fingerprint fails repeatedly
- App keeps asking for password

**Solutions:**

**1. Ensure biometric is set up on your device:**
- iOS: Settings > Face ID & Passcode (or Touch ID)
- Android: Settings > Security > Fingerprint / Face Unlock

**2. Re-enable biometric login in ShootPath:**
- Settings > Security > Toggle "Enable Biometric Login" OFF
- Toggle back ON and re-authenticate

**3. Update the app:**
- Biometric issues are sometimes fixed in app updates

**4. Use password as fallback:**
- Tap "Use Password" and log in manually

---

#### Problem: App Crashes on Launch

**Symptoms:**
- App opens briefly then closes
- Black screen or immediate crash to home screen

**Solutions:**

**1. Restart your device:**
- Power off and back on

**2. Update the app:**
- Outdated versions may crash on newer iOS/Android versions

**3. Reinstall the app:**
- Uninstall ShootPath
- Reinstall from App Store / Play Store
- Log back in (your data is safe on the server)

**4. Check device compatibility:**
- Ensure your device meets minimum requirements (iOS 17+ or Android 10+)

---

#### Problem: Cannot Load Photos in Galleries

**Symptoms:**
- Gallery thumbnails load but full-resolution images don't
- "Failed to load image" error

**Solutions:**

**1. Check data usage settings:**
- Settings > Data & Sync > Download Limit for Galleries
- Ensure it's not set to "Thumbnails only" if you want full images

**2. Use wifi:**
- Connect to wifi and try loading again

**3. Clear cache:**
- Settings > Data & Sync > Clear Cache
- Re-open the gallery

**4. Check storage:**
- Ensure your device has enough free storage to download images

---

#### Problem: Session Not Showing in Calendar

**Symptoms:**
- Session exists on desktop but doesn't appear in mobile calendar

**Solutions:**

**1. Force refresh:**
- Go to Calendar tab
- Pull down to refresh

**2. Check date:**
- Verify the session date is within the visible calendar range
- Swipe to the correct week/month

**3. Check filters:**
- If calendar has filters (e.g., job type), ensure the session's job type is included

**4. Sync issue:**
- Check sync status on Dashboard (should be green checkmark)
- If sync is failing, resolve sync issues first

### Best Practices for Mobile Settings

**Recommended Configuration for Most Photographers:**

**Notifications:**
- ✅ New Leads: ON
- ✅ Session Reminders: ON (both 1 day and 1 hour)
- ✅ Payments Received: ON
- ✅ Contracts Signed: ON
- ❌ Gallery Activity: OFF (unless you actively track engagement)
- ✅ Overdue Payments: ON
- ❌ Task Reminders: OFF (unless you rely on push reminders for task management)

**Data & Sync:**
- Auto-Refresh: Every 1 minute
- Cache: Clear every 3-6 months (or when app feels slow)
- Download Limit: Wifi only (save cellular data)

**Calendar:**
- Sync with Device Calendar: ON (so you see sessions in native calendar)
- Default View: Week View (shows detail)
- First Day of Week: Match your preference
- Time Zone: Use session time zone

**Security:**
- Biometric Login: ON (faster and more secure)
- Change Password: Every 6-12 months

**Appearance:**
- Light/Dark Mode: Follow System (automatic)

**Why this configuration?**

This setup keeps you informed of critical events (leads, payments, sessions) without overwhelming you with notifications. Data usage is optimized for cellular, sync is fast, and security is strong.

### Keeping Your Mobile App Updated

**Auto-updates (recommended):**

**iOS:**
1. Device Settings > App Store
2. Toggle **App Updates** ON

**Android:**
1. Play Store > Menu > Settings
2. Toggle **Auto-update apps** > Over wifi only (or any network)

**Why auto-update?**

You'll always have the latest features, bug fixes, and security patches without manual intervention.

---

**Manual updates:**

If you prefer to control when updates happen:
1. Check App Store / Play Store weekly
2. Manually tap "Update" when new versions are available

**Release notes:**

When updating, read the release notes to see what's new:
- New features
- Bug fixes
- Performance improvements
- Known issues

### What's Next?

Now that you've configured your mobile settings, explore these related articles:

**[Mobile Overview](./index)** - Getting started with ShootPath mobile

**[Mobile Features](./mobile-features)** - Complete guide to all mobile capabilities

**[On-Location Workflows](./on-location-workflows)** - Using mobile during photo shoots

**Related Topics:**

**[Account Setup](../account-setup/)** - Initial account configuration (done on desktop)

**[Notifications](../getting-started/notifications)** - Understanding notification system across platforms

---

**Questions?** Contact support via the help widget or email support@shootpath.com!
