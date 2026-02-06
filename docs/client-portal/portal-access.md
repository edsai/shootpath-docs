---
sidebar_position: 2
---

# Portal Access and Security

## Quick Reference

The Client Portal uses magic links for secure, passwordless access. Clients receive unique links via email and can access their portal pages instantly - no account creation required.

**How Portal Access Works:**
- Each job gets a unique portal token (random string)
- Token is included in all portal links for that job
- Links are sent via email when you send quotes, contracts, invoices, or galleries
- Clients click the link and immediately see their content
- No username or password needed

**Security Features:**
- Portal tokens are cryptographically random and impossible to guess
- Each token is unique per job (no reuse)
- Links use HTTPS encryption
- Only the client with the exact link can access that portal page
- Tokens don't expire

**Resending Links:**
If a client loses the email, you can resend any portal link from the job details page. Just click "Resend Quote Email" or "Resend Contract Email" and they'll get a fresh copy of the link.

**Next Steps:** Learn about [quote acceptance](./quote-acceptance) or [contract signing](./contract-signing).

---

## Detailed Guide

### What Are Portal Tokens?

A portal token is a unique identifier for each job's client portal. Think of it like a secure key - only someone with the key can unlock that specific portal page.

**Example portal link:**
```
https://yourshootpath.com/portal/k8p2m9n4x7q5/quote
```

In this URL:
- `yourshootpath.com` - Your ShootPath instance
- `/portal/` - Indicates this is a portal page
- `k8p2m9n4x7q5` - The unique portal token for this job
- `/quote` - The specific content they're viewing

**What makes tokens secure:**
- **Randomly generated** - Tokens use cryptographically secure random generation, making them impossible to predict
- **Long enough** - Tokens are 12+ characters, giving billions of possible combinations
- **Unique per job** - No two jobs share the same token
- **No pattern** - Tokens don't reveal anything about the client, date, or booking
- **Can't be brute-forced** - Even trying millions of combinations wouldn't find valid tokens

:::tip Security Note
Portal tokens provide the same level of security as password-reset links or one-time login links used by banks and other secure services. They're a proven, secure authentication method!
:::

### How Clients Receive Portal Links

When you take certain actions in ShootPath, the system automatically emails your client with a portal link:

#### Sending a Quote
**You do:** Click "Send Quote" on a lead
**Client receives:** Email with subject "Your Quote from \{Business Name\}"
**Email contains:**
- Brief message about the quote
- "View Quote" button with portal link
- Your contact information

**Portal link goes to:** `/portal/\{token\}/quote`

#### Quote Acceptance (Auto-Generated Contract)
**Happens when:** Client accepts your quote
**Client receives:** Email with subject "Your Contract is Ready to Sign"
**Email contains:**
- Notification that their quote was accepted
- "Review and Sign Contract" button with portal link
- Reminder that contract must be signed before payment

**Portal link goes to:** `/portal/\{token\}/contract`

#### Sending an Invoice
**You do:** Create invoice or payment schedule triggers a payment due
**Client receives:** Email with subject "Invoice from \{Business Name\}"
**Email contains:**
- Invoice details and amount due
- "View and Pay Invoice" button with portal link
- Due date if applicable

**Portal link goes to:** `/portal/\{token\}/invoice`

#### Delivering a Gallery
**You do:** Upload photos and mark gallery as ready
**Client receives:** Email with subject "Your Gallery is Ready!"
**Email contains:**
- Excited message that their photos are available
- "View Gallery" button with portal link
- Brief instructions on downloading or favoriting

**Portal link goes to:** `/portal/\{token\}/gallery`

#### Sending a Questionnaire
**You do:** Assign a questionnaire to a job
**Client receives:** Email with subject "We need some information for your \{Job Type\}"
**Email contains:**
- Context about why you need this information
- "Fill Out Questionnaire" button with portal link
- Estimated time to complete

**Portal link goes to:** `/portal/\{token\}/questionnaire/\{id\}`

### The Client Experience

Let's walk through exactly what your client experiences when accessing the portal:

#### Step 1: Receiving the Email

Your client opens their email inbox and sees a message from your business. The email is:
- **Professional** - Clean design, your branding
- **Clear** - Subject line states exactly what it is ("Your Quote from Sarah Photography")
- **Actionable** - Large button or link makes next step obvious

