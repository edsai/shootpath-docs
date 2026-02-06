---
sidebar_position: 4
---

# Email Delivery Issues

## Quick Reference

Having trouble with emails not sending or going to spam? This guide covers common email delivery problems in ShootPath, from Gmail integration issues to SMTP connection errors.

**Common Email Problems:**
- Emails not sending → Check email integration connection
- Emails going to spam → Improve sender reputation, use proper formatting
- SMTP connection errors → Verify SMTP settings and credentials
- Gmail integration not working → Reauthorize OAuth connection
- Client not receiving emails → Ask client to check spam, whitelist your address

**Quick Troubleshooting:**
1. Check email integration: **Settings → Integrations → Email** (should show "Connected")
2. Check sent email logs: **Settings → Integrations → Email → Recent Emails**
3. Send test email to yourself
4. Check spam folder
5. Verify client email address is correct

:::tip Most Common Causes
95% of email issues are caused by:
1. Email integration not connected (check Settings → Integrations)
2. Gmail security settings blocking the connection (enable "Less secure app access")
3. Emails going to client's spam folder (ask them to check)
:::

---

## Detailed Guide

### Emails Not Sending

If you're trying to send an email and it's not going out:

**Step 1: Check Email Integration Status**

1. Go to **Settings → Integrations**
2. Find the **Email** section
3. Check status:
   - **Connected** (green checkmark) - Integration is working
   - **Not Connected** or **Disconnected** (red X) - Integration needs setup/reconnection

