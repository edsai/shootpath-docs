---
sidebar_position: 2
---

# Creating Email Templates

## Quick Reference

Building email templates is simple once you understand the three main components: template name (internal), subject line (what clients see), and body (your message with variables).

**Quick Steps:**
1. Go to **Settings > Email Templates**
2. Click **New Template**
3. Name your template (internal only)
4. Write subject line with variables
5. Write body with variables and formatting
6. Preview with test data
7. Save and use

**Template Editor Features:**
- Text formatting (bold, italic, links)
- Variable insertion buttons (no need to type `{{}}` manually)
- Real-time preview with sample data
- Mobile preview mode
- Template duplication for variations

**Common Use Cases:**
- Quote sent notification
- Contract signature reminder
- Gallery delivery announcement
- Payment reminders
- Session confirmations

---

## Detailed Guide

### Accessing the Template Editor

**Step 1: Navigate to Settings**

From your ShootPath dashboard:
1. Click your profile picture or initials (top right)
2. Select **Settings** from the dropdown
3. Click **Email Templates** in the left sidebar

You'll see your template library with all existing templates.

**Step 2: Create New Template**

Click the **New Template** button (usually top right of the templates list).

The template editor opens with three main sections:
- **Template name** - Internal identifier
- **Subject line** - What appears in client's inbox
- **Email body** - Your message content

### Template Name

The template name is for YOUR reference only - clients never see it. Use descriptive names that help you quickly find the right template.

**Naming Conventions:**

**Format:** `[Category] - [Type] - [Variation]`

**Examples:**
- `Quote - Wedding - Initial Send`
- `Quote - Wedding - Follow Up 3 Days`
- `Booking - Contract Reminder`
- `Gallery - Delivery Notification`
- `Payment - Deposit Due`
- `Session - Day Before Reminder`

**Good naming practices:**
- Be specific about purpose
- Include timing if it's part of a sequence
- Add genre if you have genre-specific templates
- Keep it concise (under 50 characters if possible)

**Examples of good vs bad names:**

✅ Good:
- `Quote - Portrait - Follow Up 1`
- `Booking Confirmation - Wedding`
- `Gallery Ready - Standard`
- `Contract Reminder - 7 Days`

❌ Bad:
- `Template 1`
- `Email`
- `The good one`
- `USE THIS ONE`
- `asdkfjh`

### Writing Subject Lines

The subject line is the first thing clients see. It determines whether they open your email immediately or let it sit in their inbox.

#### Subject Line Best Practices

**Be Clear and Specific**

Tell them exactly what the email is about:

✅ Good:
- "Your Wedding Photography Quote from Acme Studios"
- "Sarah, Your Gallery is Ready to View!"
- "Reminder: Family Session This Saturday"

❌ Vague:
- "Important Information"
- "Hi!"
- "Please Read"

**Use Personalization**

Including the client's name can increase open rates:

```
{{client_name}}, Your Portrait Gallery is Ready!
```

Becomes: "Sarah, Your Portrait Gallery is Ready!"

**Keep It Short**

Aim for 50-60 characters or less. Longer subject lines get cut off on mobile devices:

✅ "Your Wedding Quote from Acme Studios" (40 chars)
❌ "Here is the Custom Wedding Photography Quote You Requested from Acme Studios Including All Package Options" (110 chars)

**Create Urgency When Appropriate**

For time-sensitive emails:
- "Your quote expires in 3 days"
- "Reminder: Session tomorrow at 10am"
- "Action needed: Sign your contract"

But don't create fake urgency - clients see through it!

**Use Variables in Subject Lines**

Common variables for subject lines:
- `{{client_name}}` - Personalizes to recipient
- `{{job_type}}` - Wedding, Portrait, Event, etc.
- `{{session_date}}` - When the shoot happens
- `{{your_business}}` - Your business name

**Example subject lines:**

**Quote emails:**
```
Your {{job_type}} Quote from {{your_business}}
```
Result: "Your Wedding Quote from Acme Studios"

**Gallery delivery:**
```
{{client_name}}, Your Photos Are Ready! 📸
```
Result: "Sarah, Your Photos Are Ready! 📸"

**Reminders:**
```
Reminder: {{job_type}} Session on {{session_date}}
```
Result: "Reminder: Family Portrait Session on October 15"

**Contract signing:**
```
Action Needed: Sign Your {{job_type}} Contract
```
Result: "Action Needed: Sign Your Wedding Contract"

#### Subject Line Testing