The email might look like this:
```
Subject: Your Quote from Sarah Photography

Hi Luna!

Your quote for your October wedding is ready! I've put together pricing
based on our conversation about full-day coverage and an engagement session.

[View Your Quote]  ← Big blue button

The quote includes package details, pricing, and our payment schedule.
Let me know if you have any questions!

Looking forward to working with you!
Sarah
```

#### Step 2: Clicking the Link

When they click "View Your Quote," their default browser opens and loads the portal page. This happens instantly - no loading screens, no "create an account" prompts, no passwords.

**What loads:**
- Your business logo at the top
- Client name and job details
- The specific content (quote, contract, invoice, etc.)
- Clear instructions on what to do next

**On mobile:** The page adapts perfectly to phone screens, with touch-friendly buttons and readable text sizes.

**On desktop:** The page uses the full screen to show content clearly and professionally.

#### Step 3: Interacting with Content

Depending on what page they're on, they can:
- Read package details and pricing
- Sign contracts digitally
- Submit payments
- Answer questionnaire questions
- Browse photo galleries

Everything is intuitive. There's no learning curve - if your client can use Facebook, they can use the portal!

#### Step 4: Completing Actions

When they take an action (accept a quote, sign a contract, submit payment):
- **Instant feedback** - Confirmation message appears immediately
- **You're notified** - ShootPath sends you a notification
- **Next steps shown** - The portal tells them what happens next

**Example after accepting a quote:**
```
✓ Quote Accepted!

Thanks for choosing Sarah Photography! You'll receive an email shortly
with your contract to review and sign.

We'll be in touch soon with more details about your session.
```

Clear, friendly, and reassuring - just like you'd communicate in person!

### Portal Link Lifetime

**Portal links don't expire.** Here's what that means:

#### During the Booking Process
Your client can click the quote link multiple times if they want to review it again before deciding. They can share the link with their partner or family member to get input. The link keeps working!

#### After Signing and Payment
Even after the booking is complete, the portal link remains active. Clients can:
- Access their signed contract months later
- View their invoice and payment history
- Download their gallery photos anytime

**Why no expiration?** Because your clients might need to access documents or photos long after the job is done. Maybe they need their signed contract for insurance, or they want to download gallery photos to a new computer. The portal stays accessible as long as the job exists in ShootPath.

:::warning Important
While links don't expire, if you delete a job in ShootPath, the portal link will stop working. Keep completed jobs in your system if clients might need ongoing access!
:::

### Multiple Portal Pages

Each job has several different portal URLs, all using the same token:

- `/portal/\{token\}/job` - Overview of the job status
- `/portal/\{token\}/quote` - Quote details and acceptance
- `/portal/\{token\}/contract` - Contract review and signing
- `/portal/\{token\}/invoice` - Invoice and payment
- `/portal/\{token\}/gallery` - Photo gallery
- `/portal/\{token\}/questionnaire/\{id\}` - Specific questionnaire

**Same token, different pages!** The token proves they're the right client, and the path determines what content they see.

**Navigation between pages:** Some portal pages have links to related content. For example, after paying an invoice, there might be a "View Gallery" link (if the gallery is ready). This helps clients navigate without needing separate emails for everything.

### Resending Portal Links

Life happens - clients lose emails, change email addresses, or accidentally delete messages. Here's how to resend portal links:

#### Resending via Admin Dashboard

1. Open the job in your admin dashboard
2. Look for the relevant section (Quote, Contract, Invoice, Gallery)
3. Click the "Resend Email" button or "Send Again" option
4. Confirm the client's email address is correct
5. Click send

The client receives a fresh email with the portal link!