**If Not Connected:**
You must connect an email service before you can send emails. See [Connecting Email Integration](#connecting-email-integration) below.

**Step 2: Check Recent Email Logs**

1. Go to **Settings → Integrations → Email**
2. Scroll down to **Recent Emails Sent**
3. Find the email you tried to send
4. Check status:
   - **Sent**: Successfully delivered to mail server
   - **Delivered**: Confirmed received by recipient
   - **Bounced**: Email address doesn't exist or mailbox full
   - **Failed**: Error occurred (click for details)
   - **Not Found**: Email was never sent (check if you clicked "Send")

**If Status is "Failed":**
- Click the email to see error message
- Common errors and solutions below

**Step 3: Common Error Messages**

**Error: "Email integration not configured"**
- Solution: Connect Gmail or SMTP in **Settings → Integrations → Email**

**Error: "Daily sending limit exceeded"**
- Gmail free accounts: 500 emails/day
- Gmail Workspace accounts: 2,000 emails/day
- SMTP providers: Varies by provider
- Solution: Wait 24 hours for limit to reset, or upgrade email service

**Error: "Authentication failed"**
- Gmail: OAuth connection expired, reconnect in Settings
- SMTP: Username/password incorrect, update in Settings
- Solution: Reconnect email integration

**Error: "Recipient address rejected"**
- Client email address is invalid
- Common issues: typos, spaces, missing @, wrong domain
- Solution: Fix client's email address in ShootPath and resend

**Error: "Connection timeout"**
- Email server is temporarily unreachable
- Could be your internet, Gmail's servers, or SMTP server
- Solution: Wait 10 minutes and try again

**Error: "Relay access denied"**
- SMTP server requires authentication
- Or: SMTP server doesn't allow relaying from your IP
- Solution: Check SMTP settings, ensure username/password are correct

**Error: "Attachment too large"**
- Most email services limit attachments to 25MB
- ShootPath attachments rarely exceed this (PDFs are small)
- If you're attaching photos: Use gallery links instead

**Step 4: Send a Test Email**

Send an email to yourself to test the integration:

1. Create a test job with your own email as the client
2. Send a quote or invoice email
3. Check if you receive it

**If you receive it:**
- Email integration works correctly
- The problem is specific to certain clients (see [Emails Going to Spam](#emails-going-to-spam))

**If you don't receive it:**
- Check your spam folder
- Check email logs for errors
- Email integration has a problem (see below)

### Connecting Email Integration

ShootPath supports two email methods:

**Option 1: Gmail (Recommended for Most Users)**
- Easy setup (one-click OAuth)
- Reliable delivery
- Free for up to 500 emails/day
- Works with personal Gmail or Google Workspace

**Option 2: SMTP (For Advanced Users)**
- Works with any email provider (SendGrid, Mailgun, Amazon SES, etc.)
- Requires technical setup
- Better for high-volume sending (1000+ emails/day)
- Better deliverability for custom domains

**Connecting Gmail:**

**Step 1: Start Connection**
1. Go to **Settings → Integrations**
2. Find **Email** section
3. Click **Connect Gmail**

**Step 2: Choose Google Account**
- You'll be redirected to Google sign-in
- Choose the Gmail account you want to use for sending emails
- This should be your business email (e.g., [your-email@example.com](mailto:your-email@example.com))

**Step 3: Authorize ShootPath**
- Google will show: "ShootPath wants to access your Gmail account"
- Permissions requested:
  - Send emails on your behalf
  - View email address
- Click **Allow**

**Step 4: Confirm Connection**
- You'll be redirected back to ShootPath
- You'll see: "Gmail connected successfully"
- Email section should now show: **Connected** (green checkmark)

**Step 5: Test the Connection**
- Send a test email to yourself
- Check if you receive it

**If Authorization Fails:**

**Error: "Access blocked: This app's request is invalid"**
- Google Workspace admins can block third-party apps
- Solution: Ask your IT admin to whitelist ShootPath in Google Workspace admin console
- Or: Use a personal Gmail account instead

**Error: "This app isn't verified"**
- Google showing a security warning
- Click **Advanced** → **Go to ShootPath (unsafe)** (it's safe, we're just not fully verified yet)
- Or: Use SMTP instead

**Connecting SMTP:**

You'll need these details from your email provider:

**Required Information:**
- **SMTP Host:** e.g., smtp.gmail.com, smtp.sendgrid.net
- **SMTP Port:** Usually 587 (TLS) or 465 (SSL)
- **Username:** Your email address or account username
- **Password:** Your email password or app-specific password
- **Encryption:** TLS or SSL

**Common SMTP Settings:**

**Gmail:**
- Host: smtp.gmail.com
- Port: 587
- Encryption: TLS
- Username: your-email@gmail.com
- Password: App-specific password (not your regular Gmail password)

**Google Workspace:**
- Host: smtp.gmail.com
- Port: 587
- Encryption: TLS
- Username: your-email@yourdomain.com
- Password: App-specific password

**SendGrid:**
- Host: smtp.sendgrid.net
- Port: 587
- Encryption: TLS
- Username: apikey
- Password: Your SendGrid API key

**Mailgun:**
- Host: smtp.mailgun.org
- Port: 587
- Encryption: TLS
- Username: Your Mailgun SMTP username
- Password: Your Mailgun SMTP password

**Setup Steps:**
1. Go to **Settings → Integrations → Email**
2. Click **Configure SMTP**
3. Enter all required fields
4. Click **Test Connection**
5. If test succeeds, click **Save**

**If Test Fails:**

**Error: "Could not connect to SMTP server"**
- Check host and port are correct
- Check your firewall isn't blocking port 587 or 465
- Try alternate port (587 vs 465)

**Error: "Authentication failed"**
- Username or password is wrong
- For Gmail: You need an app-specific password, not your regular password (see [Gmail SMTP Setup](#gmail-smtp-setup))

**Error: "SSL/TLS error"**
- Wrong encryption setting
- Try TLS instead of SSL, or vice versa

### Gmail Integration Issues

If Gmail was connected but stopped working:

**Reconnect Gmail:**
1. Go to **Settings → Integrations**
2. Find **Email** section
3. Click **Disconnect**
4. Click **Connect Gmail**
5. Authorize again

**Common Gmail Problems:**

**Problem: "Less secure app access" Error**

Gmail may block ShootPath if "Less secure app access" is disabled.

**For Personal Gmail Accounts:**
1. Go to [myaccount.google.com/lesssecureapps](https://myaccount.google.com/lesssecureapps)
2. Turn **ON** "Allow less secure apps"
3. Return to ShootPath and reconnect Gmail

**For Google Workspace Accounts:**
1. This setting is controlled by your IT admin
2. Ask admin to enable "Less secure apps" for your account
3. Or: Use SMTP with app-specific password instead

**Problem: "Account Access Disabled" Email from Google**

Google may send you an email: "Someone just tried to sign in to your Google Account"

**Solution:**
1. In the email, click **Yes, it was me**
2. This tells Google ShootPath is authorized
3. Return to ShootPath and try connecting again

**Problem: Two-Factor Authentication Enabled**

If you have 2FA on your Gmail:
- OAuth connection (Connect Gmail button) should still work
- If using SMTP: You must create an app-specific password

**Creating App-Specific Password:**
1. Go to [myaccount.google.com/apppasswords](https://myaccount.google.com/apppasswords)
2. Click **Select app** → Other (custom name)
3. Enter "ShootPath"
4. Click **Generate**
5. Google shows a 16-character password
6. Copy this password
7. In ShootPath SMTP settings, paste this as your password (not your regular Gmail password)

### Emails Going to Spam

If emails are sending successfully but clients say they never received them:

**Step 1: Verify Email Was Sent**

1. Go to **Settings → Integrations → Email → Recent Emails**
2. Find the email
3. Check status is "Sent" or "Delivered"

If status is "Delivered," the email definitely reached the client's mail server. It's either in their inbox or spam.

**Step 2: Ask Client to Check Spam**

Most email providers have spam filters that can incorrectly flag legitimate emails.

**Gmail:**
- Check **Spam** folder
- Check **Promotions** tab
- Check **Updates** tab

**Outlook/Hotmail:**
- Check **Junk Email** folder
- Check **Focused** vs **Other** tabs

**Yahoo:**
- Check **Spam** folder
- Check **Bulk** folder

**Corporate Email (Office 365, etc.):**
- Check **Junk Email** folder
- Check with IT if emails are quarantined

**If Found in Spam:**
Have client:
1. Mark the email as "Not Spam" or "Not Junk"
2. Add your email address to their contacts
3. Create a filter to always move your emails to inbox

**Step 3: Improve Email Deliverability**

**Why Emails Go to Spam:**
- Sending domain has poor reputation
- Email content looks like spam (too many links, ALL CAPS, etc.)
- No SPF/DKIM records (technical email authentication)
- Client's email provider is overly aggressive

**How to Avoid Spam:**

**Use a Professional Email Domain:**
- **Bad:** Sending from generic Gmail (yourname@gmail.com)
- **Good:** Sending from custom domain (yourname@yourbusiness.com)
- Custom domains are less likely to be flagged as spam

**Improve Email Content:**
- Avoid ALL CAPS in subject lines
- Don't use spam trigger words (FREE, URGENT, ACT NOW, LIMITED TIME)
- Keep links minimal (ShootPath emails only include necessary links)
- Personalize with client's name
- Write naturally, not like marketing copy

**Set Up Email Authentication (Advanced):**
If you're using SMTP with a custom domain, configure:
- **SPF record:** Tells receiving servers your SMTP server is authorized
- **DKIM record:** Cryptographically signs your emails
- **DMARC record:** Tells receivers how to handle failed authentication

These are DNS records. Ask your domain registrar or IT admin for help setting them up.

**Send Test Emails:**
Use [mail-tester.com](https://www.mail-tester.com):
1. Send an email from ShootPath to the address mail-tester provides
2. Check your score (out of 10)
3. Fix issues identified (missing SPF/DKIM, spam content, etc.)

**Warm Up Your Sending Domain:**
If you just started using a new email address:
- Send a few emails per day for the first week
- Gradually increase volume
- This builds sender reputation with email providers

**Step 4: Have Client Whitelist Your Address**

Provide these instructions to clients:

**Gmail:**
1. Open an email from you
2. Click the three dots → **Add [your-name] to Contacts**
3. Or: Settings → Filters → Create new filter → From: [your-email] → Never send to Spam

**Outlook:**
1. Open an email from you
2. Right-click on sender → **Add to Contacts**
3. Or: Settings → Junk email → Safe senders → Add [your-email]

**Yahoo:**
1. Open an email from you
2. Click **Add to Contacts**
3. Or: Settings → Filters → Add new filter → From contains [your-email] → Move to Inbox

### SMTP Connection Errors

If you're using SMTP and getting connection errors:

**Error: "Could not connect to SMTP host"**

**Possible Causes:**
- SMTP host is wrong (typo, missing smtp. prefix)
- SMTP port is wrong (try 587 or 465)
- Your firewall is blocking the port
- SMTP server is temporarily down

**Solutions:**
1. Double-check host and port with your email provider's documentation
2. Try port 587 (TLS) instead of 465 (SSL), or vice versa
3. Check if your router/firewall blocks outbound port 587/465
4. Contact your email provider to confirm SMTP details

**Error: "Authentication failed"**

**Possible Causes:**
- Username is wrong (should be full email address for most providers)
- Password is wrong
- For Gmail with 2FA: Need app-specific password, not regular password

**Solutions:**
1. Verify username is correct (usually your full email address)
2. Verify password is correct
3. For Gmail: Create app-specific password (see [Gmail SMTP Setup](#gmail-smtp-setup))
4. For other providers: Confirm password hasn't expired or been reset

**Error: "Relay access denied"**

**Possible Causes:**
- SMTP server doesn't allow relaying from your IP address
- Authentication is required but not configured

**Solutions:**
1. Ensure you've entered username and password
2. Contact your email provider to confirm your account has SMTP access
3. Some corporate email systems block SMTP relay (use OAuth Gmail instead)

**Error: "SSL/TLS handshake failed"**

**Possible Causes:**
- Wrong encryption setting (TLS vs SSL)
- Outdated SSL certificate
- Man-in-the-middle security software (corporate antivirus)

**Solutions:**
1. Try TLS instead of SSL, or vice versa
2. Update your browser and operating system
3. If on corporate network, ask IT if there's a proxy or antivirus blocking SMTP

### Client Not Receiving Emails

If a specific client says they never receive your emails:

**Step 1: Verify Email Address**

**Check for Typos:**
- Extra spaces before/after email
- Wrong domain (.com vs .net, .org vs .co)
- Swapped letters (gmai.com vs gmail.com)
- Missing or extra dots (john.doe vs johndoe)

**Test the Email:**
Send a test email from your personal email to their address. If it bounces back, the address is wrong.

**Step 2: Check Email Logs**

1. Go to **Settings → Integrations → Email → Recent Emails**
2. Find emails sent to that client
3. Check status:
   - **Bounced**: Email address doesn't exist or mailbox full
   - **Delivered**: Email reached their server (check spam)
   - **Failed**: See error message for details

**Step 3: Ask Client to Whitelist**

Provide these instructions:
- Add your email address to their contacts
- Create filter to move your emails to inbox
- Check spam/junk folder

**Step 4: Use Alternative Email**

If client has multiple email addresses:
- Try sending to their alternate email
- Ask if they prefer personal vs work email
- Some clients' work emails block external messages

**Step 5: Send Via Personal Email**

As a last resort:
- Send from your personal Gmail/Outlook directly (outside ShootPath)
- Include the invoice/quote as an attachment
- Mark it as sent in ShootPath manually

### Email Template Problems

If email templates aren't loading or sending:

**Template Variables Not Replacing:**

Example: Email shows "\{\{client_name\}\}" instead of "John Smith"

**Cause:** Template syntax error or missing data.

**Solution:**
1. Go to **Settings → Email Templates**
2. Click the template having issues
3. Check variable syntax: \{\{variable_name\}\} (two curly braces, no spaces)
4. Common variables:
   - \{\{client_name\}\}
   - \{\{job_type\}\}
   - \{\{quote_total\}\}
   - \{\{invoice_due_date\}\}
5. Save template
6. Send test email to yourself

**Template Formatting Broken:**

Email appears with weird formatting, missing line breaks, etc.

**Cause:** HTML formatting issue.

**Solution:**
1. Edit template
2. Click the **Source** button to view HTML
3. Look for unclosed tags (div tags without closing tags)
4. Simplify formatting (remove complex HTML)
5. Save and test

**Attachments Not Included:**

Quote or invoice PDF not attaching to email.

**Cause:** Attachment generation failed.

**Solution:**
1. Check **Settings → Integrations → Email → Recent Emails**
2. Find the email
3. If error mentions "PDF generation failed":
   - Quote/invoice template may have errors
   - Try regenerating the quote/invoice
   - Contact support if it persists

---

## Common Questions

**Why do my emails go to spam even though I'm using Gmail?**
Sending from a Gmail address (yourname@gmail.com) can still trigger spam filters if:
- You're sending to corporate emails with strict filters
- Your email content looks like marketing/spam
- You're sending to many recipients at once

Use a custom domain (yourname@yourbusiness.com) for better deliverability.

**Can I use my existing email address?**
Yes! You can use:
- Personal Gmail
- Google Workspace (yourname@yourbusiness.com)
- Any email provider via SMTP

**How many emails can I send per day?**
- Gmail free: 500 emails/day
- Google Workspace: 2,000 emails/day
- SMTP providers: Varies (SendGrid, Mailgun have higher limits)

Most photographers send fewer than 50 emails/day, so Gmail free is usually enough.

**Do clients see my email address?**
Yes, emails come FROM your email address (the one you connected in Settings → Integrations). Replies from clients come back to your email inbox.

**Can I change the "From" name?**
Yes:
1. Go to **Settings → Business Information**
2. Update **Business Name**
3. Emails will show as: "Business Name" with your email address

**What if Gmail blocks my account?**
If Gmail suspects unusual activity:
- You'll receive an email: "Suspicious activity blocked"
- Click **Yes, it was me** to confirm
- Reconnect Gmail in ShootPath

If your account is permanently blocked, contact Google support or switch to SMTP.

**Can I use multiple email addresses?**
Currently, ShootPath only supports one email integration at a time. If you have multiple businesses, either:
- Use one email for all
- Switch email integration when needed (disconnect old, connect new)
- Create separate ShootPath accounts

**Why does it take a few minutes for emails to send?**
- ShootPath queues emails to avoid overloading email servers
- Most emails send within 1-2 minutes
- During high usage, may take up to 5 minutes
- Check email logs to confirm sending

---

## Still Having Email Issues?

**Contact Support:**

**For ShootPath Email Integration:**
Email [support@shootpath.com](mailto:support@shootpath.com)
- Include: Email logs screenshots, error messages, steps you tried

**For Gmail Account Issues:**
Contact Google support: [support.google.com/mail](https://support.google.com/mail)

**For SMTP Provider Issues:**
Contact your email provider's support (SendGrid, Mailgun, etc.)

We're here to help get your emails delivering reliably!
