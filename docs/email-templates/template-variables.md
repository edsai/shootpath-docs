---
sidebar_position: 3
---

# Template Variables Reference

## Quick Reference

Template variables are placeholders that automatically populate with real data when you send an email. They use double curly braces: `{{variable_name}}`

**Most Common Variables:**
- `{{client_name}}` - Client's name
- `{{job_type}}` - Wedding, Portrait, Event, etc.
- `{{session_date}}` - Date of shoot
- `{{quote_link}}` - Link to view quote
- `{{gallery_link}}` - Link to view gallery
- `{{your_name}}` - Your name
- `{{your_business}}` - Your business name

**Quick Tips:**
- Variables are case-sensitive: `{{client_name}}` ≠ `{{Client_Name}}`
- Not all variables work in all contexts (you can't use `{{gallery_link}}` before creating a gallery!)
- Test templates to ensure variables populate correctly
- Use the variable picker in the template editor to avoid typos

**Variable Categories:**
- [Client Information](#client-information)
- [Job & Session Details](#job--session-details)
- [Pricing & Payments](#pricing--payments)
- [Important Links](#important-links)
- [Your Business Info](#your-business-information)
- [Dates & Times](#dates--times)

---

## Detailed Guide

### How Variables Work

Variables are dynamic placeholders that get replaced with actual data when an email is sent.

**What you write in your template:**
```
Hi {{client_name}},

Your {{job_type}} session on {{session_date}} is confirmed!

View your contract: {{contract_link}}
```

**What the client receives:**
```
Hi Sarah,

Your Wedding session on October 15, 2024 is confirmed!

View your contract: https://app.shootpath.com/portal/abc123/contract
```

The system automatically pulls data from the lead, job, quote, or contract record and populates the variables.

### Variable Syntax

All variables use the same format:

```
{{variable_name}}
```

**Rules:**
- Must start and end with double curly braces `{{ }}`
- Variable names use lowercase with underscores: `client_name` not `ClientName`
- No spaces inside the braces: `{{client_name}}` not `{{ client_name }}`
- Case-sensitive: `{{Client_Name}}` won't work

**Inserting variables:**

**Option 1: Use the Variable Picker** (recommended)
- Click the "Insert Variable" button in the template editor
- Select the variable from the dropdown
- It's inserted at your cursor with correct syntax

**Option 2: Type Manually**
- Type exactly: `{{variable_name}}`
- Make sure spelling and case match exactly

### Client Information

Variables related to your client.

#### {{client_name}}

**What it does:** Client's full name or first name (depending on your settings)

**Example output:** "Sarah Thompson" or "Sarah"

**Common uses:**
- Email greetings: `Hi {{client_name}},`
- Subject lines: `{{client_name}}, Your Gallery is Ready!`
- Personalization: `Thanks {{client_name}} for choosing us!`

**Example template:**
```
Hi {{client_name}},

I'm so excited to work with you on your upcoming session!

Best,
Emma
```

**What the client sees:**
```
Hi Sarah,

I'm so excited to work with you on your upcoming session!

Best,
Emma
```

#### {{client_email}}

**What it does:** Client's email address

**Example output:** "sarah@example.com"

**Common uses:**
- Rarely used in client-facing emails (they already know their email!)
- More common in internal notifications or admin templates
- Account confirmation messages

**Example template:**
```
Account created for: {{client_email}}
```

#### {{client_phone}}

**What it does:** Client's phone number (formatted)

**Example output:** "(555) 123-4567" or "+1-555-123-4567"

**Common uses:**
- Confirmation emails showing contact info
- "Call me at..." messages
- Rarely needed in most templates

**Example template:**
```
If you have questions before your session, call or text me
or reach me at the number I have on file: {{client_phone}}
```

#### {{client_partner_name}}

**What it does:** Partner/spouse name (for couples)

**Example output:** "John"

**Common uses:**
- Wedding emails: `Hi {{client_name}} and {{client_partner_name}},`
- Engagement sessions
- Couple portraits

**Example template:**
```
Hi {{client_name}} and {{client_partner_name}},

Congratulations on your engagement! I'd love to photograph
your love story.

Best,
Emma
```

**What the couple sees:**
```
Hi Sarah and John,

Congratulations on your engagement! I'd love to photograph
your love story.

Best,
Emma
```

### Job & Session Details

Variables about the photography session or project.

#### {{job_type}}

**What it does:** Type of photography job

**Example output:** "Wedding", "Portrait", "Event", "Commercial", "Newborn", etc.

**Common uses:**
- Specifying what type of session: `Your {{job_type}} session...`
- Subject lines: `Your {{job_type}} Quote`
- Personalizing messages by genre

**Example template:**
```
Hi {{client_name}},

I'm excited about your upcoming {{job_type}} session!
{{job_type}} photography is one of my favorite genres.

Best,
Emma
```

**What the client sees:**
```
Hi Sarah,

I'm excited about your upcoming Wedding session!
Wedding photography is one of my favorite genres.

Best,
Emma
```

#### {{session_date}}

**What it does:** Date of the photography session (formatted)

**Example output:** "October 15, 2024" or "Saturday, October 15"

**Common uses:**
- Confirmations: `Your session on {{session_date}}...`
- Reminders: `Your session is tomorrow ({{session_date}})!`
- Calendar references

**Example template:**
```
Hi {{client_name}},

Quick reminder: Your {{job_type}} session is scheduled for
{{session_date}} at {{session_time}}.

See you soon!
Emma
```

**What the client sees:**
```
Hi Sarah,

Quick reminder: Your Wedding session is scheduled for
October 15, 2024 at 10:00 AM.

See you soon!
Emma
```

#### {{session_time}}

**What it does:** Time of the photography session

**Example output:** "10:00 AM", "2:30 PM", "14:30"

**Common uses:**
- Session confirmations
- Day-before reminders
- Coordination with clients

**Example template:**
```
Session Details:
📅 {{session_date}}
🕐 {{session_time}}
📍 {{session_location}}
```

#### {{session_location}}

**What it does:** Location or venue name

**Example output:** "Central Park", "Willow Creek Barn", "123 Main Street"

**Common uses:**
- Session confirmations
- Location reminders
- Direction references

**Example template:**
```
We'll meet at {{session_location}} on {{session_date}} at {{session_time}}.

If you need directions, let me know!
```

**What the client sees:**
```
We'll meet at Willow Creek Barn on October 15, 2024 at 10:00 AM.

If you need directions, let me know!
```

#### {{job_notes}}

**What it does:** Any internal notes about the job (use carefully!)

**Example output:** Whatever notes you've added to the job

**Common uses:**
- Internal templates only
- Referencing specific client requests
- Usually NOT used in client-facing emails

**Warning:** Only use this if you're careful about what you put in job notes!

### Pricing & Payments

Variables related to money and invoices.

#### {{quote_total}}

**What it does:** Total amount of the quote

**Example output:** "$2,500" or "$2,500.00"

**Common uses:**
- Quote emails: `Total investment: {{quote_total}}`
- Pricing summaries
- Confirmation of amounts

**Example template:**
```
Hi {{client_name}},

Your custom {{job_type}} quote is ready!

Total investment: {{quote_total}}
Deposit to book: {{deposit_amount}}
Balance due: {{balance_amount}}

View full details: {{quote_link}}

Best,
Emma
```

**What the client sees:**
```
Hi Sarah,

Your custom Wedding quote is ready!

Total investment: $5,000
Deposit to book: $2,500
Balance due: $2,500

View full details: [link]

Best,
Emma
```

#### {{deposit_amount}}

**What it does:** Amount of the deposit/retainer

**Example output:** "$1,250", "$500.00"

**Common uses:**
- Booking confirmations: `Deposit of {{deposit_amount}} due`
- Payment reminders
- Invoice descriptions

**Example template:**
```
To secure your booking, a deposit of {{deposit_amount}} is due
by {{deposit_due_date}}.

Pay your deposit: {{invoice_link}}
```

#### {{balance_amount}}

**What it does:** Remaining balance after deposit

**Example output:** "$1,250", "$2,500.00"

**Common uses:**
- Payment schedules
- Final payment reminders
- Quote summaries

**Example template:**
```
Payment Schedule:
- Deposit: {{deposit_amount}} (due at booking)
- Balance: {{balance_amount}} (due before session)

Total: {{quote_total}}
```

#### {{payment_amount}}

**What it does:** Amount of a specific payment/invoice

**Example output:** "$1,250"

**Common uses:**
- Invoice emails
- Payment confirmation
- Receipt notifications

**Example template:**
```
Thank you for your payment of {{payment_amount}}!

Your remaining balance is {{balance_amount}}.
```

#### {{deposit_due_date}}

**What it does:** When the deposit payment is due (formatted date)

**Example output:** "September 1, 2024"

**Common uses:**
- Payment reminders
- Booking confirmations
- Deadline communications

**Example template:**
```
Your deposit of {{deposit_amount}} is due by {{deposit_due_date}}.

Pay here: {{invoice_link}}
```

#### {{final_due_date}}

**What it does:** When the final balance is due

**Example output:** "October 1, 2024"

**Common uses:**
- Payment schedules
- Final payment reminders
- Timeline confirmations

**Example template:**
```
Payment Schedule:
✅ Deposit: {{deposit_amount}} - Due {{deposit_due_date}}
⏰ Balance: {{balance_amount}} - Due {{final_due_date}}
```

#### {{invoice_number}}

**What it does:** Invoice reference number

**Example output:** "INV-2024-0042", "10042"

**Common uses:**
- Invoice emails
- Payment references
- Accounting communications

**Example template:**
```
Invoice #{{invoice_number}}
Amount due: {{payment_amount}}
Due date: {{final_due_date}}

Pay here: {{invoice_link}}
```

### Important Links

Variables that generate URLs to portals and resources.

#### {{quote_link}}

**What it does:** URL to view the online quote

**Example output:** "https://app.shootpath.com/portal/abc123/quote"

**Common uses:**
- Quote emails
- Follow-up messages
- Quote reminders

**Example template:**
```
Hi {{client_name}},

Your {{job_type}} quote is ready!

View your quote: {{quote_link}}

The quote includes package options, pricing, and payment details.
Review it at your convenience!

Best,
Emma
```

**What the client sees:**
```
Hi Sarah,

Your Wedding quote is ready!

View your quote: https://app.shootpath.com/portal/abc123/quote

The quote includes package options, pricing, and payment details.
Review it at your convenience!

Best,
Emma
```

**Important:** Only use this variable in emails sent AFTER a quote is created!

#### {{contract_link}}

**What it does:** URL to view and sign the contract

**Example output:** "https://app.shootpath.com/portal/abc123/contract"

**Common uses:**
- Contract signature requests
- Contract reminders
- Booking confirmations

**Example template:**
```
Hi {{client_name}},

Congrats on booking! To finalize everything, please sign
your contract:

{{contract_link}}

The contract outlines what's included, payment schedule,
cancellation policy, and other important details.

Let me know if you have questions!

Emma
```

**Important:** Only use after a contract exists for the job!

#### {{invoice_link}}

**What it does:** URL to view and pay an invoice

**Example output:** "https://app.shootpath.com/portal/abc123/invoice/456"

**Common uses:**
- Payment requests
- Payment reminders
- Invoice notifications

**Example template:**
```
Hi {{client_name}},

Your {{job_type}} deposit invoice is ready!

Amount due: {{deposit_amount}}
Due date: {{deposit_due_date}}

Pay your invoice: {{invoice_link}}

Thank you!
Emma
```

**Important:** Only use after an invoice is created!

#### {{gallery_link}}

**What it does:** URL to view the photo gallery

**Example output:** "https://app.shootpath.com/portal/abc123/gallery"

**Common uses:**
- Gallery delivery notifications
- Gallery reminders
- Download instructions

**Example template:**
```
Hi {{client_name}},

Your photos are ready! 📸

View your gallery: {{gallery_link}}

Your gallery includes {{photo_count}} edited photos available
for viewing, downloading, and print ordering.

Gallery access expires in 30 days, so be sure to download
your favorites!

Enjoy!
Emma
```

**Important:** Only use after you've uploaded a gallery for the job!

#### {{questionnaire_link}}

**What it does:** URL to fill out a questionnaire

**Example output:** "https://app.shootpath.com/portal/abc123/questionnaire/789"

**Common uses:**
- Questionnaire requests
- Pre-session prep
- Information gathering

**Example template:**
```
Hi {{client_name}},

To help me prepare for your {{job_type}} session, please
fill out this quick questionnaire:

{{questionnaire_link}}

It takes about 5 minutes and helps me understand your vision,
preferences, and any special requests.

Thanks!
Emma
```

**Important:** Only use after assigning a questionnaire to the job!

#### {{portal_link}}

**What it does:** General URL to client's portal homepage

**Example output:** "https://app.shootpath.com/portal/abc123"

**Common uses:**
- Welcome emails
- "Check your portal" messages
- General portal access

**Example template:**
```
Hi {{client_name}},

You can always access your project details, contracts, invoices,
and gallery through your client portal:

{{portal_link}}

Bookmark this link for easy access!

Emma
```

### Your Business Information

Variables about you and your business.

#### {{your_name}}

**What it does:** Your name (or business owner name)

**Example output:** "Emma Rodriguez", "Emma"

**Common uses:**
- Email signatures
- Personal touches
- Sign-offs

**Example template:**
```
Looking forward to working with you!

Best,
{{your_name}}
```

**What the client sees:**
```
Looking forward to working with you!

Best,
Emma Rodriguez
```

#### {{your_business}}

**What it does:** Your business name

**Example output:** "Acme Photography Studio", "Emma Rodriguez Photography"

**Common uses:**
- Email signatures
- Subject lines: `Your Quote from {{your_business}}`
- Branding

**Example template:**
```
Thank you for choosing {{your_business}}!

{{your_name}}
{{your_business}}
{{your_phone}}
{{your_website}}
```

#### {{your_email}}

**What it does:** Your business email address

**Example output:** "hello@acmephoto.com", "emma@example.com"

**Common uses:**
- Email signatures
- Contact information
- Reply instructions

**Example template:**
```
Questions? Reply to this email or reach me at:
📧 {{your_email}}
📞 {{your_phone}}
```

#### {{your_phone}}

**What it does:** Your business phone number

**Example output:** "(555) 123-4567", "+1-555-123-4567"

**Common uses:**
- Email signatures
- Contact information
- "Call me" messages

**Example template:**
```
Feel free to call or text with any questions:
{{your_phone}}
```

#### {{your_website}}

**What it does:** Your website URL

**Example output:** "https://acmephoto.com", "www.acmephoto.com"

**Common uses:**
- Email signatures
- "Learn more" links
- Portfolio references

**Example template:**
```
Want to see more of my work? Check out my portfolio:
{{your_website}}

Best,
{{your_name}}
{{your_business}}
```

### Dates & Times

Variables related to dates and deadlines.

#### {{today}}

**What it does:** Today's date (when email is sent)

**Example output:** "September 15, 2024"

**Common uses:**
- Date-stamping emails
- Timelines ("As of {{today}}, your balance is...")
- Rarely needed in most templates

#### {{days_until_session}}

**What it does:** Number of days until the session

**Example output:** "7 days", "1 day", "14 days"

**Common uses:**
- Countdown reminders
- Urgency creation
- Session proximity notifications

**Example template:**
```
Hi {{client_name}},

Your {{job_type}} session is {{days_until_session}} away!

So excited to see you on {{session_date}}!

Emma
```

**What the client sees:**
```
Hi Sarah,

Your Wedding session is 7 days away!

So excited to see you on October 15, 2024!

Emma
```

#### {{days_since_gallery}}

**What it does:** Days since gallery was delivered

**Example output:** "5 days", "14 days"

**Common uses:**
- Gallery download reminders
- Expiration warnings
- Follow-up timing

**Example template:**
```
Hi {{client_name}},

It's been {{days_since_gallery}} since I delivered your gallery.

Your gallery access expires in 30 days, so be sure to
download your favorites soon!

View gallery: {{gallery_link}}
```

### Gallery & Delivery

Variables related to photo delivery.

#### {{photo_count}}

**What it does:** Number of photos in the gallery

**Example output:** "127", "250"

**Common uses:**
- Gallery delivery emails
- Setting expectations
- Summary information

**Example template:**
```
Hi {{client_name}},

Your gallery is ready with {{photo_count}} edited photos!

View your gallery: {{gallery_link}}

All photos are high-resolution and ready for download.

Enjoy!
Emma
```

**What the client sees:**
```
Hi Sarah,

Your gallery is ready with 250 edited photos!

View your gallery: [link]

All photos are high-resolution and ready for download.

Enjoy!
Emma
```

#### {{gallery_expiration_date}}

**What it does:** Date when gallery access expires

**Example output:** "November 15, 2024"

**Common uses:**
- Gallery delivery emails
- Expiration reminders
- Download deadline notices

**Example template:**
```
Your gallery will be available until {{gallery_expiration_date}}.

Please download your favorites before this date!
```

### Packages & Add-Ons

Variables for selected packages and extras.

#### {{selected_package}}

**What it does:** Name of the package the client selected

**Example output:** "Premium Wedding Package", "Standard Portrait Session"

**Common uses:**
- Booking confirmations
- Quote summaries
- Contract references

**Example template:**
```
Hi {{client_name}},

You've selected: {{selected_package}}

This includes:
- {{package_description}}

Total investment: {{quote_total}}

Best,
Emma
```

#### {{package_description}}

**What it does:** Description/details of the selected package

**Example output:** "8 hours coverage, 500+ edited photos, online gallery"

**Common uses:**
- Quote emails
- Booking confirmations
- Package summaries

#### {{selected_addons}}

**What it does:** List of add-ons the client selected

**Example output:** "Second Photographer, Engagement Session, Photo Album"

**Common uses:**
- Quote summaries
- Booking confirmations
- Invoice descriptions

**Example template:**
```
Package: {{selected_package}}
Add-ons: {{selected_addons}}

Total: {{quote_total}}
```

### Conditional Variables

These variables return true/false and are used with conditional logic.

#### {{deposit_paid}}

**What it does:** True if deposit has been paid

**Use with conditionals:**
```
{{#if deposit_paid}}
✅ Deposit received! You're all set.
{{else}}
Reminder: Your deposit of {{deposit_amount}} is still due.
Pay here: {{invoice_link}}
{{/if}}
```

#### {{contract_signed}}

**What it does:** True if contract has been signed

**Use with conditionals:**
```
{{#if contract_signed}}
✅ Contract signed!
{{else}}
⏰ Please sign your contract: {{contract_link}}
{{/if}}
```

#### {{gallery_uploaded}}

**What it does:** True if gallery has been delivered

**Use with conditionals:**
```
{{#if gallery_uploaded}}
Your gallery is ready! View here: {{gallery_link}}
{{else}}
I'm still editing your photos - they'll be ready soon!
{{/if}}
```

### Variable Context

Not all variables work in all situations. Here's when each variable is available:

#### Lead Emails (Before Booking)

**Available:**
- Client info: `{{client_name}}`, `{{client_email}}`, `{{client_phone}}`
- Business info: `{{your_name}}`, `{{your_business}}`, etc.
- Quote variables: `{{quote_link}}`, `{{quote_total}}`, etc.

**NOT Available:**
- Job-specific: `{{session_date}}`, `{{session_time}}`
- Contract: `{{contract_link}}`
- Gallery: `{{gallery_link}}`
- Invoices: `{{invoice_link}}` (unless you send a quote with deposit)

#### Job Emails (After Booking)

**Available:**
- Everything from lead emails, PLUS:
- Job info: `{{job_type}}`, `{{session_date}}`, `{{session_location}}`
- Contract: `{{contract_link}}` (once contract exists)
- Invoices: `{{invoice_link}}` (once invoices created)
- Gallery: `{{gallery_link}}` (once gallery uploaded)

#### Invoice Emails

**Available:**
- All job variables
- Payment variables: `{{payment_amount}}`, `{{invoice_number}}`, `{{invoice_link}}`
- Balance info: `{{balance_amount}}`

#### Gallery Emails

**Available:**
- All job variables
- Gallery variables: `{{gallery_link}}`, `{{photo_count}}`, `{{gallery_expiration_date}}`

### Testing Variables

Always test templates to ensure variables populate correctly.

**Testing checklist:**
- [ ] All variables show actual data (not `{{variable_name}}`)
- [ ] Links are clickable and work
- [ ] Dates format correctly
- [ ] Money amounts show currency symbol
- [ ] No "undefined" or error messages
- [ ] Mobile view looks good

**How to test:**
1. Create a test lead or job with real data
2. Send the template to yourself
3. Check that all variables populated
4. Click all links to verify they work
5. View on mobile device

### Common Variable Mistakes

**Mistake 1: Typos in Variable Names**

❌ `{{clint_name}}` (typo)
✅ `{{client_name}}` (correct)

**Mistake 2: Wrong Syntax**

❌ `{client_name}` (single braces)
❌ `{{ client_name }}` (spaces inside)
✅ `{{client_name}}` (double braces, no spaces)

**Mistake 3: Using Variables Before They Exist**

❌ Using `{{gallery_link}}` in a quote email (no gallery yet!)
✅ Only use variables appropriate for that email's context

**Mistake 4: Not Testing**

❌ Assuming variables work without testing
✅ Always send a test email before using with real clients

**Mistake 5: Hardcoding Info That Should Be Variables**

❌ "View your quote at: https://..."
✅ "View your quote: {{quote_link}}"

Variables automatically update if URLs change!

### Custom Variables

Some systems allow custom variables you define yourself.

**Example custom variables:**
- `{{studio_address}}` - Your physical address
- `{{instagram_handle}}` - Your Instagram username
- `{{booking_fee}}` - A specific fee amount
- `{{turnaround_time}}` - Your typical delivery timeline

Check your system's documentation for how to create custom variables!

### What's Next?

**Want to see complete template examples?** → [Default Templates](./default-templates)

**Need help writing templates?** → [Creating Templates](./creating-templates)

**Want email writing tips?** → [Email Best Practices](./email-best-practices)

---

**Questions?** Look for the help links in ShootPath, or use the support widget for assistance!