Test subject lines by sending yourself the email:
- Does it make sense out of context?
- Is anything cut off on mobile?
- Would YOU open this email if you received it?

### Writing Email Body Content

The email body is where you communicate your message. Good templates balance personalization with efficiency.

#### Email Structure

**Standard structure:**

```
[Greeting]
Hi {{client_name}},

[Main Message - Why you're emailing]
I'm excited to share your wedding photography quote!

[Details/Information]
I've put together pricing based on what you're looking for:
- Coverage options from 6-12 hours
- Package add-ons to customize your experience
- Clear payment schedule

[Call to Action]
View your quote here: {{quote_link}}

[Next Steps/Closing]
If you have any questions about packages or pricing,
just reply to this email!

Looking forward to working with you.

[Signature]
Best,
{{your_name}}
{{your_business}}
{{your_phone}}
{{your_website}}
```

#### Greeting

Keep it simple and friendly:

**Simple greetings:**
```
Hi {{client_name}},
```

```
Hello {{client_name}},
```

```
Hey {{client_name}},
```

Choose the level of formality that matches your brand. Most photographers use "Hi" - it's friendly without being too casual.

**Avoid overly formal greetings:**
- "Dear Sir or Madam" (too stiff)
- "To Whom It May Concern" (impersonal)
- "Greetings" (sounds like a robot)

#### Opening Line

Hook them immediately with why you're emailing:

**For quote emails:**
```
Thanks for your inquiry about {{job_type}} photography!
I'm excited about the possibility of working with you.
```

**For gallery delivery:**
```
Your photos are ready! I'm so excited to share them with you.
```

**For reminders:**
```
Just a quick reminder that your {{job_type}} session
is coming up on {{session_date}}!
```

**For follow-ups:**
```
I wanted to check in about the quote I sent a few days ago.
Do you have any questions?
```

#### Main Content

This is where you provide necessary information. Keep it scannable:

**Use short paragraphs:**
```
I've put together a custom quote based on what you're looking for.

The quote includes three package options, each with different
coverage hours and deliverables. You can also add extras like
an engagement session or photo album.

Pricing is clearly laid out with no hidden fees, and you'll
see the payment schedule so you know exactly when payments are due.
```

**Use bullet points for lists:**
```
Your gallery includes:
- 250+ edited high-resolution photos
- 30-day online viewing and download access
- Easy sharing with friends and family
- Print ordering available (optional)
```

**Use formatting sparingly:**
- **Bold** for emphasis on key points
- *Italic* for subtle emphasis
- Links for actions (View Quote, Sign Contract, etc.)

**Avoid:**
- SHOUTING IN ALL CAPS
- Too many exclamation points!!!
- Walls of text without breaks
- Overly complex sentences

#### Call to Action

Tell clients exactly what to do next:

**Be explicit:**
```
View your quote here: {{quote_link}}
```

```
Sign your contract here: {{contract_link}}
```

```
View and download your photos: {{gallery_link}}
```

**Make it clickable:**
Use the link variable directly rather than "click here":

✅ Better:
```
{{quote_link}}
```

✅ Also good:
```
[View Your Quote]({{quote_link}})
```

❌ Less effective:
```
Click here to view your quote: {{quote_link}}
```

**Provide alternative if needed:**
```
View your quote: {{quote_link}}

(If the link doesn't work, copy and paste this URL into your browser)
```

#### Closing

Wrap up with next steps or an invitation to respond:

**Inviting questions:**
```
If you have any questions about packages, pricing, or anything else,
just reply to this email - I'm here to help!
```

**Setting expectations:**
```
I'll follow up in a few days if I haven't heard from you,
but feel free to reach out anytime!
```

**Expressing excitement:**
```
I'm so excited about the possibility of photographing your wedding!
```

**Simple professional close:**
```
Looking forward to hearing from you.
```

#### Signature

Include your contact information:

**Standard signature:**
```
Best,
{{your_name}}
{{your_business}}
{{your_phone}}
{{your_email}}
{{your_website}}
```

**Simplified signature:**
```
{{your_name}}
{{your_business}}
{{your_phone}}
```

**With social media:**
```
{{your_name}}
{{your_business}}

📞 {{your_phone}}
📧 {{your_email}}
🌐 {{your_website}}
📷 Instagram: @yourusername
```

Choose the level of detail that makes sense for your brand.

### Using Variables

Variables are the secret sauce that makes templates powerful. They automatically populate with real data when you send the email.

#### Variable Syntax

Variables use double curly braces:
```
{{variable_name}}
```

