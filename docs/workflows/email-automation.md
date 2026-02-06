---
sidebar_position: 5
---

# Email Automation

## Quick Reference

Email automation in ShootPath sends the right message to the right client at the right time—automatically. You write the emails once, and workflows send them based on triggers and timing.

**What Gets Automated:**
- Quote sent confirmations
- Follow-up reminders
- Contract and invoice emails
- Session reminders
- Gallery notifications
- Thank you messages

**How It Works:**
1. You create email templates (or use defaults)
2. Workflows trigger emails based on events
3. Emails send automatically with dynamic content (client name, dates, links)
4. You can preview, edit, or override any automated email

**Benefits:**
- Never forget to send important emails
- Consistent communication across all clients
- Save hours per week on repetitive emails
- Professional, timely client experience

**Quick Access:**
- **Email Templates** - Settings > Email Templates
- **Workflow Email Settings** - Settings > Workflows > [Workflow] > [Stage]
- **Email History** - View in job timeline or email log

:::tip Start With Defaults
ShootPath includes pre-written email templates that work well for most photographers. Use them as-is initially, then customize to match your voice!
:::

---

## Detailed Guide

### Why Email Automation Matters

**Time savings:**
Imagine sending 10-15 emails per job manually: quote sent, contract reminder, deposit reminder, questionnaire, session reminder, gallery notification... That's exhausting!

With automation, you write each email once. Workflows handle the sending. You save 30-60 minutes per job!

**Consistency:**
Every client gets the same professional experience. No one is forgotten because you were busy editing another job.

**Timeliness:**
Emails send at optimal times without you having to remember. Follow-ups happen automatically on day 5, not day 7 because you forgot.

**Professionalism:**
Clients notice when you're on top of things. Automated confirmations and reminders make you look organized—because you are!

### Email Templates vs. Automated Emails

Let's clarify the difference:

**Email Templates:**
Pre-written email content stored in ShootPath. They include placeholders for dynamic content like `{{clientName}}` or `{{sessionDate}}`.

**Think of templates as:** Your email scripts

**Automated Emails:**
Emails that workflows send automatically using templates. The workflow decides when to send, which template to use, and to whom.

**Think of automated emails as:** The delivery system

**Example:**

**Template:** "Contract Signing Request"
```
Hi {{clientName}},

I'm so excited to work with you! Please review and sign your contract here:
{{contractLink}}

Let me know if you have any questions!

Best,
{{yourName}}
```

**Automated Email:** Job workflow sends this template automatically when a job is created and contract is generated.

**Result:** Client receives a personalized email without you lifting a finger!

### Default Email Templates

ShootPath includes templates for common scenarios:

#### Lead Workflow Emails

**"Quote Sent"**
- When: Quote is sent to client
- Purpose: Provide direct link to quote and next steps
- Includes: Quote link, package summary, expiration date

**"Follow-Up #1"**
- When: 5 days after quote with no response
- Purpose: Gentle reminder and offer to answer questions
- Includes: Quote link, "any questions?" prompt

**"Follow-Up #2"**
- When: 10 days after quote with no response
- Purpose: Final reminder with urgency (expiration)
- Includes: Quote expiration date, offer to discuss

**"Booking Confirmation"**
- When: Client accepts quote
- Purpose: Celebrate booking and explain next steps
- Includes: What happens next (contract, deposit), portal link

#### Job Workflow Emails

**"Contract Signing Request"**
- When: Job created, contract generated
- Purpose: Direct client to sign contract
- Includes: Contract link, brief terms overview, e-signature instructions

**"Deposit Invoice"**
- When: Contract signed
- Purpose: Request deposit payment
- Includes: Invoice link, amount due, payment methods

**"Questionnaire Request"**
- When: Deposit paid, 2-3 weeks before session
- Purpose: Gather session details and preferences
- Includes: Questionnaire link, why it's important, deadline

**"Session Reminder"**
- When: 7 days before session
- Purpose: Confirm details and build excitement
- Includes: Date, time, location, what to bring/wear, weather considerations

**"Post-Session Update"**
- When: Session marked complete
- Purpose: Thank client and set delivery expectations
- Includes: Thank you, estimated delivery date, sneak peek (optional)

**"Gallery Ready"**
- When: Gallery uploaded and published
- Purpose: Notify client photos are ready
- Includes: Gallery link, download instructions, print ordering, sharing guidelines

**"Final Invoice"**
- When: Gallery delivered but balance remains
- Purpose: Request final payment
- Includes: Invoice link, amount due, payment methods

**"Thank You"**
- When: Final payment received
- Purpose: Express gratitude and request review/referral
- Includes: Thank you message, review request, gallery link for reference

### Creating Custom Email Templates

To create a new email template:

