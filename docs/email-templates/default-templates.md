---
sidebar_position: 4
---

# Default Email Templates

## Quick Reference

ShootPath comes with pre-built email templates that cover the most common client communications. These templates are professionally written, tested with real photographers, and ready to use immediately.

**Default Template Categories:**
- **Inquiry & Quote** - Respond to leads and send pricing
- **Booking & Contract** - Confirm bookings and get signatures
- **Pre-Session** - Prepare clients before shoots
- **Post-Session** - Keep clients informed during editing
- **Delivery** - Send galleries and final deliverables
- **Follow-Up** - Request reviews and maintain relationships

**Using Default Templates:**
- Available immediately after account creation
- Can be used as-is or customized
- Automatically triggered by workflows (optional)
- Include all necessary variables and links

**Customization Options:**
- Edit subject lines to match your voice
- Modify body content while keeping structure
- Add your personality and brand tone
- Keep critical variables intact

---

## Detailed Guide

### Why Default Templates Matter

When you first start using ShootPath, you might feel overwhelmed by the idea of creating email templates from scratch. That's where default templates come in - they're your starting point!

**Benefits of default templates:**

**1. Immediate Functionality**
You can start automating client communication on day one without writing a single email.

**2. Professional Quality**
Templates are written by professional copywriters familiar with photography business communication.

**3. Proven Effectiveness**
These templates have been tested with hundreds of photographers and thousands of clients. They work!

**4. Complete Coverage**
Default templates handle every common scenario from first inquiry to post-delivery follow-up.

**5. Easy Customization**
Start with defaults, then tweak to match your brand voice and style.

### How to Access Default Templates

**View all templates:**
1. Go to **Settings > Email Templates**
2. Look for templates marked "Default" or in the "System Templates" section
3. Click any template to preview it

**Customize a default template:**
1. Find the template you want to modify
2. Click **Duplicate** or **Edit**
3. Make your changes
4. Save with a new name (or overwrite if allowed)

**Create your own from scratch:**
1. Click **New Template**
2. Use default templates as reference
3. Build your own version

### Inquiry & Quote Templates

Templates for responding to leads and sending pricing information.

#### Quote Sent

**When to use:** Automatically sent when you send a quote to a lead

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
- Package options to fit your needs and budget
- Available add-ons to customize your experience
- Clear pricing with no hidden fees
- Payment schedule so you know exactly when payments are due

Total investment: {{quote_total}}
Deposit to book: {{deposit_amount}}

Feel free to review the quote at your convenience. If you have
any questions about packages, pricing, or anything else, just
reply to this email!

Looking forward to hearing from you.

Best,
{{your_name}}
{{your_business}}
{{your_phone}}
{{your_website}}
```

**Why it works:**
- Friendly but professional tone
- Clear call to action (view the quote)
- Highlights what's included
- Shows pricing transparency
- Invites questions

**Customization ideas:**
- Add a personal line referencing their specific needs
- Include a link to your portfolio
- Mention your availability for their date
- Add testimonials or recent work

#### Quote Follow-Up (3 Days)

**When to use:** Automatically sent 3 days after quote if no response

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
- Availability for {{session_date}}?

I'm here to help make your decision easier. Just reply to this
email with any questions!

I hope to hear from you soon.

Best,
{{your_name}}
{{your_business}}
{{your_phone}}
```

**Why it works:**
- Not pushy, just helpful
- Lists specific question prompts
- Reminds them of the quote link
- Opens the door for dialogue

**Customization ideas:**
- Mention limited availability for their date
- Add a soft deadline ("Quote pricing valid until...")
- Share a recent testimonial
- Offer a brief call to discuss

#### Quote Follow-Up (7 Days)

**When to use:** Sent 7 days after quote if still no response

**Subject:**
```
Checking in - {{job_type}} on {{session_date}}
```

