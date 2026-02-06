---
sidebar_position: 4
---

# Google Calendar Integration

## Quick Reference

Google Calendar integration syncs your photography schedule between ShootPath and Google Calendar. When you book a wedding in ShootPath, it appears in your calendar automatically. When you block time in Google Calendar, ShootPath knows not to double-book.

**What Syncs:**
- Job session dates (weddings, portraits, events)
- Mini session event dates
- Blocked time (personal appointments, vacations)
- Job details (client name, type, location)

**Sync Direction:**
- **ShootPath → Calendar:** New bookings appear automatically
- **Calendar → ShootPath:** Block time to prevent double-booking

**Why Use It:**
- One source of truth for your schedule
- Never double-book a date
- See your photography schedule alongside personal events
- Share your availability with family or assistants
- Works with mobile calendar apps

**Setup Time:**
3-5 minutes to connect and configure

**Cost:**
Free with any Google account

**Quick Setup:**
Go to **Settings > Integrations > Google Calendar**, click "Connect", authorize ShootPath, choose which calendar to sync to.

**Next Steps:**
- [Connect your calendar](#connecting-google-calendar)
- [Configure sync settings](#configuring-sync-settings)
- [Understand what syncs](#what-gets-synced)
- [Troubleshoot sync issues](#troubleshooting-sync-issues)

---

## Detailed Guide

### What is Google Calendar Integration?

Google Calendar integration creates a two-way connection between ShootPath's internal calendar and your Google Calendar. Think of it as keeping two calendars in sync automatically.

**Without integration:**
- You book a wedding in ShootPath
- You manually add event to Google Calendar
- Client reschedules
- You update ShootPath
- You update Google Calendar
- You accidentally double-book because calendars don't match
- Repeat for every booking... error-prone!

**With integration:**
- You book a wedding in ShootPath
- **Automatic:** Event appears in Google Calendar
- Client reschedules in ShootPath
- **Automatic:** Google Calendar updates
- You block vacation in Google Calendar
- **Automatic:** ShootPath shows date unavailable
- You never worry about calendars being out of sync!

### Why Sync with Google Calendar?

#### Unified Schedule

See your photography sessions alongside:
- Personal appointments (dentist, car maintenance)
- Family events (kid's soccer games)
- Vacations
- Other commitments

**All in one place!**

#### Mobile Access

Google Calendar works everywhere:
- iPhone Calendar app
- Android Calendar app
- Google Calendar mobile app
- Desktop notifications
- Calendar widgets

**Your schedule is always in your pocket.**

#### Prevent Double-Booking

The integration prevents scheduling conflicts:

**Scenario:**
- You have a personal event Saturday at 2 PM (in Google Calendar)
- Client requests portrait session Saturday
- ShootPath shows Saturday as unavailable
- You avoid the conflict automatically

#### Share Your Availability

**With your spouse:**
"Can we do date night Friday?"
They check shared calendar - "Nope, you have a wedding!"

**With assistants:**
Second shooters see which dates you're booked without accessing ShootPath

**With clients (optional):**
Share read-only view of your availability calendar

#### Automatic Reminders

Google Calendar sends notifications:
- "Wedding tomorrow at 10 AM"
- "Portrait session in 1 hour"
- Customize reminder timing

Never miss a session!

### Connecting Google Calendar

#### Step 1: Navigate to Integration Settings

Go to **Settings > Integrations > Google Calendar**

#### Step 2: Click "Connect Google Calendar"

You'll be redirected to Google's authorization page

#### Step 3: Choose Google Account

Select which Google account contains the calendar you want to sync.

**If you have multiple accounts:**
- Choose the account with your business calendar
- Personal Google account is fine if that's where you keep your schedule
- Don't worry - you can choose which specific calendar within that account later

#### Step 4: Grant Permissions

Google asks: "ShootPath wants to access your Google Account"

**Permissions requested:**
- View and edit events on all your calendars
- Create, edit, and delete events

**Why these permissions?**
- **View:** ShootPath needs to see blocked time
- **Edit:** Update events when sessions reschedule
- **Create:** Add new bookings automatically
- **Delete:** Remove events if job is cancelled

**Important:** ShootPath only creates/edits photography events. It won't touch your personal events!

Click "Allow"

#### Step 5: Choose Which Calendar to Sync

Back in ShootPath, you'll see a dropdown:

**Select calendar:**
```
[ Choose Calendar ▼ ]
  - Primary
  - Work
  - Photography Business
  - Personal
```

**Which calendar should you choose?**

**Option 1: Create a new "Photography" calendar (recommended)**
1. Open Google Calendar
2. Click "+" next to "Other calendars"
3. Select "Create new calendar"
4. Name it "Photography Business"
5. Choose color (easy to spot in weekly view)
6. Return to ShootPath, refresh, select this calendar

**Why separate calendar?**
- Easy to distinguish photography vs. personal events
- Can share with others without revealing personal schedule
- Can hide/show photography events independently

**Option 2: Use your primary calendar**
- Simpler if you keep everything in one calendar
- Photography sessions mixed with personal events
- Still works great!

#### Step 6: Configure Sync Settings

Choose what to sync:

**Sync job session dates:**
☑ **Enabled** (recommended)
- Weddings, portraits, events with session dates
- Creates all-day or timed events

**Sync mini session events:**
☑ **Enabled** (recommended)
- Mini session dates appear on calendar
- Shows available time slots

**Sync blocked time FROM Google Calendar:**
☑ **Enabled** (recommended)
- Events in Google Calendar block time in ShootPath
- Prevents double-booking

**Event visibility:**
- **Default** - Uses calendar's default visibility
- **Public** - Anyone with calendar link can see
- **Private** - Only you can see event details

**Event reminders:**
- **Use calendar defaults** (recommended)
- **Custom:** Set ShootPath-specific reminder times

#### Step 7: Test the Sync

**Create a test job in ShootPath:**
1. Create test lead and job
2. Set session date to tomorrow
3. Save job

**Check Google Calendar:**
- Open Google Calendar
- Look at tomorrow's date
- Do you see the test event?
- Does it have correct time and details?

**Test blocking time:**
1. Create event in Google Calendar for next week
2. Go to ShootPath calendar
3. Is that date/time marked unavailable?

**If both work:** Connection successful! ✓

**If either fails:** See [troubleshooting section](#troubleshooting-sync-issues)

### What Gets Synced

#### Jobs with Session Dates

**When you create/update a job in ShootPath:**

**What syncs to Google Calendar:**
- **Event title:** "[Client Name] - [Job Type]"
  - Example: "Sarah Johnson - Wedding"
- **Date and time:** Session date and time
- **Location:** Session location (if entered in ShootPath)
- **Description:** Job details, client contact info
- **Event link:** Back to ShootPath job page

**Example calendar event:**
```
Sarah Johnson - Wedding
Saturday, June 14, 2026
10:00 AM - 6:00 PM

Location: Riverside Gardens, 123 Main St

Description:
Client: Sarah Johnson
Phone: (555) 123-4567
Email: sarah@example.com
Package: Premium Wedding Package

View in ShootPath: [link]
```

#### Mini Session Events

**When you create a mini session event in ShootPath:**

**What syncs to Google Calendar:**
- **Event title:** "Mini Sessions - [Location]"
  - Example: "Mini Sessions - Central Park"
- **Date and time:** Event start and end time
- **Available slots:** Shown in event description
- **Bookings:** Updates as clients book slots

**Example calendar event:**
```
Mini Sessions - Central Park
Saturday, April 20, 2026
9:00 AM - 3:00 PM

Available Slots: 12
Booked: 8
Remaining: 4

View bookings: [link]
```

#### Blocked Time (From Google Calendar to ShootPath)

**When you create an event in Google Calendar:**

ShootPath marks that time as unavailable. You can't schedule sessions during blocked time.

**What blocks time:**
- Any event in the synced calendar
- All-day events (vacation, day off)
- Timed events (dentist appointment 2-3 PM)
- Recurring events (every Thursday 1-2 PM)

**Event details don't sync to ShootPath** - just the fact that time is blocked. ShootPath doesn't need to know you have a dentist appointment, just that you're not available!

#### What Does NOT Sync

**From ShootPath to Google Calendar:**
- Leads (they don't have confirmed dates)
- Jobs without session dates
- Tasks or to-dos
- Client contact info (except in event description)
- Payment status
- Internal notes

**From Google Calendar to ShootPath:**
- Event titles (ShootPath just knows time is blocked)
- Event details
- Personal information
- Attendees or guests

### Configuring Sync Settings

Fine-tune how the integration works:

#### Sync Frequency

**How often does ShootPath check for updates?**

**Real-time (within 5 minutes):**
- You update job in ShootPath → Calendar updates in 2-3 minutes
- You block time in Calendar → ShootPath updates in 3-5 minutes

**Why not instant?**
- API rate limits (Google restricts how often apps can check)
- Battery/performance optimization

**In practice:** Feels instant for most use cases!

#### Event Duration Defaults

**If job doesn't have specific start/end time:**

ShootPath creates all-day event:
```
Sarah Johnson - Wedding
All day event on June 14
```

**If job has specific time:**

ShootPath creates timed event:
```
Sarah Johnson - Wedding
June 14, 10:00 AM - 6:00 PM
```

**Tip:** Set session times in ShootPath for more accurate calendar!

#### Calendar Color Coding

**In Google Calendar settings (not ShootPath):**

Assign colors to event types:
- Wedding events: Red
- Portrait sessions: Blue
- Mini sessions: Green
- Personal events: Purple

**How to set this up:**
1. Open Google Calendar
2. Click gear icon > Settings
3. Click your photography calendar
4. Choose default color
5. OR color-code individual events manually

#### Notification Settings

**Default:** Uses your Google Calendar's default notification settings

**To customize photography event notifications:**
1. Open Google Calendar
2. Create/edit photography event
3. Click "Add notification"
4. Choose timing: 1 day before, 1 hour before, etc.
5. Choose method: Notification, Email, SMS

**Recommended notification setup:**
- 1 week before: Email reminder
- 1 day before: Notification
- 1 hour before: Notification

### Managing Multiple Calendars

#### Using Sub-Calendars

**Scenario:** You shoot weddings AND teach photography workshops

**Setup:**
1. Create "Wedding Photography" calendar in Google
2. Create "Workshops & Teaching" calendar in Google
3. Connect ShootPath to "Wedding Photography" calendar
4. Manually add workshop events to "Workshops" calendar

**Result:**
- ShootPath sessions appear in "Wedding Photography"
- Workshops appear in "Workshops & Teaching"
- Both show in your main calendar view
- Easy to toggle visibility of each

#### Sharing Calendars

**Share your availability with others:**

**Read-only access:**
Perfect for spouse, parents, friends
- They see when you're busy
- They can't edit your schedule

**Edit access:**
Perfect for second shooters, assistants
- They can add/edit events
- They can check availability

**How to share:**
1. Open Google Calendar
2. Find your photography calendar
3. Click three dots > "Settings and sharing"
4. Under "Share with specific people," add email
5. Choose permission level
6. They receive invitation

**What they see:**
If you shared photography calendar, they see:
- All photography events
- Not your personal events (unless you shared that calendar too)

#### Color-Coding by Job Type

**Make your calendar easier to scan:**

**Option 1: Use event titles**
- "🎩 Sarah - Wedding"
- "📸 Johnson Family - Portrait"
- "🎉 Corporate Event - ABC Company"

Emoji make event types jump out!

**Option 2: Use calendar colors**
Google Calendar lets you color individual events:
1. Click event
2. Choose color from palette
3. Color-code by type (red = weddings, blue = portraits)

### Two-Way Sync Scenarios

#### Scenario 1: New Booking

**Action in ShootPath:**
Create job with session date June 14 at 10 AM

**What happens:**
1. ShootPath saves job
2. Within 3 minutes, event appears in Google Calendar
3. Event shows "Sarah Johnson - Wedding" on June 14 at 10 AM

**On your phone:**
- Google Calendar app shows notification
- iPhone/Android calendar shows event
- Calendar widget updates

#### Scenario 2: Rescheduling

**Action in ShootPath:**
Client reschedules from June 14 → June 21

**What happens:**
1. You update session date in ShootPath
2. Within 3 minutes, Google Calendar event moves to June 21
3. Old date now available
4. New date marked busy

**Calendar stays accurate automatically!**

#### Scenario 3: Cancellation

**Action in ShootPath:**
Client cancels, you delete job

**What happens:**
1. ShootPath deletes job
2. Within 3 minutes, Google Calendar event removed
3. Date becomes available again

#### Scenario 4: Blocking Personal Time

**Action in Google Calendar:**
Add vacation June 1-7 (all day events)

**What happens:**
1. Google Calendar saves events
2. Within 5 minutes, ShootPath marks June 1-7 unavailable
3. You try to book session June 3 in ShootPath
4. Calendar shows "Not available - time blocked"
5. Prevents double-booking

#### Scenario 5: Editing in Google Calendar

**What if you edit event in Google Calendar directly?**

**Example:** Change event from 10 AM to 11 AM in Google Calendar

**What happens:**
- Event time changes in Google Calendar ✓
- ShootPath DOES NOT update
- Session time in ShootPath still shows 10 AM
- Calendars now out of sync!

**Best practice:** Always edit session times in ShootPath, let it sync to Calendar

**Exception:** Blocking time - do this in Google Calendar, it syncs to ShootPath correctly

### Calendar Sync Best Practices

#### 1. Edit Sessions in ShootPath (Not Calendar)

**Do:**
- Change session time in ShootPath → syncs to Calendar

**Don't:**
- Change session time in Calendar → ShootPath doesn't know

**Why:** ShootPath is the source of truth for photography bookings

#### 2. Block Personal Time in Google Calendar

**Do:**
- Add vacation to Google Calendar → syncs to ShootPath
- Add appointments to Google Calendar → blocks time in ShootPath

**Don't:**
- Try to block time in ShootPath that isn't a photography session

**Why:** Google Calendar is the source of truth for personal time

#### 3. Use Descriptive Event Titles

**In ShootPath, use clear job names:**
✅ "Sarah & Mike Wedding"
✅ "Johnson Family Portrait"
✅ "ABC Corp Headshots"

❌ "Wedding"
❌ "Session"
❌ "Client 1"

**These titles appear in your calendar!** Make them informative.

#### 4. Set Session Times When Possible

**Instead of:**
- "Wedding on June 14" (all day event)

**Set:**
- "Wedding on June 14, 10 AM - 6 PM"

**Benefit:** More accurate calendar, better at preventing scheduling conflicts

#### 5. Color-Code Your Calendar

Assign colors to different event types in Google Calendar. Quickly see at a glance:
- Red = Weddings (all day)
- Blue = Portrait sessions (2 hours)
- Green = Mini sessions
- Purple = Personal events

#### 6. Keep One Primary Photography Calendar

Don't sync to multiple calendars. Choose one and stick with it:
- Easier to manage
- Less chance of confusion
- Simpler sharing with others

### Disconnecting Calendar Sync

**If you want to stop syncing:**

#### Step 1: Go to Integration Settings

Settings > Integrations > Google Calendar

#### Step 2: Click "Disconnect"

ShootPath stops syncing immediately

#### Step 3: Choose What Happens to Existing Events

**Option 1: Keep events in Google Calendar**
- Past photography events remain
- You can manually delete them if desired

**Option 2: Remove all synced events**
- ShootPath removes all events it created
- Your calendar returns to pre-sync state

**Recommended:** Keep events. They're historical record of your bookings.

#### What Happens After Disconnecting

**Future bookings:**
- New ShootPath sessions won't appear in Calendar
- You're back to manually adding events

**Existing bookings:**
- Events already in Calendar remain (unless you chose to remove them)
- Editing session in ShootPath won't update Calendar
- Calendars will drift out of sync over time

**Blocked time:**
- Blocking time in Google Calendar won't affect ShootPath
- You could accidentally double-book

### Troubleshooting Sync Issues

#### Issue 1: Events Not Appearing in Google Calendar

**Symptoms:**
Book session in ShootPath, but event doesn't show in Calendar

**Possible causes and fixes:**

**1. Sync delay**
- Wait 5-10 minutes
- Refresh Google Calendar (F5 or pull-to-refresh on mobile)
- Still not showing? Continue troubleshooting...

**2. Wrong calendar selected**
- Check which calendar ShootPath is syncing to
- Settings > Integrations > Google Calendar > "Syncing to: [calendar name]"
- Open Google Calendar and view that specific calendar
- Is the calendar hidden? (Check left sidebar, calendar should be checked)

**3. Connection expired**
- Go to Settings > Integrations > Google Calendar
- Shows "Disconnected" or error message?
- Click "Reconnect" and re-authorize

**4. Session date not set**
- Check the job in ShootPath
- Does it have a session date?
- Only jobs with session dates sync to Calendar

#### Issue 2: Events Syncing to Wrong Calendar

**Symptoms:**
Events appear in "Personal" calendar instead of "Photography" calendar

**Fix:**
1. Go to Settings > Integrations > Google Calendar
2. Check "Syncing to:" dropdown
3. Select correct calendar
4. Click "Update Settings"
5. Events will sync to new calendar going forward
6. Manually move old events in Google Calendar

**To move events in Google Calendar:**
1. Click event
2. Click "More actions" (three dots)
3. Select "Move to" > Choose correct calendar

#### Issue 3: Blocked Time Not Preventing Bookings

**Symptoms:**
You block time in Google Calendar, but ShootPath still shows date available

**Possible causes and fixes:**

**1. Wrong calendar**
- ShootPath only checks the calendar you've connected
- Did you block time in different calendar?
- Move event to connected calendar

**2. Sync delay**
- Wait 5-10 minutes for sync
- Refresh ShootPath calendar page

**3. "Sync blocked time" setting disabled**
- Go to Settings > Integrations > Google Calendar
- Check "Sync blocked time FROM Google Calendar" is enabled
- If not, enable it and save

#### Issue 4: Duplicate Events

**Symptoms:**
Same session appears twice in Google Calendar

**Why this happens:**
- You manually added event to Calendar
- Then ShootPath synced and created another

**Fix:**
1. Delete the manually-created event (keep ShootPath-created one)
2. Stop manually adding events - let sync do it!

**How to tell which is which:**
- ShootPath events have link to job in description
- ShootPath events say "Created by ShootPath" in details

#### Issue 5: Events Not Updating When Rescheduled

**Symptoms:**
Change session date in ShootPath, but Calendar still shows old date

**Possible causes:**

**1. Sync delay**
- Wait 5-10 minutes
- Refresh Google Calendar

**2. Edited event in Calendar directly**
- ShootPath can't update events you've manually edited
- Delete event from Calendar
- Let ShootPath recreate it with correct info

**3. Connection expired**
- Reconnect Google Calendar integration
- ShootPath will re-sync all events

#### Issue 6: Calendar Permissions Error

**Symptoms:**
Error: "ShootPath does not have permission to access this calendar"

**Fix:**
1. Go to Google Account settings
2. Security > Third-party apps with account access
3. Find ShootPath
4. Click "Remove access"
5. Go back to ShootPath
6. Reconnect Google Calendar integration
7. Grant all requested permissions

### Understanding Sync Limits

#### API Rate Limits

Google limits how often ShootPath can check for updates:

**Standard limits:**
- 10,000 requests per day (per user)
- Effectively unlimited for photography business use

**What uses API quota:**
- Each calendar check
- Each event create/update/delete
- Checking for blocked time

**You'll never hit these limits** unless you're booking 100+ sessions per day!

#### Event Count Limits

**Google Calendar limits:**
- 25,000 events per calendar
- If you've been in business 20 years with weekly bookings: ~1,000 events
- You're safe!

### Calendar Sync for Teams

**If you have assistants or second shooters:**

#### Sharing Your Photography Calendar (Read-Only)

**Perfect for:**
- Second shooters checking your schedule
- Virtual assistants managing inquiries
- Family knowing when you're shooting

**How to share:**
1. Open Google Calendar
2. Find photography calendar
3. Settings > "Share with specific people"
4. Add their email
5. Choose "See all event details"
6. They can view but not edit

#### Sharing with Edit Access

**Perfect for:**
- Studio manager who books sessions
- Partner who manages schedule
- Assistant who handles mini sessions

**How to share:**
1. Same steps as above
2. Choose "Make changes to events" permission
3. They can add/edit events in Google Calendar
4. **Important:** They still can't access ShootPath
5. But their calendar changes sync to ShootPath!

**Example:**
- Assistant blocks vacation in Calendar
- ShootPath marks dates unavailable
- You can't accidentally book sessions those days

### Alternative: Using ShootPath Calendar Only

**Don't use Google Calendar? That's fine!**

ShootPath has a full-featured built-in calendar:

**You get:**
- Month, week, day views
- Session scheduling
- Blocked time
- Session details
- Color-coding by job type

**You don't get:**
- Mobile app sync
- Integration with personal events
- Sharing with non-ShootPath users
- Third-party calendar app support

**Many photographers use ShootPath calendar only and love it!**

### What's Next?

Now that your calendar is synced, your schedule is always up to date!

**Learn the ShootPath calendar** → [Calendar Guide](../calendar/) for all calendar features

**Set up workflows** → [Workflows](../workflows/) to automate booking confirmations

**Create your first booking** → [Understanding Jobs](../jobs/) walks through the booking process

**Connect other integrations** → [Integrations Overview](./index) to complete your setup

---

**Questions?** Look for the help links throughout ShootPath, or reach out to support if you need assistance!