1. Go to **Settings > Email Templates**
2. Click **"New Template"**
3. Fill in template details:
   - **Name:** "Pre-Wedding Timeline Coordination"
   - **Subject:** "Planning Your Wedding Timeline"
   - **Body:** Your email content with placeholders
4. Preview and test
5. Save

**Template Components:**

**Subject Line:**
Keep it clear and personal:
- ✅ "Your Contract is Ready, {{clientName}}!"
- ❌ "ShootPath Contract Notification"

**Greeting:**
Use placeholders for personalization:
- "Hi {{clientName}},"
- "Hey {{clientFirstName}}!"
- "Hello {{clientName}} and {{secondaryClientName}}," (for weddings)

**Body:**
Write in your voice! Don't sound like a robot:
- ✅ "I'm so excited to photograph your wedding!"
- ❌ "Your booking has been confirmed in the system."

**Call to Action:**
Make it clear what they should do:
- "Click here to sign your contract: {{contractLink}}"
- "View your gallery now: {{galleryLink}}"
- "Pay your deposit: {{invoiceLink}}"

**Closing:**
Sign off naturally:
- "Can't wait to work with you!"
- "Let me know if you have questions!"
- "See you soon!"

**Signature:**
Use placeholders for consistency:
- "{{yourName}}"
- "{{businessName}}"
- "{{yourPhone}} | {{yourEmail}}"

### Dynamic Placeholders

Placeholders automatically fill in with job-specific information when emails send.

**Available Placeholders:**

**Client Information:**
- `{{clientName}}` - Full name
- `{{clientFirstName}}` - First name only
- `{{clientEmail}}` - Email address
- `{{clientPhone}}` - Phone number
- `{{secondaryClientName}}` - For weddings with two clients

**Job Information:**
- `{{jobType}}` - Wedding, Portrait, Event, etc.
- `{{jobNumber}}` - JOB-2026-0015
- `{{sessionDate}}` - February 15, 2026
- `{{sessionTime}}` - 2:00 PM
- `{{sessionLocation}}` - Central Park, NYC

**Financial Information:**
- `{{totalAmount}}` - $3,500
- `{{depositAmount}}` - $1,000
- `{{balanceAmount}}` - $2,500
- `{{invoiceLink}}` - Direct link to pay

**Business Information:**
- `{{yourName}}` - Your name
- `{{businessName}}` - Your business name
- `{{yourEmail}}` - Your email
- `{{yourPhone}}` - Your phone
- `{{businessWebsite}}` - Your website URL

**Workflow Links:**
- `{{quoteLink}}` - Link to view quote
- `{{contractLink}}` - Link to sign contract
- `{{invoiceLink}}` - Link to pay invoice
- `{{questionnaireLink}}` - Link to questionnaire
- `{{galleryLink}}` - Link to view gallery
- `{{portalLink}}` - General client portal link

**Example Template:**

```
Subject: Your {{jobType}} Gallery is Ready!

Hi {{clientFirstName}},

Your photos are here! 📸

I'm so excited to share your {{jobType}} gallery with you. Click below to view and download your photos:

{{galleryLink}}

You can download high-resolution files, share favorites with friends and family, and order prints directly from the gallery.

If you have any questions or would like to order an album or prints, just let me know!

Best,
{{yourName}}
{{businessName}}
{{yourPhone}} | {{yourEmail}}
```

**When sent, becomes:**

```
Subject: Your Wedding Gallery is Ready!

Hi Sarah,

Your photos are here! 📸

I'm so excited to share your Wedding gallery with you. Click below to view and download your photos:

https://shootpath.com/portal/abc123/gallery

You can download high-resolution files, share favorites with friends and family, and order prints directly from the gallery.

If you have any questions or would like to order an album or prints, just let me know!

Best,
Emma Johnson
Emma Johnson Photography
(555) 123-4567 | emma@example.com
```

See how personal it feels? That's the power of placeholders!

### Email Triggers

Triggers determine when automated emails send. There are three types:

#### 1. Event-Based Triggers

Emails send immediately when something happens.

**Examples:**
- Quote sent → Send "Quote Confirmation" email
- Contract signed → Send "Deposit Invoice" email
- Gallery published → Send "Gallery Ready" email
- Payment received → Send "Payment Received" email

**Why event-based?**
These are immediate responses to client actions or your actions. No delay needed!

#### 2. Time-Based Triggers

Emails send after a certain amount of time passes.

**Examples:**
- 5 days after quote sent → Send "Follow-Up #1"
- 7 days before session → Send "Session Reminder"
- 2 weeks after gallery delivered → Send "Print Sales Follow-Up"

**Why time-based?**
These are strategic delays. You don't want to follow up immediately—give clients time to review!

#### 3. Conditional Triggers

Emails send only if certain conditions are met.

**Examples:**
- If contract not signed after 3 days → Send "Contract Reminder"
- If balance due after gallery delivery → Send "Final Invoice"
- If questionnaire not completed 1 week before session → Send "Questionnaire Reminder"

