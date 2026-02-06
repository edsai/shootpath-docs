---
sidebar_position: 3
---

# Calendar Integrations

Learn how to sync your ShootPath calendar with Google Calendar, iCal, and other external calendars for seamless scheduling across all your devices.

## Quick Reference

**Integration Options:**
- **Google Calendar sync** - Two-way sync between ShootPath and Google
- **iCal feed** - One-way sync from ShootPath to Apple Calendar, Outlook, etc.
- **Calendar subscription** - Read-only feed for viewing ShootPath events elsewhere

**Sync Types:**
- **Two-way sync** - Changes in either calendar update the other (Google Calendar only)
- **One-way sync** - ShootPath events appear in external calendar, but changes don't sync back

**What Syncs:**
- Job sessions with dates and times
- Mini session events
- Blocked time (optional)
- Session locations and notes

**What Doesn't Sync:**
- Tasks and to-dos
- Client contact information
- Financial details
- Internal notes marked as private

**Best For:**
- Viewing your ShootPath schedule on your phone
- Coordinating with personal calendar events
- Sharing availability with family/team
- Ensuring you don't double-book across calendars

---

## Why Calendar Integration Matters

### The Problem Without Integration

You have multiple calendars:
- ShootPath calendar (work sessions)
- Google Calendar (personal appointments, meetings)
- Apple Calendar (family events)
- Outlook (if you have a day job or corporate clients)

**What happens:**
- You book a client session in ShootPath
- But forget you have a dentist appointment that day in Google Calendar
- Result: Double-booked and stressed

**Or:**
- Client asks if you're free Saturday at 2pm
- You check ShootPath: "Yes, I'm free!"
- But you forget your kid's soccer game is at 2pm (in your personal calendar)
- Result: Conflict and unhappy family

### The Solution: Calendar Sync

**With calendar integration:**
- Your ShootPath sessions appear in Google Calendar automatically
- You can see work + personal events in one view
- Checking availability is instant and accurate
- No more double-booking across different calendar systems

**Real-world example:**
You wake up, check your phone's default calendar app (Google Calendar or Apple Calendar), and see:
- 9am: Dentist (personal)
- 11am: Smith Family Portrait (ShootPath session)
- 2pm: Kid's soccer game (personal)
- 5pm: Editing block (ShootPath blocked time)

Everything in one place. You know exactly what your day looks like.

## Google Calendar Integration

Google Calendar offers two-way sync, making it the most powerful integration option.

### How Two-Way Sync Works

**ShootPath → Google Calendar:**
- Schedule a session in ShootPath
- Session appears in Google Calendar within minutes
- All details sync: title, time, location, notes

**Google Calendar → ShootPath:**
- Block time in Google Calendar (e.g., "Dentist appointment")
- ShootPath sees that time as busy
- Prevents scheduling client sessions during that time

**Benefits:**
- Update in either place, sync everywhere
- One source of truth for your availability
- Family/assistants can see your Google Calendar and know when you're busy

### Setting Up Google Calendar Sync

**Prerequisites:**
- Google account (Gmail)
- Access to ShootPath Settings

**Step-by-step setup:**

**1. Go to Settings > Integrations**
- Navigate to **Settings** (gear icon)
- Click **Integrations**
- Find **Google Calendar** section

**2. Click "Connect Google Calendar"**
- A popup window opens
- You'll be redirected to Google's authorization page

**3. Authorize ShootPath**
- Log in to your Google account (if not already logged in)
- Google asks: "ShootPath wants to access your Google Calendar. Allow?"
- Review permissions:
  - View your calendars
  - Create, edit, and delete events
  - See event details
- Click **Allow**

**4. Choose which calendar to sync**
- If you have multiple Google calendars (Work, Personal, Photography, etc.)
- Choose which one to sync with ShootPath
- Most photographers choose: "Create new calendar called 'ShootPath'"
- This keeps work events separate from personal

**5. Configure sync settings**
- **Sync frequency:** Real-time (recommended) or hourly
- **What to sync:**
  - ☑ Job sessions
  - ☑ Mini session events
  - ☑ Blocked time
  - ☐ Tasks (optional, usually off)
- **Event visibility:** Public, Private, or Default
- **Sync past events:** Choose how far back to sync (usually 30 days)

**6. Save and verify**
- Click **Save Settings**
- ShootPath begins initial sync (may take 1-2 minutes)
- Check Google Calendar to verify your ShootPath events appear

