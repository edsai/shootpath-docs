---
sidebar_position: 1
---

# Email Templates Overview

## Quick Reference

Email templates save you hours every week by automating repetitive client communication. Instead of typing the same "quote sent" or "gallery ready" email over and over, you create templates once and ShootPath sends them automatically.

**What Email Templates Do:**
- **Save time** - Write once, use hundreds of times
- **Ensure consistency** - Every client gets the same professional communication
- **Reduce errors** - No more forgetting to include important links or details
- **Personalize automatically** - Templates insert client names, dates, and custom details

**Template Types:**
- **System templates** - ShootPath's built-in emails (quote sent, booking confirmation, etc.)
- **Custom templates** - Your own emails for specific situations
- **Workflow templates** - Automated emails triggered by workflow stages

**Quick Access:**
- Create/edit templates in **Settings > Email Templates**
- Use templates when sending manual emails from jobs or leads
- Configure automated templates in **Settings > Workflows**

**Key Benefits:**
- Respond faster to inquiries (templates ready to go!)
- Never forget to include critical information
- Maintain professional voice across all communications
- Scale your business without spending more time on email

**Articles in This Section:**
- [Creating Templates](./creating-templates) - Build custom email templates from scratch
- [Template Variables](./template-variables) - Reference guide for all available merge fields
- [Default Templates](./default-templates) - ShootPath's built-in templates you can customize
- [Email Best Practices](./email-best-practices) - Writing effective client communication

---

## Detailed Guide

### What Are Email Templates?

Email templates are pre-written messages with placeholders that automatically fill in client-specific details. Think of them as Mad Libs for your business emails - you write the structure once, and the system fills in the blanks for each client.

**Simple example:**

**Your template:**
```
Hi {{client_name}},

Thanks for your inquiry about {{job_type}} photography! I'd love to work with you.

I've prepared a custom quote: {{quote_link}}

Looking forward to hearing from you!
{{your_name}}
```

**What the client receives:**
```
Hi Sarah,

Thanks for your inquiry about Wedding photography! I'd love to work with you.

I've prepared a custom quote: https://app.shootpath.com/portal/abc123/quote

Looking forward to hearing from you!
Emma
```

Every time you send this template, ShootPath automatically replaces `{{client_name}}`, `{{job_type}}`, `{{quote_link}}`, and `{{your_name}}` with the actual details for that specific client and job.

### Why Templates Matter

**Time Savings**

Let's do the math. If you:
- Book 50 clients per year
- Send 10 emails per client (quote, contract, reminders, gallery delivery, etc.)
- Spend 5 minutes writing each email

That's **500 emails × 5 minutes = 2,500 minutes = 41.6 hours per year** spent typing repetitive emails!

With templates, those same emails take 30 seconds to review and send - **250 minutes = 4.2 hours per year**. You just saved 37 hours!

**Consistency**

Every client deserves the same professional experience regardless of whether you're:
- Fresh and energized on Monday morning
- Exhausted after a 10-hour wedding shoot
- Sick with a cold
- Handling 5 inquiries at once

Templates ensure everyone gets your best communication, every time.

**Professionalism**

Templates help you:
- Include all necessary details (never forget to attach the quote link!)
- Maintain appropriate tone and branding
- Avoid typos and grammatical errors
- Present yourself as organized and reliable

Clients notice. They see you respond quickly with clear, professional emails, and it builds trust.

**Peace of Mind**

No more:
- "Did I remember to include the gallery link?"
- "What did I say in that booking confirmation last time?"
- "How do I word this follow-up without being pushy?"

Templates are your safety net. You know what you're sending is complete, correct, and proven to work.

### Template Categories

ShootPath organizes templates into categories based on their purpose.

#### Inquiry & Quote Templates

**Purpose:** Respond to leads and send pricing information

**Examples:**
- Initial inquiry response
- Quote sent notification
- Quote follow-up #1 (3 days after)
- Quote follow-up #2 (7 days after)
- "Sorry to hear we're not a fit" (declined quote)

**These templates help you:**
- Respond quickly to inquiries (speed = bookings!)
- Present pricing professionally
- Follow up systematically without being annoying
- Handle rejections gracefully

#### Booking & Contract Templates

**Purpose:** Convert accepted quotes into confirmed bookings

**Examples:**
- Booking confirmation
- Contract signature request
- Contract signed confirmation
- Deposit invoice sent
- Deposit payment received

**These templates help you:**
- Make clients feel excited and secure about booking
- Get contracts signed quickly
- Ensure payment goes smoothly
- Set expectations for next steps

#### Pre-Session Templates

