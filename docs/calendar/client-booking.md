---
sidebar_position: 4
---

# Client Booking

Learn how to enable client self-scheduling, share your availability, and manage booking preferences so clients can book mini sessions and see when you're available.

## Quick Reference

**Client Booking Features:**
- **Self-scheduling mini sessions** - Clients book time slots directly from your event page
- **Availability sharing** - Show clients when you're free without manual back-and-forth
- **Booking restrictions** - Control minimum notice, buffer time, and blackout dates
- **Automatic confirmations** - Clients receive instant booking confirmation

**What Clients Can Book:**
- Mini session time slots
- Consultation meetings (if enabled)
- Follow-up appointments (if enabled)

**What Clients Can't Book:**
- Full job sessions (these require quote acceptance and contract signing)
- Custom dates (only pre-defined slots or availability windows)
- Times outside your business hours

**Benefits:**
- Reduced back-and-forth ("Are you free Saturday at 2pm?")
- 24/7 booking availability
- Faster bookings = higher conversion
- Professional client experience
- Automatic conflict prevention

---

## Understanding Client Booking

### What is Client Self-Scheduling?

Client self-scheduling allows clients to book appointments directly from a public booking page or mini session event, without emailing or calling you for availability.

**How it works:**
1. You create a mini session event (e.g., "Fall Family Portraits")
2. Event has multiple time slots (e.g., 10am, 11am, 12pm, 1pm)
3. You share the event's public URL
4. Clients visit the URL, see available slots, and book
5. Slot is instantly marked as booked
6. Client receives confirmation email
7. Session appears on your calendar

**Traditional booking (manual):**
- Client: "Are you available Saturday at 2pm?"
- You check calendar: "Actually I'm booked then. How about 3pm?"
- Client: "I have soccer at 3pm. What about Sunday?"
- You: "Sunday works! 2pm?"
- Client: "Perfect!"
- Back-and-forth takes 2-3 days

**Self-scheduling (automated):**
- Client visits your Fall Mini Sessions page
- Sees available slots: Saturday 10am, 11am, 12pm, 1pm, 2pm
- Clicks "Book 2pm"
- Done in 30 seconds

**The difference:**
- Manual: 2-3 days, 5-10 messages
- Self-scheduling: 30 seconds, zero messages

### Why Client Booking Matters

**Eliminates scheduling friction:**
The easier it is to book, the more people book. Every extra step (call, email, wait for response) loses some clients.

**24/7 availability:**
Clients can book at 11pm on Sunday when they're thinking about it. You wake up Monday to new bookings, no work required.

**Professionalism:**
Self-scheduling signals "I'm organized and professional." It's a modern, polished client experience.

**Time savings:**
You're not spending hours coordinating schedules. Your time goes to creative work instead.

**Higher conversion:**
The moment a client decides "yes, I want this" and can book immediately, you've captured that decision. If they have to wait for you to respond, they might change their mind or forget.

**Prevents double-booking:**
When client books a slot, it's immediately marked as unavailable. No risk of accidentally booking two people at the same time.

### When to Use Client Booking

**Perfect for:**
- **Mini sessions** - Short, standardized sessions with fixed pricing
- **Meet-and-greet consultations** - 30-min intro calls with potential clients
- **Gallery viewing appointments** - In-person or virtual album design sessions
- **Follow-up shoots** - Quick add-on sessions for existing clients

**Not ideal for:**
- **Custom full-day shoots** - Weddings, large events (too many variables to standardize)
- **Custom pricing jobs** - When each job is quoted individually
- **Complex scheduling** - Jobs that require consultation before booking
- **First contact** - Initial inquiry should still be personal (quote sent after)

**The rule:**
If it's standardized (fixed time, fixed price, fixed scope), enable self-scheduling. If it's custom, keep it manual with personal consultation first.

## Mini Session Self-Booking

Mini sessions are the primary use case for client self-scheduling.

