---
sidebar_position: 5
---

# Sync Issues

## Quick Reference

Having problems with calendar sync or mobile app synchronization? This guide covers common sync issues between ShootPath and Google Calendar, as well as mobile app sync problems.

**Common Sync Issues:**
- Calendar sync not working → Reconnect Google Calendar integration
- Events not appearing → Check sync settings and calendar selection
- Duplicate events → Clear and re-sync calendar
- Time zone problems → Verify time zone settings match
- Mobile app not syncing → Check internet connection and app version

**Quick Troubleshooting:**
1. Check Google Calendar connection: **Settings → Integrations → Google Calendar** (should show "Connected")
2. Force sync: Click **Sync Now** in Settings
3. Check internet connection
4. Update mobile app to latest version
5. Log out and log back in

:::tip Most Common Causes
90% of sync issues are caused by:
1. Google Calendar not connected or connection expired (check Settings → Integrations)
2. Wrong calendar selected in sync settings
3. Mobile app needs updating (check App Store/Play Store)
:::

---

## Detailed Guide

### Calendar Sync Not Working

If jobs aren't appearing in Google Calendar or vice versa:

**Step 1: Check Integration Status**

1. Go to **Settings → Integrations**
2. Find **Google Calendar** section
3. Check status:
   - **Connected** (green checkmark) - Integration is working
   - **Not Connected** or **Disconnected** (red X) - Integration needs setup/reconnection