**Purpose:** Prepare clients before the shoot

**Examples:**
- Questionnaire request
- Session details confirmation
- What to wear guide
- Location details and directions
- Weather backup plan
- Day-before reminder

**These templates help you:**
- Gather important information upfront
- Reduce "where do we meet?" day-of questions
- Help clients prepare properly
- Show up to sessions fully ready

#### Post-Session Templates

**Purpose:** Keep clients informed after the shoot

**Examples:**
- Session thank you
- Editing timeline update
- Gallery ready notification
- Download instructions
- Final payment reminder

**These templates help you:**
- Maintain excitement after the session
- Set realistic delivery expectations
- Reduce "where are my photos?" inquiries
- Close out jobs smoothly

#### Follow-Up & Review Templates

**Purpose:** Maintain relationships and get testimonials

**Examples:**
- Thank you for your business
- Review request
- Referral request
- Print products follow-up
- Anniversary/birthday greeting

**These templates help you:**
- Generate reviews and testimonials
- Get word-of-mouth referrals
- Upsell print products
- Build long-term client relationships

### How Templates Work with Workflows

Templates become even more powerful when combined with workflows. Instead of manually sending each template, workflows trigger them automatically at the right time.

**Example: Quote to Booking Workflow**

**Without automation:**
- Client accepts quote
- You manually send booking confirmation email
- You manually send contract signature request
- You wait, check back later, send reminder if not signed
- Once signed, you manually send deposit invoice
- You wait, check back, send reminder if not paid
- Once paid, you manually send questionnaire
- Repeat for every client... exhausting!

**With automated templates:**
- Client accepts quote
- **Automatic:** Booking confirmation sent
- **Automatic:** Contract signature request sent
- **Automatic:** 3 days later, reminder sent if not signed
- Contract signed (client completes it)
- **Automatic:** Deposit invoice sent immediately
- **Automatic:** 3 days later, reminder sent if not paid
- Deposit paid (client completes it)
- **Automatic:** Questionnaire sent
- You just focused on creative work!

The workflow handles all the communication automatically using your templates. You're notified when action is needed, but otherwise it just works.

[Learn more about workflows →](../workflows/)

### Default vs. Custom Templates

#### Default Templates

ShootPath comes with a library of proven templates for common scenarios. These templates:
- Cover 80% of your communication needs out of the box
- Use photographer-friendly language and tone
- Include all necessary variables and links
- Are based on what works for successful photography businesses

You can use them as-is or customize them to match your brand and voice.

[See all default templates →](./default-templates)

#### Custom Templates

Custom templates let you:
- Create emails for unique situations specific to your business
- Match your personal brand voice and style
- Include information about your specific services or policies
- Handle specialty photography genres (boudoir, newborn, commercial)

**When to create custom templates:**
- You find yourself sending the same email repeatedly
- Default templates don't quite fit your situation
- You want to add unique information about your services
- You're targeting a specific niche with specialized needs

### Template Components

Every email template has several key parts:

#### Template Name

The internal name you see in ShootPath (clients never see this). Use clear, descriptive names:

✅ Good names:
- "Quote Sent - Wedding"
- "Gallery Ready - Portrait Session"
- "Contract Reminder - 3 Days"

❌ Confusing names:
- "Template 1"
- "Email thing"
- "The one I use for stuff"

#### Subject Line

The email subject line clients see in their inbox. Make it:
- **Clear** - They should know what the email is about
- **Personal** - Use variables like their name when appropriate
- **Specific** - Include relevant details like dates or session types

**Examples:**
- "Your {{job_type}} Quote from {{your_business}}"
- "{{client_name}}, Your Gallery is Ready!"
- "Reminder: {{job_type}} Session on {{session_date}}"

#### Email Body

The main content of your message. This includes:
- Greeting (often personalized with `{{client_name}}`)
- Main message explaining the purpose
- Any necessary details or instructions
- Call to action (what they should do next)
- Links to portals, galleries, or other resources
- Your signature

#### Variables/Merge Fields

Placeholders that automatically populate with real data:
- `{{client_name}}` → "Sarah"
- `{{session_date}}` → "October 15, 2024"
- `{{quote_link}}` → actual URL to their quote

[Complete variable reference →](./template-variables)

### Creating Your First Template

Here's a simple template creation walkthrough:

**Scenario:** You want a template for when you send quotes.

**Step 1: Navigate to Templates**
Go to Settings > Email Templates > New Template

**Step 2: Name It**
Internal name: "Quote Sent - General"

**Step 3: Write the Subject**
Subject: "Your {{job_type}} Photography Quote"