#### Inserting Variables

**Option 1: Variable Button (Easiest)**

The template editor has a "Variables" button or dropdown that lists all available variables. Click the variable you want and it's inserted at your cursor position.

**Option 2: Type Manually**

If you know the variable name, just type:
```
{{client_name}}
```

Make sure to use exactly matching names (case-sensitive) and proper syntax with double curly braces.

#### Common Variables by Category

**Client Information:**
- `{{client_name}}` - Client's first name or full name
- `{{client_email}}` - Client's email
- `{{client_phone}}` - Client's phone number

**Job Details:**
- `{{job_type}}` - Wedding, Portrait, Event, etc.
- `{{session_date}}` - Date of shoot (formatted)
- `{{session_time}}` - Time of shoot
- `{{session_location}}` - Location/venue name

**Pricing:**
- `{{quote_total}}` - Total amount ($2,500)
- `{{deposit_amount}}` - Deposit due
- `{{balance_amount}}` - Remaining balance
- `{{deposit_due_date}}` - When deposit is due
- `{{final_due_date}}` - When balance is due

**Links:**
- `{{quote_link}}` - URL to view quote
- `{{contract_link}}` - URL to sign contract
- `{{invoice_link}}` - URL to pay invoice
- `{{gallery_link}}` - URL to view gallery
- `{{questionnaire_link}}` - URL to fill out questionnaire

**Your Business Info:**
- `{{your_name}}` - Your name
- `{{your_business}}` - Business name
- `{{your_email}}` - Your email
- `{{your_phone}}` - Your phone
- `{{your_website}}` - Your website URL

[Complete variable reference →](./template-variables)

#### Variable Examples in Context

**Example 1: Quote Email**

```
Hi {{client_name}},

Thanks for your interest in {{job_type}} photography!
Based on our conversation, I've prepared a custom quote
for your {{session_date}} session.

View your quote: {{quote_link}}

Total investment: {{quote_total}}
Deposit to book: {{deposit_amount}}
Balance due: {{balance_amount}}

Questions? Just reply to this email!

Best,
{{your_name}}
{{your_business}}
{{your_phone}}
```

**Example 2: Gallery Delivery**

```
Hi {{client_name}},

Your {{job_type}} photos are ready! I loved photographing
your session and I'm thrilled to share these images with you.

View your gallery: {{gallery_link}}

Your gallery includes {{photo_count}} edited photos available
for viewing, downloading, and print ordering.

Enjoy!

{{your_name}}
```

**Example 3: Session Reminder**

```
Hi {{client_name}},

Just a friendly reminder that your {{job_type}} session
is tomorrow!

📅 Date: {{session_date}}
🕐 Time: {{session_time}}
📍 Location: {{session_location}}

See you soon!

{{your_name}}
{{your_phone}}
```

### Formatting Your Template

Good formatting makes emails easier to read and more professional.

#### Text Formatting

Most template editors support:
- **Bold** - For emphasis on key points
- *Italic* - For subtle emphasis
- Underline - Use sparingly (looks like links)
- Links - For clickable URLs

**Use bold for:**
- Important dates or deadlines
- Key action items
- Amounts or numbers that matter

**Example:**
```
**Important:** Your deposit of {{deposit_amount}} is due by {{deposit_due_date}}.
```

#### Paragraph Breaks

Use short paragraphs (2-3 sentences max) with blank lines between them:

✅ Good:
```
Hi Sarah,

Your quote is ready! I've included three package options
based on what you're looking for.

View your quote here: [link]

Questions? Just reply to this email.
```

❌ Hard to read:
```
Hi Sarah, Your quote is ready! I've included three package
options based on what you're looking for. View your quote
here: [link]. Questions? Just reply to this email.
```

#### Lists

Use bullet points or numbered lists for multiple items:

**Bullet points:**
```
Your session includes:
- 60 minutes of shooting time
- 25+ edited high-resolution photos
- Online gallery for viewing and downloading
- Print ordering available
```

**Numbered lists:**
```
Here's what happens next:
1. Review your quote
2. Accept if you're ready to book
3. Sign your contract
4. Pay your deposit
5. We'll schedule your session!
```

#### Emoji (Use Sparingly)

Emoji can add personality, but don't overdo it:

✅ Subtle:
```
📸 Your gallery is ready!
```

✅ Appropriate:
```
See you tomorrow! ☀️
```

❌ Too much:
```
🎉🎊🥳 OMG YOUR GALLERY IS HERE!!! 🎉🎊🥳
📸📷📸📷📸 100+ AMAZING PHOTOS!!! 📸📷📸📷📸
```