**Why conditional?**
No need to send reminders if clients already took action. Conditional triggers avoid annoying unnecessary emails!

### Setting Up Automated Emails in Workflows

Let's walk through configuring an automated email in a workflow.

**Scenario:** You want to automatically send a questionnaire 2 weeks before the session.

**Steps:**

1. Go to **Settings > Workflows**
2. Select the job workflow
3. Find the "Pre-Session Prep" stage
4. Click **"Add Email"** or edit existing email
5. Configure the email:

**Email Settings:**

**Template:** Select "Questionnaire Request" template

**Trigger:**
- Type: Time-based
- When: 14 days before session date

**Recipient:** Primary client

**Conditions:**
- Only send if questionnaire status = "not completed"

**Send Test:** Send a test to your email to preview

**Save**

**Result:**
Every job using this workflow will automatically send a questionnaire email 2 weeks before the session—but only if the client hasn't already filled it out!

### Email Timing Best Practices

**Don't follow up too fast:**
Give clients 3-5 days to review quotes before following up. Immediately following up feels pushy.

**Don't wait too long:**
Following up after 2 weeks? They've probably booked someone else or forgotten about you.

**Strategic timing examples:**

**Quote follow-ups:**
- Day 0: Quote sent
- Day 5: Follow-up #1
- Day 10: Follow-up #2
- Day 14: Mark as lost if no response

**Pre-session communication:**
- 3-4 weeks before: Questionnaire
- 2 weeks before: Questionnaire reminder (if not completed)
- 7 days before: Session reminder with details
- 2 days before: Final confirmation (optional)

**Post-session communication:**
- Immediately: Thank you and delivery estimate
- Halfway through editing: "Working on your photos!"
- Gallery ready: "Photos ready!"
- 1 week after delivery: Follow-up about prints/album

**The "Goldilocks" principle:**
Not too fast (annoying), not too slow (forgettable), just right!

### Personalizing Automated Emails

Automated doesn't mean generic! Here's how to make automated emails feel personal:

#### 1. Use Conversational Language

**Generic:**
"Your contract has been generated and is awaiting signature."

**Personal:**
"I'm so excited to work with you! Please sign your contract here so we can get started: {{contractLink}}"

#### 2. Add Your Voice

Write like you talk! If you're bubbly and enthusiastic, show it. If you're calm and professional, reflect that.

**Example (Enthusiastic):**
"OMG your photos are ready! 🎉 I LOVE how they turned out—click here to see!"

**Example (Professional):**
"Your gallery is now available for viewing. I'm pleased with the results and hope you'll love them as much as I do."

#### 3. Include Context

Don't assume clients remember every detail.

**Bad:**
"Click here: {{galleryLink}}"

**Good:**
"Remember our amazing sunset session at the beach last month? Your photos are finally ready! I edited 45 of my favorites for you to download."

#### 4. Use Names (Not Generic Greetings)

**Generic:**
"Dear Client,"

**Personal:**
"Hi Sarah!"

Placeholders like `{{clientFirstName}}` make this easy!

#### 5. Add a Personal Line Manually

Even though the email is automated, you can add a quick personal note before it sends:

**Automated content:**
"Your gallery is ready! {{galleryLink}}"

**You add manually:**
"P.S. I especially loved the photos of you and your grandma—so sweet!"

This takes 30 seconds but makes a huge impact!

### Email Preview and Testing

Before activating automated emails, test them!

**How to preview:**

1. Go to email template
2. Click **"Preview"**
3. See how it looks with sample data

**How to test:**

1. Click **"Send Test"**
2. Enter your email address
3. Receive actual email with real formatting

**What to check:**

**Placeholders working?**
Do `{{clientName}}` and `{{galleryLink}}` populate correctly?

**Links working?**
Click all links—do they go to the right place?

**Formatting correct?**
Does it look good on mobile and desktop?

**Tone appropriate?**
Does it sound like you? Is it friendly/professional/clear?

**No typos?**
Proofread carefully! Automated emails go to many clients.

**Call to action clear?**
Is it obvious what the client should do next?

### Tracking Email Opens and Clicks

ShootPath tracks when clients open emails and click links.

**Why tracking matters:**

**See engagement:**
If a client opens your quote email 5 times, they're seriously interested! Great time to follow up.

**Measure effectiveness:**
Which emails get opened? Which get ignored? Improve low-performing emails.

**Know when to follow up:**
If they haven't opened the contract email, send a text: "Hey! Did you see my email?"

**What you can see:**

**Email sent:** Date and time email was sent

**Opened:** Did client open the email? When?

**Clicked:** Did they click links? Which ones?

**Replied:** Did they respond?

**Where to see tracking:**

**In job timeline:**
See all emails sent for a specific job with open/click status