**Step 4: Write the Body**
```
Hi {{client_name}},

Thanks so much for reaching out about {{job_type}} photography! I'm excited about the possibility of working with you.

I've put together a custom quote based on what you're looking for:
{{quote_link}}

The quote includes:
- Package options to choose from
- Available add-ons to customize your experience
- Clear pricing with no hidden fees
- Payment schedule details

Feel free to review the quote at your convenience. If you have any questions about packages, pricing, or anything else, just reply to this email!

Looking forward to hearing from you.

Best,
{{your_name}}
{{your_business}}
{{your_phone}}
{{your_website}}
```

**Step 5: Test It**
Use the preview feature to see what it looks like with real client data filled in.

**Step 6: Save and Use**
Save the template, then use it when sending quotes!

[Detailed template creation guide →](./creating-templates)

### Template Best Practices

**Write Like You Talk**

Templates should sound like YOU, not a robot or corporate marketing department.

❌ Stiff: "We are in receipt of your inquiry and have prepared pricing documentation for your perusal."

✅ Natural: "Thanks for reaching out! I've put together a quote for you."

**Keep It Concise**

Clients are busy. Get to the point quickly:
- Lead with the most important information
- Use short paragraphs (2-3 sentences max)
- Break up text with bullet points
- Include clear next steps

**Be Friendly but Professional**

Find the balance between:
- Too casual ("hey sup here's ur quote lol")
- Too formal ("Dear Madam, Please be advised...")

Aim for warm and professional - like talking to a new friend you want to work with.

**Include Clear Calls to Action**

Tell clients exactly what to do next:
- "Review your quote here: [link]"
- "Sign your contract here: [link]"
- "View your gallery here: [link]"

Don't make them guess what you want them to do!

**Test Before Sending**

Always preview templates with real data before using them:
- Do all variables populate correctly?
- Are links working?
- Does the formatting look good?
- Is the tone right?

**Review and Update Regularly**

Every few months:
- Read through your templates fresh
- Update outdated information (pricing, policies, etc.)
- Refine language based on client feedback
- Remove templates you're not using

### Template Variables Explained

Variables are the magic that makes templates powerful. They're placeholders that get replaced with actual data when you send the email.

**Basic syntax:**
Variables use double curly braces: `{{variable_name}}`

**Common categories:**

**Client information:**
- `{{client_name}}` - Client's first name or full name
- `{{client_email}}` - Client's email address
- `{{client_phone}}` - Client's phone number

**Job details:**
- `{{job_type}}` - Wedding, Portrait, Event, etc.
- `{{session_date}}` - When the shoot is scheduled
- `{{session_location}}` - Where you're shooting

**Business information:**
- `{{your_name}}` - Your name
- `{{your_business}}` - Your business name
- `{{your_phone}}` - Your phone number
- `{{your_email}}` - Your business email
- `{{your_website}}` - Your website URL

**Links and URLs:**
- `{{quote_link}}` - Link to online quote
- `{{contract_link}}` - Link to sign contract
- `{{invoice_link}}` - Link to pay invoice
- `{{gallery_link}}` - Link to view gallery
- `{{questionnaire_link}}` - Link to fill out questionnaire

**Pricing information:**
- `{{quote_total}}` - Total quote amount ($2,500)
- `{{deposit_amount}}` - Deposit due ($1,250)
- `{{balance_amount}}` - Remaining balance ($1,250)

[Complete variable reference with examples →](./template-variables)

### Managing Your Template Library

As you create templates, keeping them organized becomes important.

**Organization Tips:**

**Use clear naming conventions:**
- Category - Type - Variation
- Examples: "Quote - Wedding - Follow Up 1", "Booking - Contract Sent", "Post Session - Gallery Ready"

**Create folders/categories:**
- Group templates by workflow stage
- Separate by photography genre if you shoot multiple types
- Keep active templates separate from archived ones

**Archive unused templates:**
- Don't delete templates (you might need them later!)
- Move them to an "Archive" category
- Keep your active template list clean and focused

**Duplicate and modify:**
- Start with a working template
- Duplicate it for variations
- Modify for specific use cases
- Easier than starting from scratch each time

### Common Template Mistakes to Avoid

**Mistake 1: Too Much Information**

Don't overwhelm clients with every detail in one email. Break complex information into multiple emails or link to resources.

❌ "Here's my 10-paragraph explanation of my entire process, equipment, editing style, and philosophy..."

✅ "Here's your quote! I've included everything you need to know. If you want to learn more about how I work, check out my website."

**Mistake 2: Forgetting the Call to Action**

Always tell clients what to do next!

❌ "Your gallery is ready. Have a great day!"