#### Links

Make important links stand out:

**Option 1: Standalone line**
```
View your quote here:
{{quote_link}}
```

**Option 2: Button-style (if your editor supports it)**
```
[View Your Quote]({{quote_link}})
```

**Option 3: Inline**
```
Your quote is ready: {{quote_link}}
```

### Preview and Testing

Always preview your template before using it with real clients.

#### Using the Preview Feature

Most template editors have a "Preview" button that shows:
- How the subject line looks
- How the email body renders
- How variables populate with sample data

**Check for:**
- ✅ All variables populate correctly
- ✅ Formatting looks good
- ✅ Links are clickable
- ✅ No weird spacing or line breaks
- ✅ Signature appears properly

#### Mobile Preview

Many clients read emails on their phones. Check mobile preview:
- Is text readable without zooming?
- Are links easy to tap?
- Is anything cut off or awkward?

#### Send Test Email

Send the template to yourself:
1. Click "Send Test" (if available)
2. Enter your email address
3. Send and check your inbox
4. Open on desktop AND mobile
5. Click all links to verify they work

**Test checklist:**
- [ ] Subject line makes sense
- [ ] Greeting is friendly
- [ ] Variables populated correctly
- [ ] Links work (even if they point to placeholder data)
- [ ] Formatting looks good
- [ ] No typos or grammar issues
- [ ] Mobile experience is good
- [ ] Signature appears correctly

### Template Examples for Common Scenarios

Here are complete templates for common situations.

#### Quote Sent Template

**Name:** `Quote - General - Initial Send`

**Subject:**
```
Your {{job_type}} Quote from {{your_business}}
```

**Body:**
```
Hi {{client_name}},

Thanks so much for reaching out about {{job_type}} photography!
I'm excited about the possibility of working with you.

I've put together a custom quote based on what you're looking for:
{{quote_link}}

The quote includes:
- Package options to fit your needs
- Available add-ons to customize your experience
- Clear pricing with no hidden fees
- Payment schedule details

Total investment: {{quote_total}}
Deposit to book: {{deposit_amount}}

Feel free to review at your convenience. If you have any questions
about packages, pricing, or anything else, just reply to this email!

Looking forward to hearing from you.

Best,
{{your_name}}
{{your_business}}
{{your_phone}}
{{your_website}}
```

#### Booking Confirmation Template

**Name:** `Booking - Confirmation`

**Subject:**
```
You're Booked! {{job_type}} on {{session_date}}
```

**Body:**
```
Hi {{client_name}},

Welcome aboard! I'm so excited to photograph your {{job_type}}.

Your session details:
📅 Date: {{session_date}}
🕐 Time: {{session_time}}
📍 Location: {{session_location}}

Next steps:
1. Sign your contract: {{contract_link}}
2. Pay your deposit: {{invoice_link}} ({{deposit_amount}})
3. Fill out your questionnaire: {{questionnaire_link}}

Once your deposit is received, you're officially booked!

I'll send more details about what to expect as we get closer
to your session date.

Can't wait!

{{your_name}}
{{your_business}}
{{your_phone}}
```

#### Gallery Ready Template

**Name:** `Gallery - Delivery Notification`

**Subject:**
```
{{client_name}}, Your Gallery is Ready! 📸
```

**Body:**
```
Hi {{client_name}},

Your {{job_type}} photos are here! I loved working with you
and I'm thrilled to share these images.

View your gallery:
{{gallery_link}}

Your gallery includes {{photo_count}} edited high-resolution photos.
You can view, download, share, and order prints for the next 30 days.

To download your photos:
1. Click the gallery link above
2. Browse your photos
3. Click the download button for individual photos or download all at once

Print ordering is also available if you'd like professional prints,
canvases, or albums!

Thank you for trusting me to capture these memories for you.
It was truly a pleasure!

{{your_name}}
{{your_business}}
{{your_phone}}
```

#### Payment Reminder Template

**Name:** `Payment - Deposit Reminder - 3 Days`

**Subject:**
```
Reminder: Deposit Due for {{job_type}} Session
```

**Body:**
```
Hi {{client_name}},

Just a friendly reminder that your deposit of {{deposit_amount}}
is due by {{deposit_due_date}}.

Pay your deposit here: {{invoice_link}}

Once your deposit is received, you're officially booked for
{{session_date}}!

If you've already paid, please disregard this message - it may
have crossed paths with your payment.

Questions? Just reply to this email.

Best,
{{your_name}}
{{your_phone}}
```