### Setting Up Mini Session Events

**Create a bookable mini session event:**

1. Go to **Mini Sessions > Create Event**
2. Fill in event details:
   - **Name:** "Fall Family Portraits" or "Holiday Mini Sessions"
   - **Date:** October 20, 2024
   - **Location:** Washington Park, Denver
   - **Description:** What's included, what to expect

3. Set up time slots:
   - **Start time:** 9:00 AM
   - **End time:** 3:00 PM
   - **Slot duration:** 30 minutes per family
   - **Buffer between slots:** 0 minutes (or 5 min if you want a break)
   - **Slots generated:** 12 slots (9am, 9:30am, 10am... 2:30pm)

4. Set pricing:
   - **Price per slot:** $200
   - **Payment required:** Deposit ($50) or full payment at booking

5. Configure booking settings:
   - **Public booking:** Enabled
   - **Minimum advance notice:** 48 hours (can't book within 2 days of event)
   - **Maximum slots per client:** 1 (prevents one person booking all slots)
   - **Booking deadline:** 24 hours before event start

6. Save and publish:
   - Event status: **Published**
   - Public URL generated: `shootpath.com/mini-sessions/fall-family-portraits-abc123`

**What happens:**
- Event appears on your public mini sessions page
- Clients can browse available slots
- Booked slots show as unavailable
- Event fills up as clients book

[Learn more about creating mini session events →](../mini-sessions/creating-events)

### Mini Session Booking Flow (Client Side)

**From the client's perspective:**

**1. Discover the event**
- Client finds your mini session through:
  - Your website
  - Social media post
  - Email newsletter
  - Word of mouth

**2. Visit the event page**
- Clicks link: `shootpath.com/mini-sessions/fall-family-portraits-abc123`
- Sees event details:
  - Photos/preview images
  - Location and date
  - What's included ("30-minute session, 20+ edited digital images")
  - Pricing
  - Testimonials (optional)

**3. View available slots**
- Calendar or list view shows all time slots
- Available slots: Green or clickable
- Booked slots: Grayed out or hidden
- Client picks their preferred time

**4. Book the slot**
- Clicks "Book 10:30 AM"
- Popup or new page opens

**5. Enter details**
- Client name
- Email
- Phone number
- Special requests (optional): "We have a toddler and a dog"
- Agree to terms/cancellation policy

**6. Payment**
- If deposit required: Pay $50 (Stripe checkout)
- If full payment required: Pay $200
- Secure payment processing

**7. Confirmation**
- Instant confirmation screen: "You're booked for Oct 20 at 10:30 AM!"
- Confirmation email sent immediately
- Calendar invite attached (optional)
- Slot marked as booked (no one else can book it)

**8. Reminders**
- Automatic reminder 1 week before: "Your mini session is coming up!"
- Automatic reminder 1 day before: "See you tomorrow at 10:30 AM!"

**Total time: 2-3 minutes.** Compare to days of email back-and-forth!

### Managing Bookings

**View all bookings:**
Go to **Mini Sessions > [Event Name] > Bookings** to see:
- List of all booked slots
- Client names and contact info
- Payment status (paid, deposit paid, unpaid)
- Special requests or notes

**Update a booking:**
Click any booking to:
- Edit client details
- Change time slot (if available)
- Add notes
- Process refund
- Cancel booking

**Manually add bookings:**
If a client calls or emails instead of using self-booking:
1. Go to event bookings
2. Click **Add Booking**
3. Choose available slot
4. Enter client details
5. Mark payment status
6. Save

The slot is now marked as booked, preventing double-booking.

**Cancel a booking:**
If a client cancels:
1. Open the booking
2. Click **Cancel Booking**
3. Choose:
   - Refund deposit/payment (Stripe refund processed)
   - Keep deposit (per your cancellation policy)
4. Slot becomes available again

**Waitlist (optional):**
If all slots are full, enable waitlist:
- Clients can join waitlist
- If someone cancels, waitlist clients get notified
- First to respond gets the slot

## Sharing Your Availability

Beyond mini sessions, you can share your general availability with clients for custom bookings.

### Availability Windows

**What are availability windows?**
Time ranges when you're available for custom sessions (not fixed mini session slots).

**Example:**
You tell a lead: "I'm available these dates for your family portrait session:"
- Saturday, Oct 14: 10am-2pm
- Sunday, Oct 15: 9am-12pm
- Saturday, Oct 21: All day

Instead of emailing this, you can share an availability page that shows these windows visually.

**How to create:**
1. Go to **Calendar > Share Availability**
2. Select date range: Oct 14-31
3. System shows all non-booked times
4. Customize:
   - Hide blocked personal time (keep "editing blocks" visible as busy)
   - Show only weekend availability
   - Show only times between 9am-5pm
5. Generate shareable link
6. Send to client

**Client views:**
- Calendar showing your available dates/times
- Booked times grayed out
- Available times in green
- Client can request a specific time
- Request goes to you for approval

**Important:** This is NOT self-booking. Client requests a time, you approve. This prevents clients from booking without quote/contract process.

### Booking Request Flow

**For custom jobs (portraits, weddings) that require quote first:**

**1. Lead requests more info**
- Lead: "I'm interested in family portraits. When are you available?"

**2. You send availability link**
- You: "Here's my availability for the next month: [link]"

**3. Client views and requests time**
- Client clicks link
- Sees your calendar (busy/free)
- Clicks a free time: "Saturday Oct 14 at 10am"
- Fills out request form:
  - Name
  - Email
  - Session type
  - Brief message
- Submits request

**4. You receive notification**
- Email: "New booking request from Sarah Johnson"
- Details: Oct 14 at 10am, Family portrait

**5. You respond**
- Review request
- If available, send quote: "Great! I've sent you a quote for Oct 14."
- If not available anymore, suggest alternative: "That slot was just booked, but I have Oct 15 at 2pm available."

**6. Quote accepted**
- Client accepts quote
- Job created
- Session scheduled for Oct 14 at 10am
- Shows on your calendar

**Why this extra step?**
Custom jobs need quotes, contracts, and payment setup. You can't fully book them without those elements. The availability page just streamlines the "when are you free?" conversation.

### Availability Preferences

**Configure default availability:**
Go to **Settings > Calendar > Availability** to set:

**Business hours:**
- Monday-Friday: 9am-5pm
- Saturday-Sunday: 10am-4pm
- Or customize per day

**Available days:**
- Weekends only
- Weekdays only
- Custom selection

**Booking window:**
- Clients can book 2 weeks to 6 months in advance
- Prevents last-minute bookings (you need prep time)
- Prevents too-far-future bookings (your schedule isn't set yet)

**Buffer time:**
- Minimum 30 minutes between sessions
- Applied automatically when showing availability

**Blackout dates:**
- Holidays, vacations, personal time
- These dates never show as available

**Lead time:**
- Minimum notice required: 48 hours, 1 week, etc.
- "Client can't book a session happening in 24 hours"

### Booking Restrictions

Protect yourself with smart restrictions.

**Minimum advance notice:**
Require bookings at least X hours/days before session:
- 48 hours (2 days): Gives you time to prepare, prevents last-minute chaos
- 1 week: Better for complex sessions that need planning

**Why it matters:**
Client books a mini session for tomorrow → You might not have time to prepare, scout location, or communicate details. Minimum notice ensures quality.

**Maximum advance booking:**
Don't allow bookings too far in advance:
- 6 months out: Your calendar isn't finalized that far ahead
- 3 months out: Gives clients planning time but keeps your schedule flexible

**Why it matters:**
If you let clients book 12 months in advance, your entire next year could fill with mini sessions before you realize you want to raise prices or take a vacation.

**Booking deadline:**
For mini session events, set a booking cutoff:
- 24 hours before event: "Booking closes Oct 19 at 9am"
- 48 hours before event: Gives you time to prepare and plan

**Why it matters:**
Last-minute bookings mean you don't know how many clients are coming. A deadline lets you plan accordingly.

**Maximum bookings per client:**
Prevent one person from hogging all slots:
- 1 slot per client for public mini sessions
- 2 slots if they want to book for multiple families (with approval)

**Why it matters:**
Someone could book all 10 slots "just in case" and then cancel most of them. This restriction keeps it fair.

**Payment requirement:**
Require payment or deposit at booking:
- Full payment: $200 due at booking
- Deposit: $50 due at booking, balance due day-of or after

**Why it matters:**
Free bookings lead to no-shows. Even a small deposit ($25) dramatically reduces no-show rates because clients have "skin in the game."

## Mini Session Calendar Availability

Your ShootPath calendar controls what shows as available for mini session bookings.

### How Calendar Affects Availability

**Automatic busy/free detection:**
ShootPath checks your calendar to prevent conflicts:

**If you have:**
- Job session 10am-12pm: Those slots unavailable for mini session booking
- Blocked time 1pm-3pm: Those slots unavailable
- No events 3pm-5pm: Those slots available (if within business hours)

**Real-time updates:**
- You schedule a client portrait at 11am
- That time immediately becomes unavailable on mini session booking page
- Clients see updated availability instantly

### Blocking Time for Mini Session Events

**When you create a mini session event:**
- The entire event time block appears on your calendar
- Individual slots are not separate calendar entries (would clutter your calendar)
- The event shows: "Fall Mini Sessions - 5 of 10 slots booked"

**Example:**
- Event: Oct 20, 9am-3pm (10 slots)
- Calendar shows: One block 9am-3pm labeled "Fall Mini Sessions"
- As slots book, the label updates: "Fall Mini Sessions (7/10 booked)"

**You can't book regular sessions during mini session event:**
If you try to schedule a regular portrait session at 10am on Oct 20:
- System warns: "Mini session event scheduled 9am-3pm"
- You can override if needed (e.g., you have an assistant running mini sessions)

### Preventing Conflicts

**ShootPath prevents:**
- Booking mini session slot during existing job session
- Booking job session during existing mini session slot
- Booking during blocked time
- Booking outside business hours
- Double-booking same time slot

**You can override** when needed:
- You have a second photographer covering mini sessions
- You're using a studio with multiple rooms
- You intentionally want to double-book (not recommended)

**Best practice:**
Trust the system. If it warns about a conflict, there's usually a good reason.

## Booking Confirmations and Reminders

Automatic communication keeps clients informed and reduces no-shows.

### Instant Booking Confirmation

**When client books:**
1. Confirmation screen appears: "You're booked!"
2. Confirmation email sent immediately
3. Email includes:
   - Session details (date, time, location)
   - What to bring/wear
   - Cancellation policy
   - Contact information if they have questions
   - Link to reschedule or cancel (if allowed)
   - Optional: Add to calendar button (.ics file)

**Why immediate confirmation matters:**
Clients need reassurance: "Did it work? Am I actually booked?" Instant confirmation eliminates uncertainty.

### Automated Reminders

**Set up reminder schedule:**
Go to **Settings > Email Templates > Mini Session Reminders** to configure:

**1 week before:**
- Subject: "Your mini session is coming up!"
- Content:
  - Reminder of date/time/location
  - What to wear suggestions
  - What to bring (if anything)
  - Reschedule link (if allowed)

**1 day before:**
- Subject: "See you tomorrow!"
- Content:
  - Final reminder
  - Address and parking info
  - Your phone number
  - Weather plan (if outdoor session)

**Day of (morning):**
- Subject: "Excited for your session today!"
- Content:
  - "See you at 10:30am!"
  - Directions/map link
  - Your contact number

**Post-session:**
- Subject: "Thank you for an amazing session!"
- Content:
  - Thank you message
  - When to expect gallery
  - What happens next

**Benefits:**
- Reduces no-shows by 50-70%
- Clients show up prepared (right location, right clothes)
- Fewer "where are we meeting?" messages day-of
- Professional, organized experience

**Customize per event:**
You can customize reminder templates for specific events:
- Holiday mini sessions might include "wear festive colors!"
- Outdoor events might include "bring bug spray in summer"

## Managing Client Expectations

Clear communication prevents confusion and creates happy clients.

### Setting Booking Policies

**Document your policies clearly:**

**Cancellation policy:**
- "Cancel 48 hours before for full refund"
- "Cancel 24-48 hours before for 50% refund"
- "Cancel less than 24 hours: no refund"

**Reschedule policy:**
- "One free reschedule with 48 hours notice"
- "Additional reschedules: $25 fee"

**Weather policy (outdoor sessions):**
- "If rain, we reschedule at no charge"
- "Photographer decides by 8am day-of"

**Late arrival policy:**
- "15 minutes late = session shortened"
- "30+ minutes late = session forfeited, no refund"

**No-show policy:**
- "No-show = full payment forfeited"
- "Please communicate if you're running late"

**Display policies:**
- On booking page (client must agree before booking)
- In confirmation email
- In reminder emails
- In contract (for full sessions)

**Why this matters:**
When policies are clear upfront, clients can't claim they "didn't know." It protects you and sets fair expectations.

### Communicating Availability

**Be clear about what clients can and can't book:**

**Can book directly:**
- Mini session time slots
- Consultation calls (if enabled)

**Requires quote first:**
- Full portrait sessions
- Weddings
- Commercial shoots
- Custom packages

**Not available for booking:**
- Last-minute requests (within your minimum notice period)
- Dates you're blocked/on vacation
- Times outside business hours

**On your website/booking page:**
> "Book a mini session instantly, or [contact me for custom sessions]."

This guides clients to the right booking method.

### Handling Booking Questions

**Common client questions:**

**"Can I book a slot for my friend too?"**
- If they're booking on friend's behalf: Yes, just enter friend's info
- If they want multiple slots: Check your max bookings policy

**"All the good times are taken. Can you add another slot?"**
- If you have capacity: Yes, manually add slot
- If you're at capacity: Offer waitlist or next event date

**"I booked the wrong time. Can I change it?"**
- Within your reschedule policy: Yes, client can self-reschedule (if enabled)
- Outside policy: You can manually move them if slot is available

**"What if it rains?"** (for outdoor mini sessions)
- Point to weather policy in confirmation email
- Reassure: "I'll monitor forecast and notify you by [time] if we reschedule"

**"Can I bring my dog?"**
- If allowed: "Yes! Just noted in your booking details."
- If not allowed: "Sorry, not for this event. I offer private pet sessions!"

**Have FAQ section** on booking page to answer these preemptively.

## Rescheduling Client Bookings

When clients need to change their booking.

### Client-Initiated Reschedules

**Enable self-service rescheduling:**
- Include reschedule link in confirmation email
- Client clicks link → authenticated by email
- Sees available alternative slots
- Selects new time
- Confirmation sent for new time

**Restrictions:**
- Can only reschedule within policy (e.g., 48 hours notice)
- Can only reschedule to available slots
- Can only reschedule X times (e.g., once free, then fee)

**Reschedule fee (optional):**
- Charge $25 for additional reschedules
- Reduces frivolous rescheduling
- Processed through Stripe automatically

### Manual Rescheduling

**When client contacts you:**
1. Open mini session event
2. Go to **Bookings**
3. Find client's booking
4. Click **Reschedule**
5. Choose new available slot
6. Save
7. System:
   - Moves booking to new slot
   - Original slot becomes available
   - Sends updated confirmation to client

**If new slot isn't available:**
- Offer to add extra slot (if you have time)
- Offer next event date
- Offer spot on waitlist

### Weather Reschedules

**For outdoor mini sessions:**

**Monitoring weather:**
- Check forecast 5 days before event
- Check again 48 hours before
- Make final call 12-24 hours before

**If rain/bad weather forecast:**
1. Send message to ALL booked clients: "Looks like rain Saturday. We're rescheduling to Sunday at the same times."
2. In ShootPath:
   - Create new event (Sunday)
   - Move all bookings to Sunday (bulk action)
   - Cancel Saturday event
3. Confirm clients received message and new time works
4. If new time doesn't work for some: Offer future date

**Have backup date planned:**
- When creating outdoor event, block the following day as backup
- Include in event description: "Rain date: Oct 21"
- Makes rescheduling smoother

## Troubleshooting Client Booking

### Clients Can't Complete Booking

**Common issues:**

**Payment failing:**
- Check Stripe integration is active
- Ensure test mode is off (if live)
- Client might have payment method issue
- Offer to process payment manually or over phone

**Slot showing as available but won't book:**
- Might have been booked by someone else seconds before
- Refresh availability page
- Suggest alternative slot

**Form validation errors:**
- Client entering email incorrectly
- Phone number format not recognized
- Special characters in name field
- Review form requirements and adjust if too strict

**Link not working:**
- URL might have typo
- Event might be unpublished or expired
- Check event status and republish

### Bookings Not Appearing on Calendar

**Check:**
1. Is event published? (Draft events don't sync to calendar)
2. Is calendar filter hiding this event type?
3. Is calendar showing correct date range?

**Fix:**
- Publish event
- Clear calendar filters
- Navigate to event date
- Refresh calendar

### Double-Booking Issues

**How it happens:**
- Two people click "Book" at exact same second
- System processes both before marking slot unavailable
- Rare, but possible

**Prevention:**
ShootPath uses transaction locks to prevent this, but if it happens:
1. Contact both clients immediately
2. Apologize for the error
3. Offer both clients:
   - Alternative slot
   - Discount/free add-on as apology
   - Refund if they can't reschedule
4. Let one client choose first (whoever booked first timestamp)

## Best Practices Summary

**Enable self-booking for mini sessions:**
It's faster, more professional, and increases bookings.

**Keep custom jobs manual:**
Full sessions need quotes, contracts, and personal touch. Don't try to fully automate them.

**Set clear policies:**
Cancellation, reschedule, weather, no-show policies prevent disputes.

**Require deposits:**
Even $25 dramatically reduces no-shows and frivolous bookings.

**Send automated reminders:**
1 week, 1 day, day-of. Reduces no-shows and client questions.

**Have backup plan for weather:**
Rain dates, clear weather policy, proactive communication.

**Monitor bookings:**
Check daily when event is open. Respond quickly to questions.

**Make it easy to find:**
Link to mini session booking from:
- Your website homepage
- Social media bios
- Email signature
- Blog posts

**Test the booking flow:**
Book a test slot yourself to see the client experience. Fix anything confusing.

**Review and refine:**
After each mini session event, review:
- What questions did clients ask? (Add to FAQ)
- What caused confusion? (Clarify on booking page)
- Did policies work? (Adjust for next event)

---

## What's Next?

Master client booking and calendar management with these related articles:

**[Calendar Overview](./index)** - Understand calendar view modes and navigation

**[Scheduling Sessions](./scheduling-sessions)** - Learn how to add sessions and block time

**[Calendar Integrations](./calendar-integrations)** - Sync with external calendars

**Related topics:**

**[Mini Sessions](../mini-sessions/)** - Complete guide to creating and marketing mini session events

**[Client Portal](../client-portal/)** - Learn what clients see when they access their portal

**[Workflows](../workflows/)** - Automate booking confirmations and reminders

---

**Questions?** Look for the help links throughout ShootPath, or use the support widget if you need assistance!
