---
sidebar_position: 1
---

# Integrations Overview

## Quick Reference

Integrations connect ShootPath to the services that power your photography business - payments, email, and scheduling. Think of them as bridges between ShootPath and the tools you already use, creating one seamless workflow.

**Available Integrations:**
- **Stripe** - Accept credit card payments and manage invoicing
- **Gmail/SMTP** - Send emails from your own email address
- **Google Calendar** - Sync shoots to your calendar automatically

**Why Integrations Matter:**
- **Unified workflow** - Everything in one place, no switching between apps
- **Automation** - Actions in one system trigger updates in another
- **Client experience** - Professional, seamless experience across all touchpoints
- **Time savings** - No manual data entry or duplicate work

**Quick Setup:**
All integrations are managed in **Settings > Integrations**. Each integration takes 5-10 minutes to connect and requires you to authorize ShootPath to access the service securely.

**What Gets Connected:**
- Stripe connects to your bank account for deposits
- Email connects to your Gmail or SMTP server for sending
- Google Calendar syncs job dates and blocked time

**Articles in This Section:**
- [Stripe Integration](./stripe) - Accept payments securely
- [Email/SMTP Integration](./email-smtp) - Send from your own email
- [Google Calendar Integration](./google-calendar) - Two-way calendar sync

---

## Detailed Guide

### What Are Integrations?

Integrations are connections between ShootPath and external services. They allow ShootPath to perform actions on your behalf - like charging a client's credit card, sending an email from your Gmail account, or adding a wedding to your Google Calendar.

**How they work:**

1. **You authorize the connection** - Give ShootPath permission to access the service (e.g., "ShootPath can send emails using my Gmail account")
2. **ShootPath uses secure APIs** - Industry-standard connections that are encrypted and safe
3. **Actions happen automatically** - When you trigger something in ShootPath (like sending a quote), the integration handles the rest

**Example workflow without integrations:**
- Client accepts quote in ShootPath
- You copy client name and email to Gmail
- You manually compose payment request
- You add event to Google Calendar manually
- You switch back to ShootPath to mark it booked
- Repeat for every client... exhausting!

**Example workflow with integrations:**
- Client accepts quote in ShootPath
- **Automatic:** Email sent from your Gmail account
- **Automatic:** Invoice created and sent via Stripe
- **Automatic:** Wedding date added to Google Calendar
- **Automatic:** ShootPath marks job as booked
- You just focused on creative work!

### Core Integration Philosophy

ShootPath integrates with industry-leading services instead of building everything from scratch. Here's why:

**Best-in-class tools:**
- Stripe is THE standard for online payments
- Gmail is trusted by billions of users
- Google Calendar is universal

**Security and compliance:**
- Payment processors handle PCI compliance (card security)
- Email providers maintain deliverability reputation
- Calendar providers handle scheduling conflicts

**Reliability:**
- These services have 99.99%+ uptime
- They have massive teams dedicated to security and performance
- They're not going anywhere

**You control your data:**
- Your Stripe account belongs to YOU
- Your Gmail account is YOURS
- Your calendar is YOUR property
- If you ever leave ShootPath, you keep all of these

### Required vs. Optional Integrations

#### Required: Stripe

**Why it's required:**
ShootPath's invoicing system is built around Stripe. You cannot accept credit card payments without it.

**What you need:**
- A Stripe account (free to create)
- A bank account for deposits
- Business verification info (SSN/EIN, address)

**Cost:**
- No monthly fees
- 2.9% + $0.30 per successful transaction
- Example: Client pays $1,000, you receive $970.70

**Setup time:**
- 5-10 minutes to connect
- Instant verification (most cases) or 1-3 days (manual review)

[Learn how to connect Stripe →](./stripe)

#### Recommended: Gmail or SMTP

**Why you should connect it:**
Without email integration, ShootPath can't send emails to clients. You'd have to copy/paste everything manually.

**What you get:**
- Automated quote emails, booking confirmations, gallery notifications
- All emails come FROM your email address (not "noreply@shootpath.com")
- Professional appearance to clients

**Two options:**

**Option 1: Gmail** (easiest)
- Free for most photographers
- Quick OAuth connection (3 clicks)
- 500 emails per day limit (sufficient for most)

**Option 2: Custom SMTP** (for advanced users)
- Use your own domain (yourname@yourstudio.com)
- Higher sending limits
- Requires SMTP server credentials

**Cost:**
- Gmail: Free (included with Google Workspace for business email)
- SMTP: Depends on your email provider (usually included with hosting)

