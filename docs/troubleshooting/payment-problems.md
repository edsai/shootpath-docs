---
sidebar_position: 3
---

# Payment Problems

## Quick Reference

Having issues with client payments in ShootPath? This guide covers common payment problems, from clients unable to pay invoices to Stripe connection issues and payment verification problems.

**Common Payment Issues:**
- Client payment fails → Check card details, ask client to try different card
- Stripe not connected → Complete Stripe onboarding in Settings → Integrations
- Invoice not sending → Verify email settings and client email address
- Payment not recording → Check Stripe dashboard for transaction
- Refund issues → Process refunds through Stripe dashboard

**Quick Troubleshooting:**
1. Check Stripe connection: **Settings → Integrations → Stripe** (should show "Connected")
2. Verify invoice was sent: **Jobs → Select job → Invoices** (check sent date)
3. Check Stripe dashboard: [dashboard.stripe.com](https://dashboard.stripe.com) (view all transactions)
4. Test with your own card: Pay a test invoice to confirm the flow works

:::tip Most Common Cause
90% of payment problems are caused by:
1. Stripe not properly connected (check Settings → Integrations)
2. Client entered wrong card details (ask them to double-check)
3. Client's bank blocking the transaction (they need to call their bank)
:::

---

## Detailed Guide

### Client Payment Failures

When a client tries to pay an invoice and the payment fails:

**Step 1: Identify the Error**
Ask your client what error message they saw:
- "Card declined"
- "Insufficient funds"
- "Invalid card number"
- "Your card does not support this type of purchase"
- "Transaction blocked by your bank"

**Step 2: Solutions by Error Type**

**Error: "Card Declined"**

Most common causes:
- Insufficient funds
- Card expired
- Incorrect CVC code
- Card reported lost/stolen
- Bank declined for security reasons

**Client actions:**
1. Call their bank to authorize the transaction
2. Tell bank they're paying a photography invoice to [your business name]
3. Ask bank if they block international transactions (Stripe is US-based)
4. Try a different card
5. Ask bank if there's a daily spending limit they've exceeded

**Error: "Insufficient Funds"**
- Client needs to use a different payment method
- Or pay a smaller amount now (if you'll accept partial payment)
- Debit cards show this error immediately; credit cards don't (so it's likely a debit card)

**Error: "Invalid Card Number"**
- Client typed card number incorrectly
- Common mistakes:
  - Swapped digits
  - Used spaces or dashes
  - Entered debit card number instead of credit card (or vice versa)
- Have them re-enter carefully, one digit at a time

**Error: "Card Expired"**
- Client's card has passed its expiration date
- They need to use a different card
- If they recently got a replacement card, use the new card's details

**Error: "CVC Incorrect"**
- The 3 or 4 digit security code on back of card
- Common mistakes:
  - Reading smudged or worn numbers
  - Confusing 0 and O, 1 and I
- Have client check carefully, try again

**Error: "Transaction Blocked by Bank"**
- Bank's fraud detection system flagged the transaction
- This is common for:
  - Large amounts ($1000+)
  - First-time online payments
  - Payments to businesses in different states/countries
  - Multiple failed attempts

**Client must:**
1. Call their bank immediately
2. Tell bank: "I'm trying to pay [your business name] for photography services"
3. Confirm the exact amount
4. Ask bank to authorize the transaction
5. Try payment again within 30 minutes

**Error: "Your Card Does Not Support This Type of Purchase"**
- Some prepaid cards don't work for online payments
- Some gift cards have restrictions
- Corporate cards may block certain merchant categories

**Solutions:**
- Try a personal credit/debit card instead
- Use a different payment method (if you accept PayPal, Venmo, etc.)
- Have client contact their card issuer to enable online purchases

**Step 3: Alternative Payment Methods**

If the client still can't pay via Stripe:

**Option 1: Try a Different Card**
- Many people have multiple cards
- Try credit card vs debit card
- Try a card from a different bank

**Option 2: Bank Transfer/Check**
- Provide your bank account details for ACH/wire transfer
- Or accept a check (note: slower and less secure)
- Mark invoice as paid manually once you receive funds

**Option 3: In-Person Payment**
- If you're meeting the client in person, bring a mobile card reader
- Square, PayPal, or Stripe mobile readers work for in-person payments
- Or accept cash/check

**Option 4: Split Payment**
- Some banks have daily spending limits
- Client can pay half today, half tomorrow
- You'll need to create multiple invoices or mark partial payments

### Stripe Connection Issues

If Stripe isn't connected or stopped working:

**Check Connection Status:**
1. Go to **Settings → Integrations**
2. Find Stripe section
3. Status should show: **Connected to Stripe** (green checkmark)

**If Not Connected:**
You'll see a "Connect Stripe" button.

**Connecting Stripe for the First Time:**

**Step 1: Create Stripe Account** (if you don't have one)
1. Click **Connect Stripe** in ShootPath
2. You'll be redirected to Stripe's website
3. Click **Create Account**
4. Fill in:
   - Email address
   - Full name
   - Country
   - Password
5. Click **Create Account**

**Step 2: Complete Stripe Onboarding**
Stripe requires business information before you can accept payments:

**Business Information:**
- Business type (Individual / Sole Proprietor / LLC / Corporation)
- Business name (or your name if sole proprietor)
- Business website (optional)
- Business description: "Photography services"

**Personal Information:**
- Full legal name (as it appears on government ID)
- Date of birth
- Last 4 digits of SSN (US) or equivalent (other countries)
- Phone number
- Home address

**Banking Information:**
- Bank name
- Routing number (9 digits for US banks)
- Account number
- Account holder name

**Why Stripe Needs This:**
- Required by law for payment processing (Know Your Customer regulations)
- Stripe deposits your earnings to this bank account
- Used for identity verification

**Step 3: Verify Your Identity**
Stripe may ask you to upload:
- Photo of government-issued ID (driver's license, passport)
- Photo of a recent bank statement or utility bill (for address verification)

Use clear, well-lit photos. This typically approves within minutes to 24 hours.

**Step 4: Verify Email**
- Stripe sends a verification email
- Click the link in the email
- This confirms you own the email address

**Step 5: Return to ShootPath**
After completing Stripe onboarding:
1. Stripe will redirect you back to ShootPath
2. You'll see "Stripe connected successfully"
3. Go to **Settings → Integrations** to confirm the green checkmark

**If Connection Was Lost:**

**Reconnecting Stripe:**
1. Go to **Settings → Integrations**
2. Click **Reconnect Stripe**
3. Log in to your Stripe account
4. Authorize ShootPath to access your Stripe account
5. You'll be redirected back to ShootPath

**Common Reasons Connection is Lost:**
- You changed your Stripe password (requires reauthorization)
- You revoked ShootPath's access in Stripe dashboard
- Stripe detected suspicious activity and paused the connection
- Your Stripe account was temporarily suspended (verify with Stripe support)

**Test Your Stripe Connection:**
After connecting/reconnecting:
1. Create a test invoice in ShootPath
2. Send it to your own email
3. Try paying with your own card
4. Verify the payment appears in:
   - ShootPath (Job → Invoices → Payment History)
   - Stripe dashboard ([dashboard.stripe.com](https://dashboard.stripe.com) → Payments)

**Stripe Account Suspended/Restricted:**
If you see "Your Stripe account is restricted" in ShootPath:
1. Log in to [dashboard.stripe.com](https://dashboard.stripe.com)
2. You'll see a banner explaining why
3. Common reasons:
   - Missing or incomplete business information
   - Failed identity verification
   - Suspicious activity flagged
   - High chargeback rate
4. Follow Stripe's instructions to resolve
5. Contact Stripe support if unclear: [stripe.com/contact](https://stripe.com/contact)

Once Stripe lifts the restriction, your ShootPath payments will work again (no need to reconnect).

### Invoice Not Sending

If you're trying to send an invoice and it's not reaching your client:

**Step 1: Verify Email Settings**

**Check Your Email Integration:**
1. Go to **Settings → Integrations**
2. Find Email section
3. Status should show: **Connected** (Gmail, SMTP, etc.)

**If Not Connected:**
- Emails can't send without an email integration
- See [Email Delivery Issues](#email-delivery-issues) below for setup help

**Step 2: Verify Invoice Was Sent**

**In ShootPath:**
1. Go to the job
2. Click **Invoices** tab
3. Find the invoice
4. Check **Sent Date** column
   - If blank: Invoice was never sent
   - If shows date: Invoice was sent, but may not have been delivered

**Send/Resend Invoice:**
1. Click the invoice
2. Click **Send Invoice** (or **Resend** if already sent)
3. Confirm client's email address is correct
4. Click **Send**

**Step 3: Check Client's Email**

**Ask Client to Check:**
- Inbox (duh)
- Spam/Junk folder
- Promotions tab (Gmail)
- Quarantine (corporate email systems)

**Have Client Whitelist Your Email:**
Add your sending email (the one configured in Settings → Integrations → Email) to their contacts or safe sender list.

**Step 4: Check Email Logs**

**In ShootPath:**
1. Go to **Settings → Integrations → Email**
2. Scroll down to **Recent Emails Sent**
3. Find the invoice email
4. Check status:
   - **Sent**: Successfully delivered to mail server
   - **Delivered**: Confirmed delivered to recipient
   - **Bounced**: Email address doesn't exist or mailbox full
   - **Failed**: Error sending (see error message)

**If Bounced:**
- Client's email address is wrong (typo)
- Client's mailbox is full
- Client's email account was closed
- Fix email address and resend

**If Failed:**
- See error message for details
- Common causes:
  - Email integration not configured correctly
  - Daily sending limit exceeded
  - Email service (Gmail, SMTP) is down

**Step 5: Test Email Sending**

Send a test email to yourself:
1. Create a test invoice
2. Enter your own email as the client
3. Send the invoice
4. Check if you receive it

If you receive it:
- Your email setup works
- The issue is with the client's email address or their email provider

If you don't receive it:
- Email integration is not configured correctly
- See [Email Delivery Issues](#email-delivery-issues) below

### Payment Not Recording

If a client paid an invoice but it's not showing in ShootPath:

**Step 1: Check Stripe Dashboard**

Log in to your Stripe dashboard at [dashboard.stripe.com](https://dashboard.stripe.com):
1. Go to **Payments**
2. Search for the client's name or invoice number
3. Check if payment appears there

**If Payment Shows in Stripe but Not ShootPath:**

**Cause:** Webhook connection issue between Stripe and ShootPath.

**Solution 1: Manual Sync**
1. In ShootPath, go to the job
2. Click **Invoices** tab
3. Click **Sync with Stripe** button
4. ShootPath will fetch all payments from Stripe and update the invoice

**Solution 2: Mark as Paid Manually**
If sync doesn't work:
1. Click the invoice
2. Click **Record Payment**
3. Enter:
   - Amount paid
   - Payment date (check Stripe for exact date)
   - Payment method: Credit Card
   - Transaction ID: Copy from Stripe payment details
4. Click **Save**

**Solution 3: Reconnect Stripe**
If webhooks are broken:
1. Go to **Settings → Integrations**
2. Click **Disconnect** next to Stripe
3. Click **Connect Stripe** again
4. Log in and authorize
5. Try syncing payments again

**If Payment Doesn't Show in Stripe Either:**

**Possible Causes:**
- Client never actually completed the payment (got an error and gave up)
- Client used a different Stripe account (if you have multiple businesses)
- Payment is in test mode instead of live mode

**Check Test Mode:**
In Stripe dashboard:
- Look for "TEST DATA" banner at the top
- Toggle to "Live" mode
- Check if payment appears there

**Ask Client:**
- Did they receive a payment confirmation email from Stripe?
- Did their card get charged? (Check bank statement)
- What happened after clicking "Pay Now"?

**Step 2: Check for Partial Payments**

If client paid less than the full invoice amount:
1. In ShootPath, go to invoice
2. Check **Payment History** section
3. You'll see all payments made
4. Total may be less than invoice total (shows balance due)

Partial payments are automatically tracked. Client can make additional payments until invoice is paid in full.

**Step 3: Check for Refunds**

If payment showed up then disappeared:
1. Check Stripe dashboard → Payments
2. Click the payment
3. Look for "Refunded" status
4. If refunded: Check who initiated it (you or Stripe)

Stripe may automatically refund if:
- Payment was flagged as fraudulent
- Chargeback was filed
- You refunded through Stripe dashboard

### Refund Issues

If you need to refund a client:

**How to Issue Refunds:**

**Full Refund:**
1. Log in to [dashboard.stripe.com](https://dashboard.stripe.com)
2. Go to **Payments**
3. Find and click the payment you want to refund
4. Click **Refund Payment**
5. Confirm the amount (should be full amount)
6. Click **Refund**

The refund appears on the client's card in 5-7 business days.

**Partial Refund:**
Same process, but:
1. Click **Refund Payment**
2. Change amount to the partial amount
3. Click **Refund**

**Refund Shows in Stripe but Not ShootPath:**
1. Go to job in ShootPath
2. Click **Invoices** tab
3. Click **Sync with Stripe**
4. Refund should now appear

Or mark manually:
1. Click invoice
2. Click **Record Refund**
3. Enter amount and date
4. Click **Save**

**Client Says They Didn't Receive Refund:**

**Timeline:**
- Credit cards: 5-7 business days
- Debit cards: 5-10 business days
- Some banks take longer (up to 14 days)

**If It's Been Longer:**
1. Check Stripe dashboard to confirm refund status is "Succeeded"
2. Get the refund ID from Stripe (starts with "re_")
3. Client should contact their bank with:
   - Refund ID
   - Original charge amount and date
   - Refund amount and date
   - Your business name
4. Bank can trace the refund

**Stripe Refund Fees:**
- Stripe charges 2.9% + $0.30 to process the original payment
- When you refund: Stripe refunds 2.9% but keeps the $0.30
- Example: $100 payment, you refund $100, you get back $97.40 (lose $2.60)

**Partial Refunds:**
- Stripe refunds a proportional amount of the percentage fee
- But still keeps the $0.30
- Example: $100 payment, you refund $50, you lose $2.15

This is Stripe's policy, not ShootPath's. We don't receive any portion of Stripe's fees.

### Payment Verification Problems

When payments need verification or aren't being deposited to your bank:

**Stripe Account Under Review:**

**Why This Happens:**
- New account (first 30 days)
- Sudden large payment (10x your normal)
- High-risk business indicators
- Customer disputes
- Unusual activity pattern

**What to Do:**
1. Log in to Stripe dashboard
2. You'll see a banner: "Your account is under review"
3. Follow Stripe's instructions:
   - Provide additional documentation (invoices, contracts)
   - Answer questions about your business
   - Upload identity documents
4. Stripe typically reviews within 24-48 hours

**During Review:**
- New payments are held (not transferred to your bank)
- Clients can still pay invoices
- Once review completes, held funds are released

**Payout Delays:**

**Normal Payout Schedule:**
- 2 business days after payment
- Example: Client pays Monday, you receive it in your bank Wednesday

**If Payouts Are Delayed:**

**Check Stripe Dashboard:**
1. Go to **Balance**
2. You'll see:
   - Available: Ready to be paid out
   - Pending: Will be available in X days
3. Click **Payouts** to see schedule

**Reasons for Holds:**
- **New account:** Stripe holds payouts for 7-14 days for first few transactions
- **High-risk transaction:** Manually reviewed before payout
- **Chargeback:** Stripe holds amount until chargeback resolves
- **Bank account not verified:** Verify bank account in Stripe settings

**If Your Bank Account is Wrong:**

**Update Bank Account in Stripe:**
1. Go to Stripe dashboard → **Settings**
2. Click **Bank accounts and scheduling**
3. Add your correct bank account
4. Verify it (Stripe makes two small deposits, you confirm the amounts)
5. Set as default payout account
6. Remove old account once verified

**Bank Rejected the Deposit:**

**Common Reasons:**
- Account number is wrong
- Routing number is wrong
- Account is closed
- Bank doesn't accept ACH deposits (rare)

**Solution:**
1. Contact your bank to confirm account can receive ACH deposits
2. Verify account and routing numbers (check a physical check or bank's website)
3. Update bank account in Stripe
4. Stripe will automatically retry the payout

### Test Mode vs. Live Mode

A very common issue: Accepting test payments instead of real ones.

**Understanding Stripe Modes:**

**Test Mode:**
- For testing without real money
- Uses test card numbers (4242 4242 4242 4242)
- Payments don't actually charge cards
- Money doesn't move
- Marked with "TEST DATA" in Stripe dashboard

**Live Mode:**
- Real payments
- Real money
- Client's cards actually charged
- Money deposited to your bank

**How to Check Which Mode You're In:**

**In Stripe Dashboard:**
- Look for toggle in top left: "Test mode" or "Live mode"
- Or look for "TEST DATA" banner

**In ShootPath:**
1. Go to **Settings → Integrations → Stripe**
2. Look for "Mode: Test" or "Mode: Live"

**If You're in Test Mode:**
- Client payments won't actually process
- No real money will be collected
- You'll see successful payments in Stripe, but they're fake

**Switching to Live Mode:**

**In ShootPath:**
You can't switch modes directly in ShootPath. You need to connect live mode from Stripe.

**Steps:**
1. Go to **Settings → Integrations**
2. Click **Disconnect** next to Stripe
3. Click **Connect Stripe**
4. Log in to Stripe
5. In Stripe, make sure you're in **Live** mode (toggle in top left)
6. Complete the connection
7. ShootPath is now connected to live mode

**Warning:**
- Don't accidentally use test mode for real clients
- Always verify you're in live mode before sending payment links
- Test mode payments can't be converted to live payments (you'd need to have client pay again)

### Multiple Stripe Accounts

If you have multiple Stripe accounts (e.g., for different businesses):

**Making Sure ShootPath Uses the Right Account:**
1. Go to **Settings → Integrations → Stripe**
2. You'll see the email address of the connected Stripe account
3. If it's wrong:
   - Click **Disconnect**
   - Click **Connect Stripe**
   - Log in with the CORRECT Stripe account
   - Authorize

**Payments Going to Wrong Stripe Account:**
- Disconnect and reconnect with correct account
- Payments will now go to the new account
- Past payments remain in the old account (you can't move them)

---

## Common Questions

**Why does Stripe take 2-3 days to deposit money in my bank?**
This is standard ACH processing time. You can enable **Instant Payouts** in Stripe (for 1% fee) to get money within minutes, but this is only available for Visa debit cards, not bank accounts.

**Can clients pay with PayPal, Venmo, or Apple Pay?**
ShootPath currently only integrates with Stripe for online payments. However, Stripe supports:
- Apple Pay (automatically enabled for Safari users)
- Google Pay (automatically enabled for Chrome users)
- Credit/debit cards (Visa, Mastercard, Amex, Discover)

For PayPal/Venmo: You'd need to send a separate payment link and mark the invoice as paid manually in ShootPath.

**Do clients need a Stripe account to pay?**
No! Clients simply enter their card details. They never see Stripe branding (it's your business name on their bank statement).

**What happens if a client disputes a charge?**
1. Stripe notifies you via email
2. You have 7 days to respond with evidence (contract, photos delivered, etc.)
3. Stripe submits evidence to the card issuer
4. Card issuer decides (takes 30-60 days)
5. If you win: Client's dispute is denied, you keep the money
6. If you lose: Stripe reverses the charge, and you owe a $15 chargeback fee

**Can I accept payments without Stripe?**
ShootPath requires Stripe for online invoice payments. However, you can:
- Accept cash/check in person and mark invoice as paid manually
- Use another payment processor and manually record payments
- But you lose the automation (reminders, client portal, etc.)

**How do I lower Stripe's fees?**
Stripe's standard rate is 2.9% + $0.30 per transaction. If you process over $100k/year, contact Stripe for custom pricing. ShootPath doesn't mark up these fees.

**Can I use my existing Stripe account?**
Yes! When connecting Stripe in ShootPath, just log in with your existing Stripe account credentials. You don't need to create a new account.

**What if I change banks?**
1. Update your bank account in Stripe dashboard (**Settings → Bank accounts**)
2. Verify the new account (Stripe makes 2 small deposits)
3. Set as default payout account
4. Remove old account
5. No need to change anything in ShootPath (it connects to Stripe, not directly to your bank)

---

## Still Having Payment Issues?

**Contact Support:**

**For ShootPath Integration Issues:**
Email [support@shootpath.com](mailto:support@shootpath.com)
- Include: Description of issue, screenshots, invoice number

**For Stripe Account Issues:**
Contact Stripe support: [stripe.com/contact](https://stripe.com/contact) or [support@stripe.com](mailto:support@stripe.com)
- Stripe handles: Account verification, payouts, disputes, chargebacks, account restrictions

**For Client Payment Issues:**
- Client should contact their bank/card issuer
- Have them mention they're paying your business for photography services
- Ask bank to authorize the specific transaction amount

We're here to help resolve any payment problems so you can get paid smoothly!