**Body:**
```
Hi {{client_name}},

I wanted to reach out one more time about your {{job_type}}
photography needs.

View your quote: {{quote_link}}

I know choosing a photographer is a big decision! If there's
anything I can clarify or if you'd like to discuss options,
I'm happy to help.

If you've already booked with another photographer, no worries -
I wish you all the best!

If you're still deciding, I'd love to work with you. Just
reply to this email or give me a call.

Best,
{{your_name}}
{{your_phone}}
```

**Why it works:**
- Final follow-up without being desperate
- Acknowledges they may have moved on
- Still leaves door open
- Professional and respectful

### Booking & Contract Templates

Templates for when a quote is accepted and becomes a booking.

#### Booking Confirmation

**When to use:** Automatically sent when quote is accepted

**Subject:**
```
You're Booked! {{job_type}} on {{session_date}} 🎉
```

**Body:**
```
Hi {{client_name}},

Welcome aboard! I'm so excited to photograph your {{job_type}}.

Your session details:
📅 Date: {{session_date}}
🕐 Time: {{session_time}}
📍 Location: {{session_location}}

Next steps to finalize your booking:
1. Sign your contract: {{contract_link}}
2. Pay your deposit: {{invoice_link}} ({{deposit_amount}})
3. Fill out your questionnaire: {{questionnaire_link}}

Once your deposit is received, you're officially booked and
your date is secured on my calendar!

I'll send more details about what to expect, how to prepare,
and timeline as we get closer to your session date.

So excited to work with you!

Best,
{{your_name}}
{{your_business}}
{{your_phone}}
```

**Why it works:**
- Celebrates the booking
- Clear next steps
- All important links included
- Sets expectations for what's next

**Customization ideas:**
- Add welcome gift or surprise
- Include preparation guide link
- Share your excitement about their specific session
- Mention if you have any pre-session meetings

#### Contract Signature Request

**When to use:** Sent when contract is ready to sign

**Subject:**
```
Please Sign Your {{job_type}} Contract
```

**Body:**
```
Hi {{client_name}},

To finalize your booking, please sign your photography contract:
{{contract_link}}

The contract outlines:
- What's included in your package
- Payment schedule and due dates
- Session details and timeline
- Cancellation and rescheduling policies
- Copyright and usage rights

Signing is quick and easy - just click the link above, review
the contract, and add your signature electronically.

Once signed, you'll receive a copy for your records.

Questions about anything in the contract? Just reply to this email!

Best,
{{your_name}}
{{your_business}}
```

**Why it works:**
- Clear call to action
- Explains what's in the contract
- Reassures that signing is easy
- Invites questions

#### Contract Signed Confirmation

**When to use:** Automatically sent when client signs contract

**Subject:**
```
Contract Signed - You're All Set! ✓
```

**Body:**
```
Hi {{client_name}},

Great news - your contract is signed!

A copy has been emailed to you for your records. You can also
access it anytime in your client portal: {{portal_link}}

Next step:
Pay your deposit of {{deposit_amount}}: {{invoice_link}}

Once your deposit is received, you're officially locked in
and your date is secured on my calendar!

Looking forward to your {{job_type}} on {{session_date}}.

Best,
{{your_name}}
```

**Why it works:**
- Confirms completion of contract step
- Moves them to next action (deposit)
- Provides reassurance

### Pre-Session Templates

Templates to prepare clients before the photography session.

#### Questionnaire Request

**When to use:** Sent after booking is confirmed

**Subject:**
```
Quick Questionnaire for Your {{job_type}} Session
```

**Body:**
```
Hi {{client_name}},

To help me prepare for your {{job_type}} session, please
fill out this quick questionnaire:

{{questionnaire_link}}

It takes about 5-10 minutes and helps me understand:
- Your vision and style preferences
- Any special requests or must-have shots
- Important details about your session
- Any concerns or questions you have

The more I know about what you're looking for, the better
I can tailor your session to your needs!

Thanks!
{{your_name}}
```