**What gets resent:**
- The exact same portal link (same token)
- Updated email template (in case you've changed your templates)
- Current status of the content (if you've updated the quote or invoice)

#### Changing the Email Address

If the client changed their email address:

1. Update their email in the Client record
2. Resend the portal email
3. New email address receives the link

**The token doesn't change** - you're just sending the same link to a new address.

### Security Considerations

While portal tokens are very secure, here are some best practices:

#### Always Verify Email Addresses

Before sending any portal link, double-check the email address is correct. Typos mean the link goes to the wrong person!

**Check for:**
- Transposed letters (sarah@gmial.com vs sarah@gmail.com)
- Extra spaces (before or after the email)
- Wrong domain (work email vs personal email)

#### Educate Clients About Link Security

While you don't need to scare clients, you can mention:
- "Keep this link private - it's your personal access to your booking"
- "If you share it with your partner to review together, that's fine!"
- "Don't post the link publicly on social media"

Most clients already understand this intuitively (they don't share their Amazon order links publicly), but a gentle reminder doesn't hurt.

#### Use HTTPS

ShootPath enforces HTTPS on all portal pages, so data is encrypted in transit. You don't need to do anything - this is automatic!

**What HTTPS protects:**
- Payment card details during checkout
- Personal information in contracts and forms
- Gallery photos and downloads
- Any communication between client browser and server

#### Monitor Portal Access

While you can't see real-time "who's viewing what," you can track important actions:
- Quote accepted (timestamp recorded)
- Contract signed (timestamp + IP address logged)
- Payment submitted (timestamp + transaction details)

This audit trail helps if there's ever a dispute about whether a client agreed to terms or made a payment.

### Troubleshooting Portal Access Issues

Sometimes clients report they can't access the portal. Here's how to troubleshoot:

#### "The link doesn't work"

**Most common cause:** Email client mangled the URL

**Solution:** Copy the full link and paste it directly into a browser address bar, or resend the email

#### "I get a blank page"

**Most common cause:** Browser extension blocking content, or very old browser

**Solution:** Try a different browser (Chrome, Safari, Firefox) or disable ad blockers

#### "It says the page doesn't exist"

**Most common cause:** Job was deleted or token was mistyped

**Solution:** Verify the job still exists in your admin dashboard, then resend the portal link

#### "The payment form won't load"

**Most common cause:** Stripe integration not configured or browser blocking third-party scripts

**Solution:** Verify your Stripe integration is active in Settings, or ask client to try a different browser

#### "I already paid, why does it ask me to pay again?"

**Most common cause:** Client bookmarked the invoice page instead of the job page

**Solution:** Send them a fresh portal link to the job overview page, which shows payment status accurately

### Privacy and Data Protection

The portal respects client privacy in several ways:

#### No Tracking or Analytics

ShootPath doesn't track client behavior in the portal beyond critical actions (quote acceptance, contract signing, payment). There's no creepy "Sarah viewed your quote 37 times" data.

**What IS tracked:**
- Quote accepted (yes or no, timestamp)
- Contract signed (yes or no, timestamp, signature)
- Payment submitted (yes or no, timestamp, amount, transaction ID)

**What is NOT tracked:**
- How long they spent reading the quote
- How many times they viewed the page
- What device or browser they used (except for security logging on contract signing)

#### No Sharing of Information

Portal pages don't leak information to third parties. There are no:
- Social media pixels
- Advertising trackers
- Analytics scripts (except essential error monitoring)

Your client's data stays between you and them.

#### Compliance with Data Protection Laws

ShootPath's portal token system complies with GDPR, CCPA, and other data protection regulations:
- No unnecessary data collection
- Clients can request their data be deleted
- Data is encrypted in transit and at rest
- Access controls prevent unauthorized viewing

### Tips for a Smooth Portal Experience

**Test your own portal** - Create a test job and send yourself quotes, contracts, and invoices. Experience exactly what your clients see!

**Use clear email subjects** - Make sure email subjects clearly state what the email contains ("Your Quote from Sarah Photography" not "ShootPath Notification")

**Include personal messages** - When sending portal links, add a personal note in the email template. "Hi Luna! Here's the pricing we discussed..." is much warmer than a generic template.

**Keep content updated** - If you change packages or pricing, make sure portal content reflects those changes before sending to clients.

**Mobile-test important pages** - Open portal pages on your phone to verify they look good on mobile. Most clients will view on mobile first!

### What's Next?

Now that you understand how portal access works, explore what clients do in the portal:

**Quote Acceptance** - [Learn what clients see when reviewing and accepting quotes](./quote-acceptance)

**Contract Signing** - [Understand the digital signing process](./contract-signing)

**Payments** - [See how clients pay invoices via Stripe](./payments)

**Questionnaires** - [Learn about the questionnaire experience](./questionnaires)

---

**Questions?** Look for the help links throughout ShootPath, or reach out to support if you need a hand!
