---
sidebar_position: 3
---

# Email and SMTP Integration

## Quick Reference

Email integration allows ShootPath to send emails from YOUR email address - quotes, booking confirmations, gallery notifications, and more. Clients see emails coming from you, not a generic "noreply@shootpath.com" address.

**Two Integration Options:**
- **Gmail** - Quick OAuth connection, free, works for most photographers
- **SMTP** - Use any email provider (custom domain, higher limits)

**Why Connect Email:**
- Send automated emails to clients
- All emails appear from YOUR address
- Professional appearance
- No manual copy/paste

**Setup Time:**
- Gmail: 2-3 minutes
- SMTP: 5-10 minutes

**Sending Limits:**
- Gmail (free): 500 emails/day
- Gmail (Google Workspace): 2,000 emails/day
- SMTP: Varies by provider (usually 1,000-10,000/day)

**Quick Setup:**
Go to **Settings > Integrations > Email** and choose Gmail or SMTP. Follow the prompts to authorize or enter credentials.

**Next Steps:**
- [Connect Gmail](#connecting-gmail) (easiest option)
- [Set up SMTP](#setting-up-custom-smtp) (for custom domains)
- [Troubleshoot email delivery](#troubleshooting-email-issues)

---

## Detailed Guide

### What is Email Integration?

Email integration connects ShootPath to your email account so it can send messages on your behalf. Instead of you manually copying client details into Gmail and typing emails, ShootPath handles it automatically using your email templates.

**Without email integration:**
- You create a quote in ShootPath
- You copy client's email address
- You open Gmail
- You type email manually
- You include quote link manually
- You send
- You go back to ShootPath to mark "quote sent"
- Repeat for every client... exhausting!

**With email integration:**
- You create a quote in ShootPath
- You click "Send Quote"
- **Automatic:** Email composed from template
- **Automatic:** Sent from your Gmail/SMTP account
- **Automatic:** Marked as sent in ShootPath
- **Automatic:** Activity logged
- You just focused on the next task!

### Gmail vs. SMTP: Which to Choose?

#### Choose Gmail If:

**You use Gmail for your business email:**
- yourname@gmail.com
- yourname@yourdomain.com (via Google Workspace)

**You want the easiest setup:**
- 3-click OAuth connection
- No technical knowledge required
- Works immediately

**You send moderate email volume:**
- Up to 500 emails/day (free Gmail)
- Up to 2,000 emails/day (Google Workspace)
- Sufficient for most photography businesses

**You want reliability:**
- Gmail has excellent deliverability
- Rarely ends up in spam
- Trusted by clients

#### Choose SMTP If:

**You use a custom email provider:**
- yourname@yourstudio.com (via your web hosting)
- yourname@yourname.com (custom domain)
- Any non-Gmail email service

**You need higher sending limits:**
- Your host allows 5,000+ emails/day
- You run frequent mini session promotions
- You have large mailing lists

**You want full control:**
- Your own mail server
- Custom security policies
- Advanced email routing

**You're technical savvy:**
- Comfortable finding SMTP settings
- Know what server, port, and TLS mean
- Can troubleshoot connection issues

### Connecting Gmail

Gmail integration uses OAuth, meaning you don't enter your password in ShootPath - you authorize the connection directly with Google.

#### Step 1: Navigate to Integration Settings

Go to **Settings > Integrations > Email**

#### Step 2: Choose Gmail

Click the "Connect Gmail" button

#### Step 3: Choose Google Account

A Google login window opens. Select the Gmail account you want to use for sending emails.

**If you have multiple Google accounts:**
- Choose your primary business account
- The one clients recognize
- Example: emma@crashingelegance.com (not personal.email123@gmail.com)

#### Step 4: Grant Permissions

Google asks: "ShootPath wants to access your Google Account"

**Permissions requested:**
- Send emails on your behalf
- View email settings (to verify sending limits)

**Important:** ShootPath CANNOT read your existing emails. It can only SEND new ones.

Click "Allow"

#### Step 5: Connection Complete

You're redirected back to ShootPath. You'll see:
```
Gmail Connected ✓
Connected as: emma@crashingelegance.com
Last email sent: Never (newly connected)
```

#### Step 6: Send Test Email

**Always test before sending to real clients!**

1. Create a test lead with YOUR email as the client email
2. Create a test quote
3. Click "Send Quote"
4. Check your inbox - did you receive it?
5. Does it look professional?
6. Does the "From" address show your email?

**If test succeeds:** You're ready to go!

**If test fails:** See [troubleshooting section](#troubleshooting-email-issues)

#### Gmail Sending Limits

**Free Gmail accounts:**
- 500 emails per day
- Resets at midnight Pacific Time
- If exceeded: "You have reached a limit for sending email" error

**Google Workspace (paid):**
- 2,000 emails per day
- Same reset time
- More reliable for business use

**How to avoid hitting limits:**
- Most photographers never hit 500/day
- Mini session announcements to 300 clients = fine
- If you send newsletters, use Mailchimp instead
- ShootPath only sends transactional emails (quotes, invoices, galleries)

**What happens if you hit the limit:**
- ShootPath shows error: "Daily sending limit reached"
- Emails queue until tomorrow
- You receive notification
- Next day: queued emails send automatically

### Setting Up Custom SMTP

SMTP (Simple Mail Transfer Protocol) is the standard way email servers communicate. By providing SMTP credentials, ShootPath can send emails through any email provider.

#### Before You Start: Find Your SMTP Settings

**You'll need 4 pieces of information:**
1. **SMTP Server** (e.g., mail.yourhost.com or smtp.gmail.com)
2. **Port** (usually 587 or 465)
3. **Username** (usually your full email address)
4. **Password** (your email password or app-specific password)

**Where to find these:**

**Common hosting providers:**
- **Bluehost:** Help > Email > "Email Client Setup" page
- **SiteGround:** Control Panel > Email > "Email Accounts" > "Configure Email Client"
- **HostGator:** cPanel > Email Accounts > "Configure Email Client"
- **GoDaddy:** Email & Office > My Email > Settings icon

**Gmail SMTP:**
- Server: smtp.gmail.com
- Port: 587
- Username: your full Gmail address
- Password: App-specific password (see below)

**Office 365 / Outlook:**
- Server: smtp.office365.com
- Port: 587
- Username: your full email address
- Password: your Office 365 password

**Pro tip:** Most hosting providers have a knowledge base article titled "SMTP Settings" or "Email Client Configuration"

#### Setting Up SMTP in ShootPath

**Step 1: Navigate to Integration Settings**

Go to **Settings > Integrations > Email**

**Step 2: Choose SMTP**

Click "Configure SMTP"

**Step 3: Enter Server Settings**

Fill in the form:

**SMTP Server:**
```
mail.yourdomain.com
```

**Port:**
```
587
```
(Most common. Some providers use 465 or 25)

**Encryption:**
- Select "TLS" (most common) or "SSL"
- If unsure, try TLS first

**Step 4: Enter Credentials**

**Username:**
```
yourname@yourdomain.com
```
(Usually your full email address)

**Password:**
```
your-email-password
```

**From Name:**
```
Your Business Name
```
(What clients see as sender name)

**From Address:**
```
yourname@yourdomain.com
```
(Must match the account you're authenticating with)

**Step 5: Test Connection**

Click "Test SMTP Connection"

ShootPath sends a test email to your account email address.

**Success:**
```
✅ SMTP connection successful!
Test email sent to yourname@yourdomain.com
```

**Failure:**
```
❌ SMTP connection failed
Error: Authentication failed (535)
```

If failed, see [troubleshooting section](#troubleshooting-email-issues)

**Step 6: Save Settings**

Once test succeeds, click "Save SMTP Settings"

**Step 7: Send Real Test**

Just like with Gmail:
1. Create test lead with YOUR email
2. Send test quote
3. Verify you receive it
4. Check it looks professional

#### Using Gmail with SMTP (Alternative to OAuth)

You can use Gmail via SMTP instead of OAuth. Why would you?

**Reasons to use Gmail SMTP:**
- You want more control over settings
- OAuth connection keeps expiring
- You're using a Google Workspace account with specific policies

**How to set it up:**

**Important:** You must create an "App Password" - Gmail doesn't allow regular passwords via SMTP.

**Creating Gmail App Password:**

1. Go to myaccount.google.com
2. Click "Security"
3. Enable "2-Step Verification" (required for app passwords)
4. Go to "App passwords"
5. Select "Mail" and "Other (Custom name)"
6. Name it "ShootPath"
7. Google generates 16-character password (example: abcd efgh ijkl mnop)
8. Copy this password

**SMTP Settings for Gmail:**
- Server: smtp.gmail.com
- Port: 587
- Encryption: TLS
- Username: your-email@gmail.com
- Password: [paste the 16-character app password]

### Email Sending Best Practices

#### Write Clear Subject Lines

Your email templates include subject lines. Make them:

**Specific:**
✅ "Your Wedding Photography Quote from Emma"
❌ "Quote"

**Personal:**
✅ "Sarah, Your Gallery is Ready!"
❌ "Gallery Ready"

**Action-oriented:**
✅ "Action Required: Sign Your Contract"
❌ "Contract"

#### Include Clear Calls to Action

Every email should tell the client what to do next:

✅ "View your quote here: [link]"
✅ "Pay your invoice here: [link]"
✅ "Download your photos here: [link]"

Don't make clients guess!

#### Test Emails on Mobile

60%+ of clients read emails on phones. Before going live:

1. Send test emails to yourself
2. Open on your phone
3. Check:
   - Does it load quickly?
   - Is text readable (not too small)?
   - Are buttons tappable?
   - Do links work?

#### Monitor Delivery Rates

**In ShootPath, check email logs:**
Settings > Email > Message Log

**Look for:**
- **Sent** ✓ - Email left ShootPath successfully
- **Delivered** ✓ - Email accepted by recipient's server
- **Opened** ✓ - Client opened the email
- **Failed** ❌ - Something went wrong

**If many emails show "Failed":**
- Check your integration is still connected
- Verify sending limits not exceeded
- Review spam/bounce reasons

### Email Authentication (SPF, DKIM)

Email authentication helps your emails avoid spam folders. Here's what you need to know:

#### What is SPF?

**SPF (Sender Policy Framework)** tells receiving servers which mail servers are allowed to send email from your domain.

**Example:**
Your domain is "yourstudio.com"

**Without SPF:**
Anyone can send email claiming to be from "yourname@yourstudio.com" - spammers love this!

**With SPF:**
Your DNS records say "Only these servers can send email for yourstudio.com: [list]"

Receiving servers check this and reject spoofed emails.

#### What is DKIM?

**DKIM (DomainKeys Identified Mail)** adds a digital signature to your emails proving they came from your server and weren't modified in transit.

**How it works:**
1. Your mail server signs outgoing emails with a private key
2. Your DNS records contain the public key
3. Receiving servers verify signature using public key
4. If valid: email is authentic ✓
5. If invalid: email might be spam or tampered with ❌

#### Do I Need to Set These Up?

**If using Gmail:**
Google handles SPF and DKIM automatically. You don't need to do anything!

**If using custom SMTP:**
Your email provider should have SPF and DKIM configured. But if emails go to spam, you may need to verify:

**Check with your host:**
"Do you have SPF and DKIM configured for my domain?"

**Most say yes.** If not, they can help you set them up.

**Testing email authentication:**
1. Send an email to yourself
2. Open email in Gmail
3. Click three dots (⋮) > "Show original"
4. Look for:
   - "SPF: PASS"
   - "DKIM: PASS"

If both pass, you're good!

### Using Your Own Domain for Email

Many photographers use email addresses at their own domain:

- emma@crashingelegance.com
- hello@yourname.photography
- studio@yourname.com

This looks more professional than:
- emmaphotography123@gmail.com

#### How to Get a Custom Domain Email

**Option 1: Google Workspace (recommended)**

**What it is:**
Gmail with your own domain

**Cost:**
$6/user/month (Business Starter plan)

**Benefits:**
- Professional email address
- Same Gmail interface you know
- 30GB storage
- Calendar, Drive included
- Easy ShootPath integration (use Gmail connection)

**Setup:**
1. Buy domain (Google Domains, Namecheap, GoDaddy)
2. Sign up for Google Workspace
3. Verify domain ownership
4. Create email addresses
5. Connect to ShootPath using Gmail integration (not SMTP!)

**Option 2: Email hosting with your web host**

**What it is:**
Email accounts included with your website hosting

**Cost:**
Usually free with hosting (or $1-5/month)

**Benefits:**
- Bundled with existing hosting
- Often unlimited addresses
- Direct support from host

**Drawbacks:**
- Interface might not be as nice as Gmail
- May have lower sending limits
- Need to use SMTP integration (not Gmail)

**Setup:**
1. Buy domain and hosting (Bluehost, SiteGround, etc.)
2. Create email accounts in hosting control panel
3. Get SMTP settings from host
4. Connect to ShootPath using SMTP integration

### Email Deliverability Tips

Getting emails into client inboxes (not spam) is crucial:

#### Build Good Sending Reputation

**Email providers track:**
- How many emails you send
- How many get marked as spam
- How many get opened
- How many bounce (bad email addresses)

**To maintain good reputation:**
- Only email clients who expect to hear from you
- Don't buy email lists (terrible for deliverability!)
- Clean up bounced addresses
- Use clear, professional language (avoid spam trigger words)

#### Avoid Spam Trigger Words

Words that trigger spam filters:

❌ "FREE!"
❌ "ACT NOW!"
❌ "LIMITED TIME OFFER!"
❌ "CLICK HERE!"
❌ All caps subject lines
❌ Excessive exclamation marks!!!

✅ "Your wedding quote is ready"
✅ "Gallery delivered - download your photos"
✅ "Contract ready for signature"

ShootPath's default templates are already optimized to avoid spam triggers!

#### Verify Email Addresses

**Before sending to a new client:**
Double-check their email address is correct. Common typos:
- gmail.con (not .com)
- yahooo.com (extra 'o')
- Missing letters or transposed characters

**In ShootPath:**
When creating a lead, it validates email format but can't catch typos like "sarah@gnail.com"

**Pro tip:** When you get an inquiry, reply to them first. If your email bounces, you know the address is wrong!

#### Handle Bounces Properly

**Hard bounce:**
Email address doesn't exist. Remove it from your contacts.

**Soft bounce:**
Temporary issue (mailbox full, server down). Try again later.

**ShootPath tracks bounces automatically:**
Settings > Email > Message Log shows bounce reasons

**If an email bounces:**
1. Check the reason in message log
2. Contact client via phone or social media
3. Get correct email address
4. Update in ShootPath
5. Resend

### Troubleshooting Email Issues

#### Issue 1: "Connection Failed" When Testing

**Symptoms:**
Click "Test Connection" and see error

**Common errors and fixes:**

**"Authentication failed (535)"**
- Wrong username or password
- Try your full email address as username
- Check password for typos
- Gmail users: Use app-specific password, not regular password

**"Could not connect to server"**
- Wrong server address
- Check for typos (smtp.gmail.com not stmp.gmail.com)
- Verify server address with your host

**"Connection refused (port 587)"**
- Firewall blocking port
- Try different port (465 or 25)
- Check with your host which ports are open

**"TLS/SSL error"**
- Wrong encryption setting
- Try switching between TLS and SSL
- Try "No encryption" (less secure but may work)

#### Issue 2: Emails Send But Don't Arrive

**Symptoms:**
ShootPath says "Sent ✓" but client never receives email

**Possible causes:**

**1. Emails going to spam**
- Ask client to check spam folder
- Have them mark as "Not Spam"
- Add your email to their contacts

**2. Wrong recipient email**
- Double-check client's email address
- Send test email to that address from Gmail directly
- If that bounces, email is wrong

**3. Email provider delay**
- Sometimes emails take 5-10 minutes
- Check again later
- Look in ShootPath message log for delivery status

**4. Client's inbox full**
- Rare but happens
- Email bounces back
- Contact client another way

#### Issue 3: Daily Sending Limit Reached

**Symptoms:**
"You have reached your daily sending limit"

**For Gmail users:**
- Free Gmail: 500 emails/day
- Limit resets midnight Pacific Time
- Wait until tomorrow or upgrade to Google Workspace

**For SMTP users:**
- Check your hosting plan's limits
- Upgrade plan if needed
- Contact host to raise limits

**To avoid hitting limits:**
- Spread out bulk sends over several days
- Use Mailchimp for newsletters (not ShootPath)
- ShootPath is for transactional emails only

#### Issue 4: Gmail OAuth Connection Expires

**Symptoms:**
Was working, now showing "Gmail connection expired"

**Why this happens:**
- Google security review
- You changed Gmail password
- You revoked ShootPath access in Google settings
- Token expired (rare)

**Fix:**
1. Go to Settings > Integrations > Email
2. Click "Disconnect Gmail"
3. Click "Connect Gmail" again
4. Re-authorize
5. Test again

#### Issue 5: "From" Address Doesn't Match

**Symptoms:**
Emails show wrong sender name or address

**For Gmail:**
- Emails always come from the Gmail account you connected
- To change: Disconnect and reconnect different account

**For SMTP:**
- "From Address" must match authenticated account
- You can't send from jane@domain.com if logged in as support@domain.com
- Update SMTP settings to use correct account

#### Issue 6: Emails Look Broken on Mobile

**Symptoms:**
Client says email is unreadable on phone

**Possible causes:**
- Email template has HTML formatting issues
- Images too large
- Links broken

**Fix:**
1. Send test email to yourself
2. Open on your phone
3. Identify what's broken
4. Contact ShootPath support with screenshot
5. They'll fix template

### Best Practices Summary

**1. Connect Email During Onboarding**

Don't wait! Get email set up before sending your first quote.

**2. Use Gmail If Possible**

Easiest setup, best deliverability, works for 90% of photographers.

**3. Test Before Going Live**

Send test emails to yourself, check they look good, verify links work.

**4. Monitor Deliverability**

Check email logs weekly - are emails delivering successfully?

**5. Keep Sending Limits in Mind**

If you're approaching limits, plan accordingly or upgrade plan.

**6. Use Professional Email Address**

Custom domain email (yourname@yourstudio.com) looks more professional than free Gmail.

**7. Verify Email Addresses**

Typos waste everyone's time and hurt deliverability reputation.

**8. Don't Send Marketing Emails Through ShootPath**

Use Mailchimp, ConvertKit, or similar for newsletters. ShootPath is for transactional emails only (quotes, invoices, galleries).

### What's Next?

Now that you've connected email, you're ready to send professional client communications!

**Create email templates** → [Email Templates](../email-templates/) to customize what clients receive

**Set up workflows** → [Workflows](../workflows/) to automate when emails are sent

**Send your first quote** → [Sending Quotes](../quotes/sending-quotes) walks through the process

**Connect other integrations** → [Integrations Overview](./index) to complete your setup

---

**Questions?** Look for the help links throughout ShootPath, or reach out to support if you need assistance!