**Why it works:**
- Explains the "why" (better preparation)
- Sets time expectations (5-10 minutes)
- Lists what information you're gathering
- Makes it easy with direct link

#### Session Reminder (1 Week Before)

**When to use:** Automatically sent 7 days before session

**Subject:**
```
Your {{job_type}} Session is Next Week!
```

**Body:**
```
Hi {{client_name}},

Getting excited! Your {{job_type}} session is coming up:

📅 {{session_date}}
🕐 {{session_time}}
📍 {{session_location}}

Quick reminders:
- Wear comfortable clothes you feel confident in
- Bring any props or items you'd like to include
- Eat beforehand so you have energy
- Arrive a few minutes early so we're not rushed
- Check the weather and dress accordingly

What to expect:
We'll spend about {{session_duration}} together. I'll guide
you through everything - no modeling experience needed!
Just relax and have fun.

Weather backup plan:
If weather looks bad, I'll reach out 24-48 hours before to
discuss rescheduling if needed.

Questions or concerns? Reply to this email or call/text:
{{your_phone}}

Can't wait!
{{your_name}}
```

**Why it works:**
- Builds excitement
- Provides helpful reminders
- Reduces client anxiety
- Covers logistics

**Customization ideas:**
- Add wardrobe guide link
- Include Pinterest board of inspiration
- Suggest specific outfit colors for your shooting location
- Add parking/directions details

#### Session Reminder (Day Before)

**When to use:** Sent the day before the session

**Subject:**
```
Tomorrow! {{job_type}} at {{session_time}}
```

**Body:**
```
Hi {{client_name}},

Quick reminder that your session is tomorrow!

📅 {{session_date}} (tomorrow!)
🕐 {{session_time}}
📍 {{session_location}}

Weather looks good - we're all set! ☀️

See you tomorrow!
{{your_name}}
{{your_phone}}
```

**Why it works:**
- Short and simple
- Confirms all details
- Mentions weather
- Easy to reference

### Post-Session Templates

Templates for after the photography session.

#### Session Thank You

**When to use:** Sent day after the session

**Subject:**
```
Thank You - {{job_type}} Session
```

**Body:**
```
Hi {{client_name}},

Thank you so much for yesterday's session! I had a wonderful
time photographing you.

I'm excited to get started on editing your photos. Based on
my current workload, your gallery will be ready in approximately
{{turnaround_time}}.

I'll send you an email as soon as your gallery is uploaded
and ready to view.

In the meantime, if you have any questions, feel free to reach out!

Thanks again!
{{your_name}}
```

**Why it works:**
- Shows appreciation
- Sets delivery expectations
- Maintains excitement
- Keeps communication flowing

#### Editing Update (Halfway)

**When to use:** Optional mid-editing check-in

**Subject:**
```
Update: Editing Your {{job_type}} Photos
```

**Body:**
```
Hi {{client_name}},

Quick update - I'm about halfway through editing your photos
and they're looking amazing!

Your gallery should be ready by {{estimated_delivery_date}}.
I'll send you an email the moment it's ready to view.

I know the wait can feel long, but I promise it'll be worth it!

Talk soon,
{{your_name}}
```

**Why it works:**
- Proactive communication reduces "where are my photos?" inquiries
- Maintains excitement
- Reinforces quality over speed

### Delivery Templates

Templates for delivering final photos.

#### Gallery Ready

**When to use:** Sent when gallery is uploaded and ready

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

Your gallery includes {{photo_count}} edited high-resolution photos
available for viewing, downloading, and sharing.

How to download:
1. Click the gallery link above
2. Browse your photos
3. Click "Download" on individual photos or "Download All"

Gallery access:
Your gallery will be available until {{gallery_expiration_date}}.
Please download your favorites before this date!

Print ordering:
Professional prints, canvases, and albums are available to order
directly through the gallery if you're interested!

Thank you for trusting me to capture these memories for you.
It was truly a pleasure!

Enjoy!