**Setup time:**
- Gmail: 2-3 minutes
- SMTP: 5-10 minutes (need to find server credentials)

[Learn how to set up email →](./email-smtp)

#### Optional: Google Calendar

**Why you might want it:**
If you use Google Calendar for your schedule, two-way sync means ShootPath and your calendar always match.

**What syncs:**
- Job session dates (weddings, portraits, events)
- Mini session events
- Blocked time (personal appointments, vacations)

**Direction:**
- **ShootPath → Calendar:** New bookings appear in calendar automatically
- **Calendar → ShootPath:** Block time in calendar, ShootPath won't double-book

**Why it's optional:**
If you don't use Google Calendar, you don't need this! ShootPath has its own built-in calendar that works great standalone.

**Cost:**
- Free with any Google account

**Setup time:**
- 3-5 minutes

[Learn about calendar sync →](./google-calendar)

### Integration Security

Every integration follows strict security standards to protect your business and client data.

#### How Authorization Works

**OAuth 2.0** (industry standard):

When you connect an integration, you're taken to the service's official website (Stripe, Gmail, Google Calendar) where you log in and explicitly grant permission.

**What you see:**
```
ShootPath is requesting access to:
- Send emails on your behalf
- View your email settings

[Deny] [Allow]
```

**What happens when you click Allow:**
- The service generates a secure token
- ShootPath stores this token (not your password!)
- ShootPath uses the token to act on your behalf
- You can revoke access anytime in the service's settings

**Why this is secure:**
- ShootPath never sees your password
- Tokens can be revoked without changing your password
- Tokens have limited permissions (only what you authorize)

#### Data Encryption

**In transit:**
All data sent between ShootPath and integrated services uses TLS/SSL encryption (the same security as online banking).

**At rest:**
Integration tokens are encrypted in ShootPath's database. Even if someone accessed the database, they couldn't read the tokens.

**Audit logging:**
ShootPath logs all integration actions for troubleshooting and security monitoring.

#### Revoking Access

**You can disconnect any integration at any time:**

1. Go to Settings > Integrations
2. Find the connected service
3. Click "Disconnect"
4. Confirm

**What happens:**
- ShootPath stops accessing that service immediately
- The integration token is deleted
- Previous actions (past payments, sent emails) remain unchanged
- You can reconnect later if needed

**Example scenarios:**
- You switch to a different payment processor → Disconnect Stripe
- You change email providers → Disconnect old, connect new
- You stop using Google Calendar → Disconnect it
- Security concern or account breach → Disconnect immediately for safety

### Setting Up Your Integrations

Here's the recommended order for connecting integrations when you first set up ShootPath:

#### Step 1: Connect Stripe (Required)

**Before your first booking:**
You need Stripe connected to accept payments. Even if you don't have a client yet, set this up first so you're ready when opportunities come.

**What you'll need:**
- Business name and address
- Bank account number and routing number
- Social Security Number (if sole proprietor) or EIN (if LLC/Corp)
- Photo ID for verification

**Time investment:**
- 10 minutes to connect
- Instant verification (usually) or 1-3 business days