#### Quote Follow-Up Template

**Name:** `Quote - Follow Up - 3 Days`

**Subject:**
```
Following up on your {{job_type}} quote
```

**Body:**
```
Hi {{client_name}},

I wanted to follow up on the {{job_type}} quote I sent a few days ago.
I'd love to work with you!

View your quote: {{quote_link}}

Do you have any questions about:
- Package options or what's included?
- Pricing or payment plans?
- My photography style or process?
- Availability for your date?

I'm here to help make your decision easier. Just reply to this
email with any questions!

Best,
{{your_name}}
{{your_business}}
{{your_phone}}
```

### Advanced Features

Once you're comfortable with basic templates, explore advanced features.

#### Conditional Content

Show different content based on conditions:

**Example: Different messages for paid vs unpaid deposits**
```
{{#if deposit_paid}}
Thanks for paying your deposit! You're all set for {{session_date}}.
{{else}}
Reminder: Your deposit of {{deposit_amount}} is due by {{deposit_due_date}}.
Pay here: {{invoice_link}}
{{/if}}
```

#### Loops/Repeated Content

Display lists of items:

**Example: Show all selected packages**
```
You've selected:
{{#each packages}}
- {{this.name}}: {{this.price}}
{{/each}}
```

#### HTML Customization

If you know HTML/CSS, you can customize styling:

```html
<div style="background: #f5f5f5; padding: 20px; border-radius: 8px;">
  <h2 style="color: #333;">Important Information</h2>
  <p>Your session is coming up!</p>
</div>
```

**Use HTML sparingly:**
- Keep it simple
- Many email clients don't support advanced CSS
- Test in multiple email clients
- Provide plain text alternative

### Managing Templates

#### Duplicating Templates

To create a variation of an existing template:
1. Find the template you want to copy
2. Click the duplicate/copy button
3. Give it a new name
4. Modify as needed
5. Save

This is faster than starting from scratch!

#### Archiving Templates

Don't delete old templates - archive them:
- Move to "Archive" category
- Keep them for reference
- Easy to restore if needed later

#### Version History (if available)

Some systems track template changes:
- See what changed and when
- Restore previous versions
- Useful if you break something!

### Common Mistakes When Creating Templates

**Mistake 1: Using Variables That Don't Exist Yet**

❌ Using `{{gallery_link}}` in a quote email - there's no gallery yet!

✅ Only use variables that exist at the time the email is sent

**Mistake 2: Forgetting to Test**

❌ Creating a template and using it immediately without testing

✅ Always send a test email to yourself first

**Mistake 3: Too Much Text**

❌ Writing a novel in your email template

✅ Keep it concise - link to your website for more info

**Mistake 4: Unclear Call to Action**

❌ "Let me know what you think!"

✅ "View your quote here: [link]"

**Mistake 5: No Mobile Preview**

❌ Only checking desktop view

✅ Always check mobile - most clients read email on phones!

### Template Maintenance

Templates need regular maintenance to stay effective.

#### Quarterly Review

Every 3 months:
- Read through all active templates
- Update any outdated information
- Refresh stale language
- Check that links still work
- Remove templates you're not using

#### Update Triggers

Update templates when:
- Your pricing changes
- Your website URL changes
- You change business name/branding
- You update your process
- Clients give feedback about confusion

#### Track Performance

Monitor template effectiveness:
- Open rates (subject line working?)
- Click rates (call to action working?)
- Response rates (message effective?)

Refine templates that underperform.

### Tips for Better Templates

**Write Like You Talk**

Read your template out loud. Does it sound like YOU? If not, rewrite it in your natural voice.

**Get Feedback**

Ask a friend: "If you received this email, would you understand what to do next?"

**Study Your Best Emails**

Look at manual emails you've sent that got great responses. What made them work? Turn those into templates!

**Start Simple**

Your first templates don't need to be perfect. Create a simple version, use it, refine it based on results.

**Steal (Ethically)**

Look at emails you receive from businesses you admire. What do they do well? Adapt their approach (but don't copy word-for-word).

### What's Next?

**Ready to use variables effectively?** → [Template Variables](./template-variables)

**Want to see ShootPath's built-in templates?** → [Default Templates](./default-templates)

**Need email writing tips?** → [Email Best Practices](./email-best-practices)

**Want to automate when templates are sent?** → [Workflows](../workflows/)

---

**Questions?** Look for the help links in ShootPath, or use the support widget for assistance!