✅ "Your gallery is ready! View and download your photos here: [link]"

**Mistake 3: Using Variables That Don't Exist**

Not all variables work in all contexts. For example, you can't use `{{gallery_link}}` in a quote email because there's no gallery yet!

**Mistake 4: No Personality**

Templates can sound generic if you're not careful. Add personal touches:
- Use your natural voice
- Include phrases you actually say
- Add emoji if that's your style (but use sparingly!)
- Reference your specific services or approach

**Mistake 5: Set It and Forget It**

Templates need maintenance:
- Update pricing information as it changes
- Revise links if your website changes
- Refresh language that feels stale
- Remove outdated policies or references

### Templates for Different Photography Genres

Different types of photography need different communication styles.

#### Wedding Photography

**Tone:** Professional but warm, excited, reassuring

**Key templates:**
- Inquiry response (respond fast in this competitive market!)
- Quote with package options
- Booking confirmation (make them feel special!)
- Timeline coordination
- Day-before reminder
- Post-wedding thank you
- Gallery delivery
- Album design coordination

**Special considerations:**
- Longer booking timeline = more communication touchpoints
- Multiple decision-makers (couple, sometimes parents)
- Higher price points = more detailed information needed

#### Portrait Photography

**Tone:** Friendly, warm, encouraging

**Key templates:**
- Session inquiry response
- Quote with package options
- Booking confirmation
- What to wear guide
- Location details
- Day-before reminder
- Session thank you
- Gallery delivery
- Print products follow-up

**Special considerations:**
- Often booking families, so kid-friendly language
- Wardrobe coordination is important
- Faster turnaround expectations

#### Commercial Photography

**Tone:** Professional, efficient, detail-oriented

**Key templates:**
- Project inquiry response
- Quote/estimate
- Contract and SOW
- Project timeline confirmation
- Shot list confirmation
- Delivery notification
- Invoice for payment
- Follow-up for testimonial

**Special considerations:**
- Usage rights discussion important
- More formal language appropriate
- Net 30/60 payment terms common

#### Newborn Photography

**Tone:** Gentle, reassuring, congratulatory

**Key templates:**
- Congratulations + booking confirmation
- What to expect guide
- Rescheduling flexibility reminder
- Session tips for parents
- Gallery delivery
- Thank you + milestone session offer

**Special considerations:**
- Flexibility needed for birth timing
- Safety information important
- Parent education helpful

### Testing Your Templates

Before you rely on templates for all client communication:

**1. Send Test Emails**
Send templates to yourself or a friend:
- Do variables populate correctly?
- Do links work?
- Does formatting look good on mobile?
- Is the tone right?

**2. Get Feedback**
Ask a trusted friend or family member:
- "Would you understand what to do next?"
- "Does this sound like me?"
- "Is anything confusing or unclear?"

**3. A/B Test Important Templates**
For critical templates like quote emails:
- Create two versions with different approaches
- Use each one for a few weeks
- See which one gets better response rates
- Stick with the winner

**4. Monitor Response Rates**
Track whether clients:
- Open the emails (good subject line?)
- Click links (clear call to action?)
- Respond or take action (effective messaging?)

### Advanced Template Features

Once you're comfortable with basic templates, explore advanced features:

#### Conditional Sections

Show different content based on conditions:

"If deposit is paid, show this text. If deposit is not paid, show reminder instead."

Example:
```
{{#if deposit_paid}}
Thanks for paying your deposit! We're all set.
{{else}}
Reminder: Your deposit of {{deposit_amount}} is due.
{{/if}}
```

#### Dynamic Lists

Automatically list items:

"Include all packages selected"
"List all add-ons chosen"

#### Personalization Beyond Names

Use behavioral data to personalize:
- How many times they've viewed the quote
- Whether they've visited your website
- Past bookings (for returning clients)

[Learn more about advanced features →](./creating-templates#advanced-features)

### What's Next?

Ready to dive deeper into email templates? Explore these articles:

**[Creating Templates](./creating-templates)** - Step-by-step guide to building templates from scratch

**[Template Variables](./template-variables)** - Complete reference of all available merge fields

**[Default Templates](./default-templates)** - Customize ShootPath's built-in templates

**[Email Best Practices](./email-best-practices)** - Writing effective client communication

Or explore related topics:

**[Workflows](../workflows/)** - Automate when templates are sent

**[Leads](../leads/)** - Use templates for inquiry response and follow-up

**[Jobs](../jobs/)** - Use templates throughout the client journey

---

**Questions?** Look for the help links throughout ShootPath, or use the support widget if you need assistance!