[Detailed Stripe setup guide →](./stripe#connecting-stripe-to-shootpath)

#### Step 2: Connect Email (Highly Recommended)

**Immediately after Stripe:**
Without email, you can't send quotes or booking confirmations. This is the second most critical integration.

**Choose your path:**
- **Gmail** - If you use Gmail for business, this is easiest
- **SMTP** - If you use a custom domain email (yourname@yourstudio.com)

**What you'll need:**
- Gmail: Just your Google account login
- SMTP: Server address, port, username, password (from your email provider)

**Time investment:**
- Gmail: 3 minutes
- SMTP: 10 minutes (includes finding credentials)

[Detailed email setup guide →](./email-smtp)

#### Step 3: Connect Google Calendar (Optional)

**After you've used ShootPath for a week:**
Once you're comfortable with the basics (leads, quotes, bookings), add calendar sync for convenience.

**What you'll need:**
- Google account login
- Decide which calendar to sync to (if you have multiple)

**Time investment:**
- 5 minutes to connect
- 2 minutes to configure sync preferences

[Detailed calendar setup guide →](./google-calendar)

### Managing Your Integrations

All integrations are managed from one central location: **Settings > Integrations**

#### Integration Settings Screen

**What you'll see:**

Each integration shows:
- Connection status (Connected ✓ or Not Connected)
- When it was last connected
- Quick actions (Connect, Disconnect, View Settings)
- Link to detailed documentation

**Connected integrations show:**
- Account info (e.g., "Connected as yourname@gmail.com")
- Last successful action (e.g., "Last payment: 2 hours ago")
- Error status if something is broken (e.g., "Email sending failed")

#### Testing Your Integrations

**After connecting, always test:**

**Stripe:**
1. Create a test invoice
2. Pay it with a test card (Stripe provides these)
3. Confirm payment appears in Stripe dashboard

**Email:**
1. Create a test lead
2. Send a quote email
3. Check your sent folder - did it arrive?

**Google Calendar:**
1. Create a test job with a session date
2. Check Google Calendar - does the event appear?
3. Edit the date in ShootPath - does calendar update?

#### Monitoring Integration Health

ShootPath automatically monitors all integrations and notifies you of issues:

**Types of alerts:**
- "Stripe connection expired - please reconnect"
- "Email sending failed - check your SMTP settings"
- "Calendar sync hasn't updated in 24 hours"

**Where you see alerts:**
- Dashboard notifications
- Email to your account email
- Banner at top of integration settings page

**Common causes:**
- Token expired (just reconnect)
- Service is down (wait and retry)
- Settings changed (e.g., you changed your email password)

### Integration Workflows

Here's how integrations work together in common scenarios:

#### Scenario 1: Sending a Quote

**What you do:**
Click "Send Quote" on a lead in ShootPath

**What happens behind the scenes:**
1. **Email integration** composes email from your template
2. **Email integration** sends email from your Gmail/SMTP account
3. **ShootPath** generates secure portal link for client
4. **Email integration** includes link in email body
5. **ShootPath** logs sent email in lead activity

**Client experience:**
Email arrives from YOUR email address (not ShootPath), looks professional, includes link to view quote online

#### Scenario 2: Client Books and Pays

**What you do:**
Nothing! Client clicks through from their email.

**What happens behind the scenes:**
1. **ShootPath** client accepts quote online
2. **Email integration** sends you notification
3. **ShootPath** creates contract
4. **Email integration** sends contract signing request to client
5. **ShootPath** client signs contract
6. **Stripe integration** generates payment link
7. **Email integration** sends payment request to client
8. **Stripe integration** processes payment
9. **Stripe integration** deposits funds to your bank (2-3 days)
10. **Google Calendar integration** adds session date to your calendar
11. **Email integration** sends you payment confirmation

**Your experience:**
You get one notification: "Sarah booked and paid!" Everything else happened automatically.

#### Scenario 3: Delivering Gallery

**What you do:**
Upload photos, mark gallery ready

**What happens behind the scenes:**
1. **ShootPath** finalizes gallery
2. **Email integration** sends gallery notification to client
3. **ShootPath** generates secure gallery link
4. **Email integration** includes download instructions
5. **Google Calendar integration** marks job complete (removes from production)

**Client experience:**
Email arrives: "Your photos are ready!" with link to beautiful gallery and clear download instructions

### Best Practices for Integrations

**1. Set Up All Integrations During Onboarding**

Don't wait! Get everything connected before your first client. Last thing you want is to land a booking and realize you can't send invoices.

**2. Test Everything Before Going Live**

Run through a complete workflow with test data:
- Create test lead
- Send test quote
- Accept test quote
- Process test payment with Stripe test card
- Check test event in calendar

**3. Monitor Integration Health Weekly**

Quick check (2 minutes):
- Settings > Integrations
- Verify all show "Connected ✓"
- Check for any error messages
- If issues exist, address immediately

**4. Keep Service Accounts Secure**

Use strong passwords and enable two-factor authentication on all connected services (Stripe, Gmail, Google Calendar).

**5. Document Your Integration Setup**

Keep a simple note with which accounts are connected (email addresses), date connected, and purpose. Helps with troubleshooting later!

### What's Next?

Ready to connect your integrations? Start with these detailed guides:

**[Stripe Integration](./stripe)** - Accept credit card payments securely. Start here first!

**[Email/SMTP Integration](./email-smtp)** - Send professional emails from your own address. Set up second!

**[Google Calendar Integration](./google-calendar)** - Keep your schedule synced automatically. Optional but convenient!

Or explore related topics:

**[Invoices](../invoices/)** - Learn how to create invoices that Stripe processes

**[Email Templates](../email-templates/)** - Customize the emails sent through your email integration

**[Calendar](../calendar/)** - Understand ShootPath's built-in calendar (works with or without Google Calendar sync)

---

**Questions?** Look for the help links throughout ShootPath, or reach out to support if you need assistance!