{{your_name}}
{{your_business}}
{{your_phone}}
```

**Why it works:**
- Exciting announcement
- Clear instructions for downloading
- Sets expiration expectations
- Mentions print products (upsell opportunity)
- Ends with gratitude

**Customization ideas:**
- Add social media sharing encouragement
- Include discount code for prints
- Request permission to share favorites on your portfolio
- Mention referral incentives

#### Gallery Expiration Reminder

**When to use:** Sent 7 days before gallery expires

**Subject:**
```
Reminder: Gallery Expires in 7 Days
```

**Body:**
```
Hi {{client_name}},

Just a friendly reminder that your gallery access expires
on {{gallery_expiration_date}} (one week from today).

View and download your photos:
{{gallery_link}}

Make sure to download your favorites before the gallery expires!

If you need more time or want to extend your gallery access,
just let me know.

Best,
{{your_name}}
```

**Why it works:**
- Gives them time to act
- Clear deadline
- Offers extension option

### Payment Templates

Templates related to invoices and payments.

#### Deposit Invoice

**When to use:** Sent with booking confirmation

**Subject:**
```
Deposit Invoice - {{job_type}}
```

**Body:**
```
Hi {{client_name}},

Your deposit invoice is ready!

Amount due: {{deposit_amount}}
Due date: {{deposit_due_date}}

Pay your invoice: {{invoice_link}}

Once your deposit is received, your date is officially secured
on my calendar!

Payment methods accepted:
- Credit/debit card (through the invoice link)
- Bank transfer (details in invoice)
- Check (mail to address in invoice)

Questions about payment? Just reply to this email.

Thank you!
{{your_name}}
{{your_business}}
```

**Why it works:**
- Clear amount and due date
- Direct payment link
- Lists payment options
- Professional and straightforward

#### Deposit Paid Confirmation

**When to use:** Automatically sent when deposit is received

**Subject:**
```
Deposit Received - You're Officially Booked! ✓
```

**Body:**
```
Hi {{client_name}},

Thank you for your payment! Your deposit of {{deposit_amount}}
has been received.

✅ You're officially booked for {{session_date}}!

Your date is now secured on my calendar. I'm so excited to
photograph your {{job_type}}!

Remaining balance: {{balance_amount}}
Due date: {{final_due_date}}

I'll send a reminder closer to the due date. In the meantime,
I'll be in touch with more details about preparing for your session.

Thanks again!
{{your_name}}
```

**Why it works:**
- Confirms payment immediately
- Reinforces the booking
- Shows remaining balance
- Maintains excitement

#### Final Payment Reminder

**When to use:** Sent when final payment is due

**Subject:**
```
Final Payment Due - {{job_type}}
```

**Body:**
```
Hi {{client_name}},

Your final payment is due for your upcoming {{job_type}} session!

Amount due: {{balance_amount}}
Due date: {{final_due_date}}

Pay your invoice: {{invoice_link}}

Session details:
📅 {{session_date}}
🕐 {{session_time}}
📍 {{session_location}}

Looking forward to your session!

{{your_name}}
{{your_phone}}
```

**Why it works:**
- Clear reminder without being pushy
- Shows amount and due date
- Includes session details as reminder
- Easy payment link

### Follow-Up Templates

Templates for maintaining relationships and getting reviews.

#### Review Request

**When to use:** Sent 1-2 weeks after gallery delivery

**Subject:**
```
Would Love Your Feedback! ⭐
```

**Body:**
```
Hi {{client_name}},

I hope you're loving your photos!

If you have a moment, I'd be so grateful if you could leave
a quick review about your experience:

[Leave a Review - Google]
[Leave a Review - Facebook]

Your feedback helps other couples/families find me and helps
me continue to improve my services.

Thank you so much for your business - it was truly a pleasure
working with you!