**In email log:**
Go to **Reports > Email Log** to see all emails sent across all jobs

**In lead/job detail page:**
See email status in the communication history section

### Opt-Out and Unsubscribes

**Transactional emails (always sent):**
Emails about active bookings—contracts, invoices, gallery notifications—cannot be unsubscribed from. These are essential business communication.

**Marketing emails (optional):**
Newsletters, promotions, past client re-engagement—clients can unsubscribe from these.

**Automatic unsubscribe link:**
ShootPath adds an unsubscribe link to marketing emails automatically (required by law).

**Managing unsubscribes:**
If a client unsubscribes, they'll still receive transactional emails about their active jobs but not marketing communications.

### Email Automation by Job Type

Different photography types need different email cadences.

#### Wedding Workflow Emails

**Timeline:** Long (6-12 months)

**Key emails:**
- Booking confirmation with timeline overview
- Engagement session coordination (2 months before wedding)
- Timeline planning prompt (3 months before wedding)
- Vendor coordination (1 month before wedding)
- Pre-wedding reminder (1 week before)
- Post-wedding thank you and delivery estimate
- Gallery ready (6-8 weeks after wedding)
- Album design prompt (2 weeks after gallery)

**Why more emails?**
Weddings are complex with many moving parts. More touchpoints keep clients informed and reduce anxiety!

#### Portrait Session Emails

**Timeline:** Short (2-4 weeks)

**Key emails:**
- Booking confirmation
- Questionnaire (2 weeks before)
- Session reminder (3 days before)
- Post-session thank you
- Gallery ready (2 weeks after session)
- Thank you and review request

**Why fewer emails?**
Simple process, short timeline. Over-communication would be annoying!

#### Mini Session Emails

**Timeline:** Very short (1-2 weeks)

**Key emails:**
- Booking confirmation
- Session reminder (2 days before)
- Gallery ready (3-5 days after session)
- Print promotion (1 week after gallery)

**Why minimal emails?**
Fast turnaround, minimal prep. Keep it simple and quick!

### Handling Email Failures

Sometimes emails don't deliver. Here's why and what to do:

**Bounced emails:**
Email address is invalid or doesn't exist.

**Fix:** Update client email address, resend manually.

**Spam filters:**
Email caught by spam filter.

**Fix:** Ask client to check spam folder, whitelist your email address.

**Email service down:**
Your SMTP server or Gmail integration isn't working.

**Fix:** Check Settings > Integrations > Email. Reconnect if needed.

**Workflow not triggering:**
Email should have sent but didn't.

**Fix:** Check workflow settings. Is the trigger condition met? Is automation enabled?

**View failed emails:**
Go to **Reports > Email Log** and filter by "Failed." See error messages and retry.

### Best Practices for Email Automation

**Write in your authentic voice:**
Don't sound like a corporation. Write like you're talking to a friend!

**Keep emails concise:**
Get to the point. Clients skim emails—make the action clear.

**Use clear subject lines:**
Be specific, not vague:
- ✅ "Your Wedding Contract is Ready, Sarah!"
- ❌ "Action Required"

**Include context:**
Remind clients why they're getting the email. Don't assume they remember every detail.

**Make the next step obvious:**
Every email should have a clear call to action. What should they do?

**Test before deploying:**
Always send test emails to yourself first. Check on mobile and desktop.

**Monitor open rates:**
If nobody is opening your emails, the subject line needs work!

**Don't over-automate:**
Some things should stay personal (like thank you notes or complex discussions).

**Review quarterly:**
Every 3-6 months, review your automated emails. Update wording, fix issues, improve clarity.

### Troubleshooting Email Automation

**Emails not sending?**
- Check workflow is active (not paused)
- Verify email integration is connected (Settings > Integrations)
- Confirm trigger condition is met
- Check email log for error messages

**Placeholders not populating?**
- Ensure you're using correct placeholder syntax: `{{clientName}}` not `\{clientName\}`
- Verify the data exists (can't show session date if none is set)

**Wrong email sent?**
- Check which template is assigned to that workflow stage
- Edit the template if content is wrong

**Duplicate emails sent?**
- Check if you manually sent an email AND automation sent one
- Review workflow to avoid overlapping email triggers

**Clients not receiving emails?**
- Verify email address is correct
- Ask client to check spam folder
- Whitelist your sending email address

### What's Next?

Now that you understand email automation, explore these resources:

**[Workflow Tasks](./workflow-tasks)** - Learn how tasks and emails work together

**[Customizing Workflows](./customizing-workflows)** - Set up custom email triggers for your process

**[Default Workflows](./default-workflows)** - Review the default email automation

**[Email Templates](../email-templates/)** - Deep dive into creating and managing templates

---

**Questions?** Look for the help links throughout ShootPath, or use the support widget if you need assistance!