**If Not Connected:**
You must connect Google Calendar before syncing works. See [Connecting Google Calendar](#connecting-google-calendar) below.

**Step 2: Verify Sync Settings**

1. Go to **Settings → Integrations → Google Calendar**
2. Check **Sync Direction**:
   - **Two-way sync**: ShootPath ↔ Google Calendar (recommended)
   - **ShootPath to Calendar only**: ShootPath → Google Calendar
   - **Calendar to ShootPath only**: Google Calendar → ShootPath
3. Check **Which calendar to sync**:
   - Make sure the correct Google Calendar is selected
   - Default is usually "Primary"
4. Check **What to sync**:
   - Jobs
   - Appointments
   - Meetings
   - All events (recommended)

**Step 3: Force a Sync**

1. Stay in **Settings → Integrations → Google Calendar**
2. Click **Sync Now** button
3. Wait 1-2 minutes
4. Check Google Calendar to see if events appear

**Step 4: Check Sync Logs**

1. Scroll down to **Recent Sync Activity**
2. You'll see:
   - Last sync time
   - Events synced
   - Errors (if any)
3. If errors:
   - Click error for details
   - Common errors and solutions below

**Common Sync Errors:**

**Error: "Authentication expired"**
- Google Calendar connection needs reauthorization
- Solution: Click **Reconnect Google Calendar**

**Error: "Calendar not found"**
- Selected calendar was deleted in Google
- Solution: Go to sync settings, select a different calendar

**Error: "Quota exceeded"**
- Too many sync requests in short time
- Solution: Wait 30 minutes, then try again

**Error: "Permission denied"**
- ShootPath doesn't have permission to access the calendar
- Solution: Reconnect Google Calendar and grant full permissions

### Connecting Google Calendar

If Google Calendar isn't connected or needs reconnecting:

**Step 1: Start Connection**
1. Go to **Settings → Integrations**
2. Find **Google Calendar** section
3. Click **Connect Google Calendar**

**Step 2: Choose Google Account**
- You'll be redirected to Google sign-in
- Choose the Google account with the calendar you want to sync
- This should be your business Google account

**Step 3: Authorize ShootPath**
Google will show: "ShootPath wants to access your Google Calendar"

**Permissions requested:**
- View events on all your calendars
- Create, edit, and delete events
- View and edit settings for all calendars

These permissions are necessary for two-way sync.

Click **Allow**.

**Step 4: Configure Sync Settings**

After connecting:
1. Choose **Sync Direction**:
   - **Two-way**: Recommended (changes in either place sync to the other)
   - **ShootPath to Calendar**: Job dates appear in Google Calendar but not vice versa
   - **Calendar to ShootPath**: Google Calendar events import to ShootPath but ShootPath doesn't update Calendar
2. Choose **Which Calendar** to sync:
   - Primary (your main calendar)
   - Or select a different calendar
3. Choose **What to Sync**:
   - Jobs (shoot dates, meetings, deliveries)
   - All events (recommended)
4. Click **Save Settings**

**Step 5: Initial Sync**
- ShootPath immediately syncs existing jobs to Google Calendar
- This may take 1-2 minutes if you have many jobs
- Check Google Calendar to confirm events appeared

**If Authorization Fails:**

**Error: "This app isn't verified by Google"**
- Click **Advanced** → **Go to ShootPath (unsafe)**
- It's safe - we're working on full Google verification

**Error: "Access blocked"**
- Google Workspace admin may have blocked third-party apps
- Solution: Ask IT admin to whitelist ShootPath in Google Workspace admin console

### Events Not Appearing in Google Calendar

If jobs exist in ShootPath but don't show in Google Calendar:

**Step 1: Verify Sync is Enabled**

1. Go to **Settings → Integrations → Google Calendar**
2. Check sync direction:
   - Must be "Two-way sync" or "ShootPath to Calendar only"
   - If set to "Calendar to ShootPath only," jobs won't sync to Google
3. Click **Sync Now**

**Step 2: Check Job Has a Date**

Calendar sync only works for jobs with shoot dates:
1. Go to the job in ShootPath
2. Check **Shoot Date** field
3. If empty, add a date
4. Wait 15 minutes for sync (or click Sync Now in settings)

**Step 3: Check Correct Calendar is Selected**

In Google Calendar:
1. Left sidebar shows all your calendars
2. Make sure the calendar you selected in ShootPath sync settings is VISIBLE (checked)
3. Common issue: Selected calendar is hidden in Google Calendar view

**Step 4: Check Sync Direction**

If you recently changed sync direction:
- Events only sync going forward from the change
- Past events won't retroactively sync
- Solution: Force sync all events (see below)

**Force Sync All Events:**
1. Go to **Settings → Integrations → Google Calendar**
2. Click **Advanced Options**
3. Click **Resync All Events**
4. Confirm
5. All job dates will re-sync to Google Calendar

:::warning Resync Creates Duplicates
If you already have some events synced, Resync All might create duplicates. See [Duplicate Events](#duplicate-events) section for how to fix.
:::

### Events Not Appearing in ShootPath

If events exist in Google Calendar but don't show in ShootPath:

**Step 1: Verify Sync Direction**

1. Go to **Settings → Integrations → Google Calendar**
2. Check sync direction:
   - Must be "Two-way sync" or "Calendar to ShootPath only"
   - If set to "ShootPath to Calendar only," Google Calendar events won't import
3. Change to "Two-way sync"
4. Click **Sync Now**

**Step 2: Check Event Type**

ShootPath only imports certain event types:
- **Imports:** Events you created or were invited to
- **Doesn't import:** All-day reminders, birthdays from contacts

**Step 3: Check Event Calendar**

In ShootPath sync settings:
1. Check **Which calendar to sync**
2. If you have multiple calendars in Google, only the selected one syncs
3. If events are in a different calendar:
   - Change sync settings to that calendar
   - Or move events to the synced calendar in Google

**Step 4: Manual Import**

For one-time import of Google Calendar events:
1. Go to **Settings → Integrations → Google Calendar**
2. Click **Import Events from Google Calendar**
3. Choose date range (e.g., "Next 90 days")
4. Click **Import**
5. Events will create jobs or appointments in ShootPath

### Duplicate Events

If you see duplicate entries in Google Calendar or ShootPath:

**Causes:**
- Synced multiple times
- Changed sync settings multiple times
- Connected/disconnected multiple times
- Manually created same event in both places

**Solution 1: Clear and Resync (Recommended)**

**In Google Calendar:**
1. Filter to show only "ShootPath" events
2. Select all
3. Delete all
4. In ShootPath: **Settings → Integrations → Google Calendar → Resync All Events**

**In ShootPath:**
- Duplicates are harder to fix
- You'll need to manually delete duplicate jobs/appointments
- Or: Export jobs to CSV, delete all, re-import deduplicated list

**Solution 2: Use Calendar Event IDs (Advanced)**

ShootPath stores Google Calendar event IDs:
1. Go to **Settings → Integrations → Google Calendar**
2. Click **Advanced Options**
3. Click **Clean Up Duplicates**
4. ShootPath will:
   - Find events with same date/title in both systems
   - Keep the one with matching event ID
   - Delete the duplicate

This works for most cases.

**Preventing Duplicates:**
- Don't manually create the same event in both ShootPath and Google Calendar
- Let sync handle it automatically
- If changing sync settings, clear events first, then resync

### Time Zone Problems

If events appear at wrong times in Google Calendar:

**Step 1: Check ShootPath Time Zone**

1. Go to **Settings → Business Information**
2. Check **Time Zone** field
3. Should match your local time zone
4. If wrong, update it and click **Save**

**Step 2: Check Google Calendar Time Zone**

1. Go to Google Calendar settings (gear icon → Settings)
2. Click **General** in left sidebar
3. Check **Time zone**
4. Should match your local time zone
5. Also check **Display secondary time zone** (turn off if you don't need it)

**Step 3: Resync Events**

After fixing time zones:
1. Go to **Settings → Integrations → Google Calendar**
2. Click **Advanced Options → Resync All Events**
3. Events will update with correct times

**Common Time Zone Issues:**

**Issue: Events Show 3 Hours Early/Late**
- You're in Eastern (EST) but Google Calendar is set to Pacific (PST) or vice versa
- Or: ShootPath is set to one time zone, Google is set to another
- Solution: Make sure both use the same time zone

**Issue: Events Change Time During Daylight Saving**
- One system didn't account for daylight saving time
- Solution: Make sure both ShootPath and Google Calendar auto-adjust for DST
- Check after DST changes (March and November in US)

**Issue: All-Day Events Span Two Days**
- Time zone mismatch causing all-day event to start at 11pm previous day
- Solution: Fix time zones in both systems and resync

### Mobile App Sync Issues

If ShootPath mobile app isn't syncing:

**Step 1: Check Internet Connection**

- Mobile app requires internet to sync (no offline mode yet)
- Try:
  - Open a website in your browser to confirm internet works
  - Switch between WiFi and cellular
  - Turn airplane mode on, wait 10 seconds, turn off

**Step 2: Force App Sync**

**iOS:**
1. In ShootPath app, pull down on any list (clients, jobs, etc.)
2. Release to trigger refresh
3. Wait for spinning indicator to stop

**Android:**
1. Same as iOS - pull down to refresh
2. Or: Tap menu (three dots) → Sync Now

**Step 3: Update the App**

**iOS:**
1. Open App Store
2. Tap profile icon (top right)
3. Scroll to ShootPath
4. Tap **Update** if available

**Android:**
1. Open Google Play Store
2. Tap menu (three lines) → My apps & games
3. Find ShootPath
4. Tap **Update** if available

**Step 4: Clear App Cache**

**iOS:**
- Delete the app and reinstall from App Store
- Your data is safe (stored on servers)
- Log back in after reinstalling

**Android:**
1. Settings → Apps → ShootPath
2. Storage → Clear cache (don't clear data yet)
3. Open app and try syncing

**Step 5: Log Out and Log Back In**

1. In ShootPath app: Profile → Log Out
2. Log back in
3. App will re-sync all data

**Step 6: Check App Permissions**

**iOS:**
1. Settings → ShootPath
2. Make sure these are enabled:
   - Background App Refresh
   - Cellular Data (if you use cellular)
3. Toggle them off and back on

**Android:**
1. Settings → Apps → ShootPath → Permissions
2. Make sure these are allowed:
   - Internet
   - Network access
3. Settings → Data usage → ShootPath
4. Make sure "Background data" is enabled

**Common Mobile Sync Errors:**

**Error: "Could not connect to server"**
- Internet connection issue
- ShootPath servers may be down (check [status.shootpath.com](https://status.shootpath.com))
- Solution: Check internet, wait a few minutes, try again

**Error: "Session expired"**
- You were logged out due to inactivity
- Solution: Log back in

**Error: "Sync conflict detected"**
- You edited the same job on web and mobile at the same time
- Solution: App will show conflict resolution screen - choose which version to keep

**Error: "Storage full"**
- Your device doesn't have enough space for cached photos
- Solution: Free up device storage, clear app cache

### Google Calendar Two-Way Sync

Understanding how two-way sync works:

**ShootPath to Google Calendar:**
- When you create/edit a job in ShootPath with a shoot date, it creates/updates an event in Google Calendar
- Event title: [Job type] - [Client name]
- Event time: Shoot date + time (or all-day if no time specified)
- Event description: Job details, client contact, location
- Sync happens within 15 minutes (or immediately if you click Sync Now)

**Google Calendar to ShootPath:**
- When you create an event in Google Calendar, it creates an appointment in ShootPath
- Appointment title: Same as event title
- Appointment time: Same as event time
- Sync happens within 15 minutes

**Editing Synced Events:**

**If You Edit in ShootPath:**
- Change syncs to Google Calendar within 15 minutes
- Title, date, time, location all update

**If You Edit in Google Calendar:**
- Change syncs to ShootPath within 15 minutes
- But: Some fields may not sync (depends on what changed)
- Complex changes: Safer to edit in ShootPath

**Deleting Synced Events:**

**If You Delete in ShootPath:**
- Job deletion doesn't automatically delete Google Calendar event
- Manually delete in Google Calendar, or click "Sync Now" to clean up

**If You Delete in Google Calendar:**
- Event deletion doesn't delete the job in ShootPath
- Appointment (not job) may be deleted if it was created from Google Calendar

**Best Practice:**
- Create and edit jobs in ShootPath (more reliable)
- Use Google Calendar primarily for viewing
- Only create simple events in Google Calendar if needed

### Calendar Sync Delays

Sync isn't instant - here's what to expect:

**Normal Sync Frequency:**
- Automatic sync every 15 minutes
- When you create/edit a job: Syncs within 15 minutes
- Manual "Sync Now": Immediate (within 1-2 minutes)

**Why 15-Minute Delay?**
- Google Calendar API has rate limits
- Syncing too frequently could hit the limit and stop working
- 15 minutes is a good balance between freshness and reliability

**When Sync is Slower:**
- High API usage (many ShootPath users syncing at once)
- Google Calendar servers are slow
- Large number of events to sync (100+ jobs)

**If Sync Takes Longer Than 30 Minutes:**
- Check sync logs for errors
- Try manual "Sync Now"
- Disconnect and reconnect Google Calendar
- Contact support if it persists

### Disabling Calendar Sync

If you want to stop syncing:

**Option 1: Disconnect Google Calendar**
1. Go to **Settings → Integrations → Google Calendar**
2. Click **Disconnect**
3. Confirm
4. Syncing stops immediately

**What Happens:**
- No more changes sync between ShootPath and Google
- Existing events remain in Google Calendar (not deleted)
- Jobs remain in ShootPath (not deleted)

**Option 2: Pause Syncing Temporarily**
1. Go to **Settings → Integrations → Google Calendar**
2. Click **Pause Sync**
3. Syncing stops but connection remains
4. Click **Resume Sync** when ready

**Option 3: Change to One-Way Sync**
1. Go to sync settings
2. Change sync direction:
   - "ShootPath to Calendar only" - stops importing from Google
   - "Calendar to ShootPath only" - stops exporting to Google
3. Useful if you want partial sync

**Cleaning Up After Disconnecting:**

**In Google Calendar:**
- ShootPath events remain
- Manually delete them if you don't want them
- Or: Create a filter, select all, delete

**In ShootPath:**
- Jobs and appointments remain
- No automatic cleanup needed

---

## Common Questions

**How often does calendar sync?**
Automatically every 15 minutes. You can force immediate sync by clicking "Sync Now" in Settings → Integrations → Google Calendar.

**Can I sync with other calendars (Outlook, Apple Calendar)?**
Currently only Google Calendar is supported. However:
- Outlook: Can subscribe to ShootPath's iCal feed (Settings → Calendar Feed)
- Apple Calendar: Can subscribe to ShootPath's iCal feed
- These are one-way read-only (ShootPath → Calendar)

**Do I need Google Workspace or can I use free Gmail?**
Free Gmail works perfectly! You don't need a paid Google Workspace account.

**Can I sync multiple Google Calendars?**
Currently you can only sync one Google Calendar at a time. To switch:
1. Go to sync settings
2. Change "Which calendar to sync"
3. Past events stay in old calendar (won't move)

**What if I share my Google Calendar with others?**
They'll see your synced ShootPath jobs/appointments as events. Make sure you're comfortable with them seeing:
- Client names
- Job types
- Shoot dates and times

**Can I control what details appear in Google Calendar events?**
Yes:
1. Go to **Settings → Integrations → Google Calendar**
2. Click **Advanced Options → Event Template**
3. Customize title and description
4. Use variables: \{\{client_name\}\}, \{\{job_type\}\}, \{\{shoot_date\}\}

**Why do events disappear from Google Calendar?**
Possible reasons:
- Job was deleted in ShootPath
- Shoot date was removed from job
- Sync direction was changed
- Calendar was accidentally hidden in Google Calendar view

**Can I sync to my team members' calendars?**
Not directly. But you can:
- Share your Google Calendar with team members
- They'll see your synced events
- Or: Use Google Workspace shared calendars

**What happens if I delete a job in ShootPath?**
- Job is deleted from ShootPath
- Google Calendar event remains (not auto-deleted)
- You'll need to manually delete from Google Calendar
- Or: Click "Sync Now" and ShootPath will clean up deleted events

---

## Still Having Sync Issues?

**Contact Support:**

**For ShootPath Sync Issues:**
Email [support@shootpath.com](mailto:support@shootpath.com)
- Include: Sync logs screenshot, what's not syncing, steps you tried

**For Google Calendar Issues:**
Contact Google support: [support.google.com/calendar](https://support.google.com/calendar)

**For Mobile App Issues:**
- iOS: Email with "iOS sync issue" in subject
- Android: Email with "Android sync issue" in subject
- Include: App version, device model, Android/iOS version

We'll help get your sync working smoothly across all devices!