Best,
{{your_name}}
```

**Why it works:**
- Asks politely, not demandingly
- Makes it easy with direct links
- Explains why reviews matter
- Shows gratitude

**Customization ideas:**
- Offer small incentive (discount on future session)
- Share that you're a small business and reviews really help
- Time it after they've had time to enjoy photos

#### Referral Request

**When to use:** Sent after successful project completion

**Subject:**
```
Know Anyone Looking for a Photographer?
```

**Body:**
```
Hi {{client_name}},

I'm so glad you're happy with your photos!

If you know anyone looking for a photographer, I'd love if
you'd pass my name along:

{{your_website}}
{{your_phone}}

As a thank you, if your referral books a session, I'll give
you a $50 credit toward prints or your next session!

Thanks for being such an amazing client.

Best,
{{your_name}}
```

**Why it works:**
- Asks after positive experience
- Offers incentive
- Makes it easy to share your info
- Expresses gratitude

#### Print Products Follow-Up

**When to use:** Sent 2-3 weeks after gallery delivery

**Subject:**
```
Have You Considered Prints? 🖼️
```

**Body:**
```
Hi {{client_name}},

I wanted to follow up - have you thought about ordering prints
or products from your gallery?

Your photos look amazing displayed in your home! I offer:
- Professional prints (any size)
- Canvas prints
- Photo albums
- Metal prints
- Frames

View your gallery and order prints:
{{gallery_link}}

Special offer: Use code PRINTS15 for 15% off any print order
this week!

Let me know if you have questions about products or sizing.

Best,
{{your_name}}
```

**Why it works:**
- Creates upsell opportunity
- Provides incentive with discount
- Shows what products are available
- Easy ordering through gallery

### Customizing Default Templates

Default templates are a starting point. Here's how to make them yours:

#### Keep the Structure, Change the Voice

**Default tone:**
```
Hi {{client_name}},

Thanks for your inquiry about {{job_type}} photography!
```

**More casual:**
```
Hey {{client_name}},

So excited you reached out about {{job_type}} photography!
```

**More formal:**
```
Dear {{client_name}},

Thank you for your interest in my {{job_type}} photography services.
```

#### Add Personal Touches

**Generic:**
```
Looking forward to working with you!
```

**Personal:**
```
I'm especially excited because fall weddings at [your favorite venue]
are absolutely magical!
```

#### Include Your Unique Policies

Add sections about:
- Your specific process
- Your editing style
- Your gear or approach
- Unique services you offer

#### Adjust Timing

Default templates suggest timing (3-day follow-up, 7-day follow-up). Adjust to match your style:
- More aggressive: 2-day, 5-day follow-ups
- More relaxed: 5-day, 10-day follow-ups

### What NOT to Change

When customizing default templates, keep these elements:

**Critical variables:**
- `{{quote_link}}`, `{{contract_link}}`, etc. - Clients need these!
- `{{client_name}}` - Personalization is important
- Pricing variables - Accuracy matters

**Clear calls to action:**
- "View your quote here: [link]"
- "Sign your contract: [link]"
Don't make it harder for clients to take action!

**Important information:**
- Payment due dates
- Gallery expiration notices
- Session details

### Testing Your Customized Templates

After customizing:

1. **Send test to yourself**
   - Check formatting
   - Verify variables populate
   - Click all links

2. **Read it fresh**
   - Does it sound like you?
   - Is anything confusing?
   - Are you proud to send it?

3. **Get feedback**
   - Ask a friend to read it
   - "Would you understand what to do next?"

4. **Monitor results**
   - Are clients responding?
   - Are they completing actions?
   - Do you get questions that indicate confusion?

### What's Next?

**Want to create your own templates?** → [Creating Templates](./creating-templates)

**Need variable reference?** → [Template Variables](./template-variables)

**Want email writing tips?** → [Email Best Practices](./email-best-practices)

**Ready to automate templates with workflows?** → [Workflows](../workflows/)

---

**Questions?** Look for the help links in ShootPath, or use the support widget for assistance!