**Initial sync:**
After connecting, ShootPath syncs all existing sessions. This might take a few minutes if you have many scheduled events. You'll see a progress indicator.

### Managing Google Calendar Sync

**View sync status:**
Go to **Settings > Integrations > Google Calendar** to see:
- ✅ Connected and syncing
- Last sync time (e.g., "2 minutes ago")
- Number of events synced
- Any errors or warnings

**Pause sync temporarily:**
If you need to stop syncing temporarily (e.g., during data cleanup):
1. Click **Pause Sync**
2. Make your changes in ShootPath
3. Click **Resume Sync** when ready

**Disconnect Google Calendar:**
If you want to stop syncing entirely:
1. Click **Disconnect**
2. Confirm: "Are you sure? Existing synced events will remain in Google Calendar but won't update anymore."
3. Events remain in both calendars but stop syncing

**Reconnect later:**
You can reconnect anytime. Choose whether to:
- Sync all events again (creates duplicates if old events still exist)
- Sync only new events going forward

### Two-Way Sync Best Practices

**Use ShootPath as primary for client sessions:**
- Always create client sessions in ShootPath first
- This ensures all job details, workflows, and payments are linked correctly
- The session then syncs to Google Calendar

**Use Google Calendar for personal events:**
- Add personal appointments, family events, and non-photography commitments to Google Calendar
- ShootPath sees these as "busy" times and prevents booking

**Don't edit synced events in Google Calendar:**
Technically you can, but it's confusing:
- If you edit a ShootPath session in Google Calendar (change time, location)
- The change syncs back to ShootPath
- But you lose context (which job is it? client details?)
- **Better:** Edit sessions in ShootPath where you have full context

**Exception - Blocking time:**
Feel free to add blocked time in either ShootPath or Google Calendar. If you're on-the-go and need to quickly block time for a dentist appointment, add it in Google Calendar. ShootPath respects it.

**Use separate Google calendars:**
If you have multiple Google calendars (Work, Personal, Photography):
- Sync ShootPath to a dedicated "Photography" or "ShootPath" calendar
- Keep personal events in "Personal" calendar
- View all calendars together in Google Calendar app
- But each calendar stays organized and separate

### Handling Conflicts

**What if you accidentally double-book?**

**Scenario 1: Double-book in Google Calendar**
- You already have a ShootPath session at 2pm
- You add a personal appointment at 2pm in Google Calendar
- **Result:** Both events exist, you see the conflict visually in Google Calendar
- **Fix:** Delete or move one of them

**Scenario 2: Double-book in ShootPath**
- You already have a personal appointment at 2pm in Google Calendar
- You try to schedule a ShootPath session at 2pm
- **Result:** ShootPath warns "This time conflicts with existing event" (because it sees the Google Calendar event)
- **Fix:** Choose a different time, or confirm you want to override

**The system prevents most conflicts**, but human error can still create them. Weekly calendar review catches these.

### Troubleshooting Google Calendar Sync

#### Events Not Syncing

**Check:**
1. Is sync still connected? (Settings > Integrations > Google Calendar)
2. Is sync paused?
3. When was last successful sync? (If more than 1 hour ago, there's a problem)

**Common causes:**
- Google authorization expired (need to reconnect)
- Network/connectivity issue
- Google Calendar API rate limit (rare, usually resolves in 10 min)

**Fix:**
1. Click **Refresh Sync** to force an immediate sync
2. If that doesn't work, disconnect and reconnect
3. Contact support if issue persists

#### Duplicate Events

**Why duplicates happen:**
- You disconnected and reconnected, syncing all events again
- Events were manually created in both places
- Sync conflict (rare)

**Fix:**
1. Choose which calendar to trust (usually ShootPath)
2. Delete duplicates from the other calendar
3. Let sync propagate the deletions

**Prevent:**
- Always create client sessions in ShootPath
- Always create personal events in Google Calendar
- Don't manually create same event in both places

#### Wrong Calendar Syncing

**Problem:**
ShootPath events are syncing to your "Personal" calendar instead of your "Work" calendar in Google.

**Fix:**
1. Go to Settings > Integrations > Google Calendar
2. Click **Change Calendar**
3. Select the correct Google calendar
4. Choose whether to:
   - Move existing events to new calendar
   - Leave existing events and sync only new ones to new calendar

#### Deleted Events Reappearing

**Problem:**
You delete a ShootPath event, but it reappears after sync.

**Cause:**
Event was deleted in Google Calendar but still exists in ShootPath (or vice versa).

**Fix:**
Delete the event in both places:
1. Delete in ShootPath
2. Check Google Calendar, delete there too if it still exists
3. Wait for sync to complete

**Two-way sync can be tricky with deletions.** If an event keeps reappearing, try disconnecting sync, cleaning up both calendars, then reconnecting.

## iCal Feed Integration

iCal feeds provide one-way sync from ShootPath to other calendar apps.

### How iCal Feeds Work

**One-way sync:**
- ShootPath events appear in your external calendar (Apple Calendar, Outlook, etc.)
- Changes in ShootPath update the external calendar
- Changes in external calendar do NOT sync back to ShootPath

**Use cases:**
- You primarily use Apple Calendar on iPhone/Mac
- You use Outlook for work and want to see ShootPath sessions
- You want to share your availability without giving full edit access
- You don't need two-way sync (simpler, fewer conflicts)

**Limitations:**
- You can't edit ShootPath sessions from the external calendar
- Blocked time in external calendar doesn't prevent ShootPath bookings
- Need to manually check both calendars to avoid conflicts

### Setting Up iCal Feed

**Generate your iCal feed URL:**

**1. Go to Settings > Integrations**
- Navigate to **Settings** (gear icon)
- Click **Integrations**
- Find **Calendar Feed** or **iCal** section

**2. Configure feed settings**
- **What to include:**
  - ☑ Job sessions
  - ☑ Mini session events
  - ☑ Blocked time (optional)
- **Event visibility:** Choose how much detail to show
  - Full details (client names, locations, notes)
  - Basic (just "Session blocked" without client info)
  - Times only (just busy/free)

**3. Generate feed URL**
- Click **Generate iCal Feed**
- ShootPath creates a unique URL like:
  `https://app.shootpath.com/api/calendar/feed/abc123def456`
- **This URL is private** - anyone with it can view your calendar
- Copy the URL

**4. Add to your calendar app**

**For Apple Calendar (macOS/iOS):**
1. Open Calendar app
2. Go to **File > New Calendar Subscription** (Mac) or **Settings > Accounts > Add Account > Other** (iOS)
3. Paste your ShootPath iCal feed URL
4. Set refresh frequency: Every 15 minutes (more frequent = more up-to-date)
5. Name it "ShootPath" or "Work Calendar"
6. Click **Subscribe**

**For Microsoft Outlook:**
1. Open Outlook
2. Go to **Calendar view**
3. Click **Add Calendar > From Internet**
4. Paste your ShootPath iCal feed URL
5. Name it "ShootPath"
6. Set refresh frequency
7. Click **OK**

**For other calendar apps:**
Look for "Subscribe to calendar," "Add calendar by URL," or "iCal subscription." Most calendar apps support this standard.

**5. Verify sync**
- Check your external calendar
- Your ShootPath sessions should appear within 15-30 minutes (depending on refresh frequency)
- If nothing appears, verify the URL and try again

### Managing iCal Feed

**Update feed settings:**
If you change what's included in the feed (e.g., add blocked time):
1. Go to Settings > Integrations > Calendar Feed
2. Update settings
3. Click **Save**
4. The feed URL stays the same, but content updates automatically
5. External calendars see changes on next refresh

**Revoke and regenerate feed:**
If your feed URL is compromised (accidentally shared publicly):
1. Click **Revoke Feed**
2. The old URL stops working immediately
3. Click **Generate New Feed**
4. Update the URL in all your external calendars

**Refresh frequency:**
External calendars don't refresh instantly. Typical refresh times:
- Apple Calendar: Every 15 minutes - 1 hour (you choose)
- Google Calendar: Every few hours (Google's choice, can't adjust)
- Outlook: Every 30 minutes - few hours (you choose)

**For time-sensitive updates** (e.g., you just rescheduled a session), manually refresh:
- Apple Calendar: Right-click calendar name > **Refresh**
- Outlook: Click **Send/Receive > Update Folder**

### iCal Feed Best Practices

**Use for viewing, not editing:**
iCal feeds are read-only. Always make changes in ShootPath, not the external calendar.

**Choose the right detail level:**
- Full details: Use if only you see this calendar
- Basic: Use if family members see the calendar (they don't need client names)
- Times only: Use for availability sharing (busy/free without details)

**Set frequent refresh:**
The more frequently your external calendar refreshes, the more up-to-date it is. 15-30 minutes is a good balance.

**Keep URL private:**
Your iCal feed URL is like a password. Don't share it publicly or post it online. Anyone with the URL can see your calendar.

**Test before sharing:**
If you're sharing the feed with team members or family, test it first to ensure the right level of detail appears.

## Syncing with Apple Calendar

Apple Calendar (formerly iCal) is popular with iPhone and Mac users.

### Setup Methods

**Option 1: iCal feed (one-way sync)**
- Follow iCal feed setup above
- Simple, reliable, read-only

**Option 2: Via Google Calendar (two-way sync)**
- Set up Google Calendar sync in ShootPath
- Add your Google account to Apple Calendar
- ShootPath → Google → Apple (two-way)

**Which to choose:**
- **iCal feed:** Simpler, fewer moving parts, one-way is fine
- **Via Google:** Two-way sync, but requires Google as middleman

### Apple Calendar Subscription Steps

**On Mac:**
1. Open Calendar app
2. **File > New Calendar Subscription**
3. Paste ShootPath iCal feed URL
4. Click **Subscribe**
5. Configure:
   - Name: "ShootPath"
   - Color: Choose a distinct color
   - Location: "On My Mac" or "iCloud" (iCloud syncs to iPhone/iPad too)
   - Refresh: Every 15 minutes
   - Remove: Never
6. Click **OK**

**On iPhone/iPad:**
1. Go to **Settings > Calendar > Accounts**
2. Tap **Add Account**
3. Tap **Other**
4. Tap **Add Subscribed Calendar**
5. Paste ShootPath iCal feed URL
6. Tap **Next**
7. Configure settings
8. Tap **Save**

**Verify:**
Open Calendar app, and you should see a new calendar called "ShootPath" with your sessions.

### Viewing in Apple Calendar

**Calendar list:**
- Your ShootPath calendar appears in the calendar list (left sidebar on Mac, calendar button on iPhone)
- Toggle visibility on/off by checking/unchecking it

**Color coding:**
- Choose a distinct color for ShootPath events
- This helps differentiate work sessions from personal events

**Combined view:**
View all calendars together to see your complete schedule:
- Work sessions (ShootPath)
- Personal appointments (iCloud Calendar)
- Family events (Shared Family Calendar)

**Search:**
Apple Calendar's search includes ShootPath events. Search for a client name, and the session appears in results.

## Syncing with Outlook

Microsoft Outlook (desktop, web, and mobile) supports iCal feed subscriptions.

### Outlook Desktop Setup

**For Windows/Mac Outlook app:**

1. Open Outlook
2. Go to **Calendar** view (bottom navigation)
3. Right-click in calendar list
4. Select **Add Calendar > From Internet**
5. Paste ShootPath iCal feed URL
6. Click **OK**
7. Outlook asks: "Subscribe to this Calendar?"
8. Click **Yes**
9. Name it "ShootPath"
10. Choose where to store: "My Calendars"
11. Outlook begins downloading events (may take a few minutes)

**Configure update frequency:**
1. Right-click the ShootPath calendar
2. Select **Properties** or **Subscription Settings**
3. Set **Update Limit:** Every 15-30 minutes
4. Check **Update this subscription with the publisher's recommendation** (uses ShootPath's suggested refresh)

### Outlook Web (Outlook.com) Setup

**For Outlook on the web:**

1. Go to Outlook.com and sign in
2. Click **Calendar** icon
3. Click **Add Calendar**
4. Choose **Subscribe from web**
5. Paste ShootPath iCal feed URL
6. Name it "ShootPath"
7. Choose a color
8. Click **Import**

**Note:** Outlook.com refresh frequency is controlled by Microsoft (usually every few hours). You can't adjust it.

### Outlook Mobile Setup

Outlook mobile (iOS/Android) syncs calendars from your Outlook account. If you've added the ShootPath calendar to Outlook desktop or web, it automatically appears in mobile.

**If it doesn't appear:**
1. Open Outlook mobile app
2. Tap **Calendar**
3. Tap **hamburger menu (☰)**
4. Check that ShootPath calendar is visible/enabled

## Other Calendar Apps

Most calendar apps support iCal feeds. Here's how to add ShootPath to common ones.

### Fantastical (macOS/iOS)

1. Open Fantastical
2. Go to **Fantastical > Add Calendar > New Calendar Subscription**
3. Paste ShootPath iCal feed URL
4. Configure name, color, refresh frequency
5. Click **Subscribe**

### BusyCal (macOS)

1. Open BusyCal
2. Go to **File > New Calendar Subscription**
3. Paste ShootPath iCal feed URL
4. Configure settings
5. Click **Subscribe**

### Thunderbird (cross-platform)

1. Open Thunderbird
2. Right-click in calendar list
3. Select **New Calendar**
4. Choose **On the Network**
5. Select **iCalendar (ICS)**
6. Paste ShootPath iCal feed URL
7. Name it "ShootPath"
8. Choose offline support settings
9. Click **Next** and **Finish**

### Yahoo Calendar

1. Go to Yahoo Calendar
2. Click **Actions > Import Calendar**
3. Choose **Import by URL**
4. Paste ShootPath iCal feed URL
5. Name it "ShootPath"
6. Click **Import**

## Calendar Subscription for Sharing

Generate shareable calendar subscriptions for team members, family, or others who need to see your availability.

### Creating a Shareable Feed

**Different from your personal feed:**
- Your personal feed might include full client details
- A shareable feed should show less detail (privacy!)

**Steps:**
1. Go to **Settings > Integrations > Calendar Feed**
2. Click **Create Shareable Feed**
3. Configure what to share:
   - Event titles: Generic ("Session," "Blocked time") or detailed ("Smith Family Portrait")
   - Locations: Show or hide
   - Notes: Show or hide
   - Contact info: Never include
4. Set expiration (optional):
   - Active for 30 days
   - Active for 6 months
   - Never expires (for permanent team members)
5. Click **Generate Shareable Feed**
6. Copy the unique URL

**Share the URL:**
- Send to team members, assistants, or second shooters
- They add it to their calendar app (same process as iCal feed above)
- They see your availability without full details

### Managing Shareable Feeds

**View all active feeds:**
Settings > Integrations > Calendar Feed shows:
- Your personal feed
- All shareable feeds you've created
- Who has access (if you labeled them)
- Expiration dates

**Revoke a feed:**
If someone shouldn't have access anymore:
1. Click **Revoke** next to that shareable feed
2. The URL stops working immediately
3. Their calendar stops receiving updates

**Update a feed's settings:**
You can't change an existing feed's settings. Instead:
1. Revoke the old feed
2. Create a new one with updated settings
3. Share the new URL

### Use Cases for Shareable Feeds

**Team coordination:**
- Assistant sees when you're booked vs. available
- They can schedule accordingly
- But they don't see client names or private details

**Family/partner:**
- Your spouse sees when you have sessions
- They can plan family activities around your work
- Generic labels like "Portrait Session" give context without client info

**Second shooters:**
- They see when you need coverage
- They know which dates you're already booked
- Can coordinate their availability

**Venue coordinators:**
- Share with preferred venues so they know your busy dates
- Helps them recommend you when you're actually available
- No client info shared, just busy/free

## Calendar Privacy and Security

Your calendar contains sensitive scheduling information. Protect it.

### What's in Your Calendar Data

**Public info (safe to share broadly):**
- Date and time of sessions
- General type (portrait, wedding)
- Location (city or general area)

**Private info (sensitive):**
- Client full names
- Specific addresses
- Phone numbers or contact info
- Session notes (client preferences, health info, etc.)
- Pricing or financial details

**Internal info (never share):**
- Internal notes about clients
- Workflow task details
- Payment status
- Client communication history

### Feed Privacy Levels

**ShootPath supports multiple privacy levels:**

**Level 1: Full details (Personal use only)**
- Client names
- Full locations and addresses
- Notes and details
- Use for: Your own devices only

**Level 2: Basic details (Team/family sharing)**
- Generic event titles ("Portrait Session")
- General locations ("Washington Park")
- Duration and times
- No client names or sensitive info
- Use for: Assistants, family, team members

**Level 3: Times only (Public sharing)**
- Just shows busy/free
- No details at all
- Use for: Public availability sharing, booking widgets

**Choose the right level** when generating iCal feeds or shareable subscriptions.

### Securing Your Calendar Feed

**Protect your feed URL:**
- Treat it like a password
- Don't post publicly on social media
- Don't include in emails that might be forwarded
- Use shareable feeds (with limited detail) for team, not your personal feed

**If feed URL is compromised:**
1. Immediately revoke the feed
2. Generate a new one
3. Update all your devices/apps with new URL
4. Anyone with old URL loses access

**Use expiring feeds for temporary access:**
If you're working with a temporary assistant or contractor, create a shareable feed with 30-day expiration. It automatically stops working after 30 days.

## Troubleshooting Common Issues

### Events Not Showing Up

**Checklist:**
1. Is the feed URL correct? (Copy/paste again to be sure)
2. Has the external calendar refreshed? (Check refresh frequency, or manually refresh)
3. Is the date range within the sync window? (Some feeds only sync upcoming events)
4. Did ShootPath actually create the events? (Check in ShootPath to confirm)

**Fix:**
- Wait 15-30 minutes for refresh
- Manually refresh external calendar
- Remove and re-add the feed
- Check ShootPath integration settings

### Events Not Updating

**Problem:**
You change a session time in ShootPath, but the external calendar still shows the old time.

**Cause:**
External calendar hasn't refreshed yet.

**Fix:**
- Manually refresh the external calendar
- Wait for next automatic refresh
- Check refresh frequency settings (set to 15-30 min if possible)

### Duplicate Events

**Problem:**
Same session appears twice in external calendar.

**Cause:**
- Feed was added twice (check calendar subscriptions list)
- Event was manually created in external calendar AND synced from feed
- Two different ShootPath feeds are syncing

**Fix:**
- Remove duplicate feeds (check calendar subscription list)
- Delete manually created duplicates
- Ensure only one ShootPath feed is active

### Wrong Time Zone

**Problem:**
Events show at wrong times (e.g., 2pm session shows as 5pm).

**Cause:**
Time zone mismatch between ShootPath, external calendar, or device.

**Fix:**
1. Check ShootPath time zone: Settings > Calendar > Time Zone
2. Check external calendar time zone settings
3. Check device time zone (especially if traveling)
4. Ensure all three match

### Google Sync Stopped Working

**Problem:**
Google Calendar sync was working, now it's not.

**Causes:**
- Google authorization expired (happens every few months)
- You changed your Google password
- Network connectivity issue
- Google Calendar API issue

**Fix:**
1. Go to Settings > Integrations > Google Calendar
2. Check sync status
3. If "Not connected" or "Authorization expired," click **Reconnect**
4. Re-authorize with Google
5. Sync resumes

## Best Practices Summary

**Choose the right sync method:**
- Two-way sync (Google): Best for most photographers, especially if you use Google on phone
- One-way sync (iCal feed): Simpler, fewer conflicts, good for Apple/Outlook users

**Keep it simple:**
Don't sync ShootPath with five different calendars. Choose one or two primary calendars and stick with them.

**Use ShootPath as primary:**
Always create client sessions in ShootPath (not external calendar). This ensures all job details, workflows, and data are connected properly.

**Review sync status weekly:**
Quick check every Monday: "Is my calendar sync still working?" Catch issues before they become problems.

**Protect your feed URLs:**
Treat them like passwords. Don't share publicly. Revoke if compromised.

**Set appropriate detail levels:**
- Full details: Your devices only
- Basic details: Team/family
- Times only: Public sharing

**Manually refresh before important scheduling:**
Before confirming availability with a client, manually refresh your external calendar to ensure it's current.

**Have a backup plan:**
If sync breaks, don't panic. You can always view your schedule directly in ShootPath. Fix sync when you have time.

**Test after setup:**
After setting up any integration, create a test session in ShootPath and verify it appears in your external calendar.

---

## What's Next?

Master your calendar system with these related articles:

**[Calendar Overview](./index)** - Understand calendar view modes, color coding, and navigation

**[Scheduling Sessions](./scheduling-sessions)** - Learn how to add sessions, block time, and manage availability

**[Client Booking](./client-booking)** - Enable clients to self-schedule mini sessions

**Related topics:**

**[Jobs Overview](../jobs/)** - Understand how jobs and calendar sessions work together

**[Workflows](../workflows/)** - Automate reminders and tasks based on calendar dates

---

**Questions?** Look for the help links throughout ShootPath, or use the support widget if you need assistance!
