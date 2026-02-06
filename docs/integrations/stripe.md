---
sidebar_position: 2
---

# Stripe Integration

## Quick Reference

Stripe is the payment processor that powers ShootPath's invoicing system. It handles credit card payments securely, deposits money to your bank account, and provides fraud protection - all without you ever touching sensitive card data.

**What is Stripe?**
- Payment processing platform (like Square or PayPal)
- Handles credit/debit card payments
- PCI-compliant (you never see full card numbers)
- Used by millions of businesses worldwide
- Integrates seamlessly with ShootPath

**Key Benefits:**
- **Security** - Card data never touches your servers
- **Simplicity** - Clients pay with one click
- **Speed** - Funds in your bank in 2-3 days
- **Transparency** - Track every transaction
- **Support** - Stripe handles disputes and fraud

**Costs:**
- 2.9% + $0.30 per successful transaction
- No monthly fees, setup fees, or hidden costs
- Example: $1,000 payment = $29.30 fee, you receive $970.70

**Quick Setup:**
Go to **Settings > Integrations > Stripe** and click "Connect". You'll be guided through account creation or connection in about 10 minutes.

**Next Steps:**
- [Connect your Stripe account](#connecting-stripe-to-shootpath)
- [Understand how payments flow](#how-stripe-processes-payments)
- [Learn about fees](#stripe-fees-explained)
- [View your transactions](#stripe-dashboard-tour)

---

## Detailed Guide

### What is Stripe?

Stripe is a payment processing company that handles the complex, technical, and legal aspects of accepting credit card payments online. Think of it as the middleman between your client's credit card and your bank account.

**Without Stripe:**
- You'd need a merchant account (expensive, complicated)
- You'd have to handle card data securely (huge legal liability)
- You'd need to integrate with banks directly (technical nightmare)
- You'd be responsible for fraud detection (risky!)

**With Stripe:**
- They handle all of that for you
- You just send invoices, they process payments
- Money appears in your bank account
- You focus on photography, not payment infrastructure

**Why ShootPath uses Stripe:**

Stripe is the industry standard for online payments. It's:
- **Reliable** - 99.99%+ uptime
- **Secure** - Bank-level encryption and fraud detection
- **Developer-friendly** - Easy for ShootPath to integrate
- **Transparent** - Clear pricing, no hidden fees
- **Global** - Accepts cards from most countries

### How Stripe Works with ShootPath

Here's the flow from invoice to bank account:

#### Step 1: You Send an Invoice

You create an invoice in ShootPath for $1,500 and send it to your client.

#### Step 2: Client Clicks Payment Link

Client receives email, clicks "Pay Now" which opens a Stripe-hosted payment page.

#### Step 3: Client Enters Card Info

Client enters:
- Card number
- Expiration date
- CVC code
- Billing ZIP code

**Important:** This happens on Stripe's secure page, NOT on ShootPath's servers. You never see the full card number!

#### Step 4: Stripe Processes Payment

Stripe:
- Validates card is real and has funds
- Checks for fraud
- Communicates with card issuer (bank)
- Charges the card
- Takes 2-3 seconds

#### Step 5: Payment Confirms

- Client sees "Payment successful!" message
- Client receives email receipt from Stripe
- You receive notification in ShootPath: "Sarah paid $1,500"
- Invoice status changes to "Paid"

#### Step 6: Funds Deposited to Your Bank

- Stripe holds funds for 2-3 business days (standard processing time)
- Funds deposited to your bank account automatically
- You see deposit with description like "Stripe payment - Jan 15"

**Timeline:**
- Client pays: Monday at 10 AM
- Funds available: Wednesday or Thursday morning
- You never have to do anything - it's automatic!

### Connecting Stripe to ShootPath

Before you can accept payments, you need to connect your Stripe account to ShootPath:

#### If You Don't Have a Stripe Account Yet

**Step 1: Go to Settings > Integrations**

Find the "Stripe" section in ShootPath settings.

**Step 2: Click "Connect Stripe Account"**

This starts the connection process.

**Step 3: Create Stripe Account**

You'll be redirected to Stripe's website to create an account:
- Enter email address
- Create password
- Verify email

**Step 4: Complete Stripe Onboarding**

Stripe asks for:
- Business name and address
- Bank account details (where funds will be deposited)
- Tax ID (SSN for individuals, EIN for businesses)
- Identity verification (photo ID)

**Why all this info?**

Stripe is legally required to verify you're a legitimate business. This protects against fraud and money laundering.

**Step 5: Connection Complete**

Once verified, you're redirected back to ShootPath. You'll see "Stripe Connected ✓"

**You're ready to accept payments!**

#### If You Already Have a Stripe Account

**Step 1: Click "Connect Existing Account"**

In ShootPath Settings > Integrations > Stripe.

**Step 2: Log into Stripe**

You'll be redirected to Stripe, log in with your existing credentials.

**Step 3: Authorize Connection**

Stripe asks: "Allow ShootPath to access your account?"
Click "Authorize"

**Step 4: Connection Complete**

You're redirected back to ShootPath with "Stripe Connected ✓"

**Your existing Stripe account now works with ShootPath!**

#### Verification Timeline

**Instant verification (most common):**
- Provide all required info
- Stripe verifies instantly
- Accept payments immediately

**Manual verification (rare):**
- Stripe needs additional documents
- Review takes 1-3 business days
- You'll receive email when approved

**Red flags that trigger manual review:**
- High-risk business category
- International business
- Incomplete information
- Identity doesn't match bank account

**Best practice:** Complete all fields accurately to avoid delays!

### Stripe Fees Explained

Stripe charges a fee for each successful payment. Here's the breakdown:

#### Standard Fee Structure

**Per transaction:**
- 2.9% of transaction amount
- PLUS $0.30 flat fee

**Examples:**

**$500 payment:**
- Fee: ($500 × 0.029) + $0.30 = $14.50 + $0.30 = $14.80
- You receive: $500 - $14.80 = $485.20

**$1,000 payment:**
- Fee: ($1,000 × 0.029) + $0.30 = $29.00 + $0.30 = $29.30
- You receive: $1,000 - $29.30 = $970.70

**$3,000 payment:**
- Fee: ($3,000 × 0.029) + $0.30 = $87.00 + $0.30 = $87.30
- You receive: $3,000 - $87.30 = $2,912.70

**Quick estimate:** About 3% of each payment goes to Stripe.

#### When Fees Are Charged

**Successful payments:**
- Client's card is charged
- Fee is deducted automatically
- You receive net amount (payment minus fee)

**Failed payments:**
- Card declined
- No charge to client
- **No fee to you** (Stripe only charges on successful payments)

**Refunds:**
- You refund $1,000 to a client
- Stripe refunds their $29.30 fee to you
- You get the fee back! (You're not charged twice)

**Partial refunds:**
- Client paid $1,000, you refund $500
- Stripe refunds half the fee ($14.65)
- You keep the rest ($14.65 fee for $500 kept)

#### No Hidden Fees

**What Stripe does NOT charge:**
- Monthly fees
- Setup fees
- Account maintenance fees
- PCI compliance fees (included)
- Payout fees (deposits to your bank are free)
- Dispute/chargeback fees (unless you lose)

**The only cost is 2.9% + $0.30 per successful transaction.**

#### Passing Fees to Clients (Optional)

Some photographers add a "processing fee" to invoices:

**Example 1: Absorb the fee (most common)**
- Invoice: $1,000
- Client pays: $1,000
- You receive: $970.70 (after $29.30 fee)
- You absorb the $29.30 cost

**Example 2: Add processing fee**
- Invoice: $1,030 ($1,000 + $30 processing fee)
- Client pays: $1,030
- You receive: $1,000.40 (after Stripe fee)
- Client absorbs the cost

**Which approach?**
- **Most photographers absorb the fee** - simpler, clients prefer it
- **Some add processing fee** - maintains profit margins, but can annoy clients
- **Hybrid:** Absorb for most, add for very large amounts ($5k+)

**Important:** If you add processing fees, state this in your contract! "Client is responsible for payment processing fees" or "A 3% processing fee applies to credit card payments."

### Client Payment Experience

Let's walk through what your client sees when paying an invoice:

#### Step 1: Client Receives Invoice Email

**Email from ShootPath:**
```
Subject: Invoice from [Your Business Name]

Hi Sarah,

Your invoice for Wedding Photography is ready.

Amount: $1,500.00
Due: March 15, 2026

[View Invoice and Pay]

Questions? Reply to this email!

[Your Business Name]
```

#### Step 2: Client Clicks "View Invoice"

Opens a page showing:
- Your business name and logo
- Invoice details (description, amount, due date)
- Job information
- "Pay Now" button (big and obvious!)

**Design:** Clean, professional, branded to your business.

#### Step 3: Client Clicks "Pay Now"

Redirects to Stripe-hosted payment page:

**What they see:**
```
Pay [Your Business Name]

Invoice #INV-5234-01
Amount: $1,500.00

Card Information
Card number: [____-____-____-____]
MM/YY: [__/__]
CVC: [___]
ZIP: [_____]

[Pay $1,500.00]

🔒 Secured by Stripe
```

**Security indicators:**
- Green padlock in browser
- "https://" in URL (encrypted)
- Stripe branding (trustworthy)

#### Step 4: Client Enters Card Details

Types:
- 16-digit card number
- Expiration month/year
- 3-digit CVC code (back of card)
- Billing ZIP code

**Card types accepted:**
- Visa
- Mastercard
- American Express
- Discover
- Most debit cards

**International cards:**
- Most international cards work
- Some foreign banks block international transactions (client must call bank)

#### Step 5: Client Submits Payment

Clicks "Pay $1,500.00" button.

**Processing (2-3 seconds):**
- Stripe validates card
- Checks for fraud
- Contacts card issuer
- Charges card

**Success screen:**
```
✅ Payment Successful

Your payment of $1,500.00 has been received.

Receipt sent to sarah@example.com

[Download Receipt]

Questions? Contact [Your Business Name]
```

#### Step 6: Client Receives Receipt

**Instant email from Stripe:**
```
Subject: Receipt from [Your Business Name]

Payment Received: $1,500.00

Invoice: INV-5234-01
Date: March 10, 2026 at 2:34 PM
Card: Visa ending in 4242

[Download Receipt PDF]

This charge will appear on your statement as:
[Your Business Name]
```

**Client also sees:**
- Updated invoice in their ShootPath portal (marked "Paid")
- Green checkmark next to invoice
- Payment date and method

**Total experience time:** 60-90 seconds from email to receipt!

### Payment Security and PCI Compliance

One of the biggest benefits of Stripe is you never handle sensitive card data:

#### What is PCI Compliance?

**PCI DSS** (Payment Card Industry Data Security Standard) is a set of strict security requirements for businesses that handle credit card information.

**Without PCI compliance:**
- You're legally liable if card data is stolen
- Fines up to $500,000
- Legal action from card brands (Visa, Mastercard)
- Your business could be shut down

**Why it's hard:**
- Requires secure servers, encryption, audits
- Annual recertification
- Expensive ($5,000-$50,000/year for small businesses)

#### How Stripe Handles PCI Compliance

**The magic:** Card data never touches ShootPath's servers. It goes directly from client's browser to Stripe's servers.

**Flow:**
1. Client enters card number on Stripe-hosted page
2. Card data encrypted and sent to Stripe
3. Stripe stores it securely
4. Stripe sends ShootPath a "token" (not the actual card number)
5. ShootPath uses token to charge card later

**You never see:**
- Full card number (you see last 4 digits: ****4242)
- CVC code
- Any sensitive data

**Benefits:**
- You don't need PCI certification
- You're not liable if there's a data breach
- Stripe handles all security audits
- You focus on photography, not cybersecurity

#### Fraud Detection

Stripe automatically screens every payment for fraud:

**Red flags:**
- Card stolen or reported fraudulent
- Unusual purchase pattern (10 payments in 1 hour)
- IP address mismatch (card issued in USA, payment from Russia)
- Failed CVC check
- Billing address doesn't match

**If fraud is detected:**
- Stripe declines the payment automatically
- Client sees "Payment failed" message
- You're protected (fraudulent charge never goes through)
- Client must use a different card or contact their bank

**Chargeback protection:**

If a client disputes a charge (chargeback), Stripe investigates:
- Reviews payment records
- Checks for fraud indicators
- Asks you for evidence (invoice, contract, communication)
- Makes a decision

**Your evidence:**
- Signed contract proving services were agreed upon
- Email confirmations
- Delivery receipts (you sent the gallery)

**Good documentation protects you from false chargebacks!**

### Handling Payment Failures

Sometimes payments fail. Here's what happens and how to handle it:

#### Common Failure Reasons

**1. Insufficient funds**
- Client's account doesn't have enough money
- Error: "Your card was declined"

**2. Expired card**
- Card expiration date has passed
- Error: "Your card has expired"

**3. Incorrect card details**
- Typo in card number, CVC, or ZIP
- Error: "Your card number is incorrect"

**4. Bank fraud protection**
- Bank flags transaction as suspicious
- Error: "Payment blocked by your bank"

**5. International card restrictions**
- Some banks block international purchases
- Error: "Card cannot be used for international transactions"

**6. Exceeded credit limit**
- Card is maxed out
- Error: "Insufficient credit available"

#### What Happens When Payment Fails

**For the client:**
- Sees error message on payment page
- No charge to their card
- Can try again with different card

**For you:**
- Receive notification: "Payment failed for [Client]"
- Invoice remains unpaid
- No fees charged (Stripe only charges on success)

**ShootPath automatically:**
- Keeps invoice status as "Unpaid"
- Client can retry payment from same link
- No need to send new invoice

#### How to Respond to Failed Payments

**Step 1: Notify client (if they don't reach out first)**

"Hi Sarah, I noticed the payment didn't go through. This usually means the card was declined or there was a technical issue. Can you try again or use a different card? Here's the payment link: [link]"

**Step 2: Troubleshoot common issues**

**If it's insufficient funds:**
"No worries! Sometimes cards decline if the amount is high. Try using a different card or calling your bank to authorize the transaction."

**If it's fraud protection:**
"Your bank may have flagged this as unusual activity. Call them at [number on back of card] and let them know it's a legitimate purchase. Then try again!"

**If it's expired card:**
"Looks like the card might be expired. Double-check the expiration date or try a different card."

**If it's international card:**
"Some international banks block US transactions. You may need to call your bank to authorize international purchases, or use a different card."

**Step 3: Offer alternatives**

"If credit card isn't working, I also accept:
- Bank transfer (ACH)
- Venmo/Zelle
- Check

Let me know what works best!"

#### Preventing Future Failures

**For large amounts:**
- Warn client in advance: "The final payment is $3,000. Make sure your card has sufficient credit!"
- Some clients need to split across multiple cards (Stripe allows this)

**For international clients:**
- Let them know they may need to call their bank
- Provide your business location (helps bank verify it's legitimate)

### Stripe Dashboard Tour

Stripe provides a dashboard where you can view all payment activity:

#### Accessing Stripe Dashboard

**Two ways:**
1. **From ShootPath:** Settings > Integrations > Stripe > "View Stripe Dashboard"
2. **Directly:** Log into dashboard.stripe.com

**What you can do:**
- View all transactions
- See detailed payment records
- Issue refunds
- Manage connected accounts
- Download reports
- Update bank account
- View payout schedule

#### Key Sections

**Home/Overview:**
- Total revenue this month
- Recent payments
- Payout schedule
- Failed payments

**Payments:**
- List of all successful payments
- Filter by date, amount, customer
- Export to CSV for bookkeeping

**Customers:**
- Clients who have paid you
- Payment history per customer
- Saved cards (if you enable it)

**Payouts:**
- Money deposited to your bank
- Schedule (usually every 2-3 days)
- Payout details and statuses

**Disputes:**
- Chargebacks and disputes
- Your responses and evidence
- Resolution status

**Reports:**
- Revenue reports
- Tax reports (1099-K)
- Custom date ranges

#### When to Use Stripe Dashboard

**Daily/weekly:**
- Check that payouts are depositing correctly
- Monitor for any disputes or failed payments

**Monthly:**
- Review revenue totals
- Download reports for bookkeeping

**As needed:**
- Issue refunds
- Respond to disputes
- Update bank info

**Most of the time, you won't need the Stripe dashboard - ShootPath handles everything!** But it's there if you want deeper details.

### Refunds and Disputes

#### Issuing Refunds via Stripe

**Option 1: Refund from ShootPath (easiest)**
1. Open the paid invoice in ShootPath
2. Click "Refund"
3. Choose full or partial
4. Add reason
5. Process refund

**Option 2: Refund from Stripe Dashboard**
1. Log into Stripe dashboard
2. Find the payment
3. Click "Refund"
4. Enter amount
5. Confirm

**What happens:**
- Money returned to client's card
- Appears in 5-10 business days
- Stripe refunds their fee to you
- ShootPath invoice updated to show refund

#### Handling Chargebacks

A **chargeback** is when a client disputes a charge with their bank:

**Common reasons:**
- "I didn't authorize this charge" (card stolen)
- "I didn't receive what I paid for" (you didn't deliver)
- "This isn't what I agreed to" (dispute about services)
- "I already paid this" (duplicate charge)

**What happens:**
1. Client contacts their bank to dispute charge
2. Bank initiates chargeback with Stripe
3. Stripe notifies you
4. Money is temporarily removed from your account
5. You have 7-21 days to respond with evidence
6. Stripe reviews evidence and makes decision
7. If you win: money returned to you
8. If you lose: client keeps money, you lose revenue

**How to protect yourself:**

**Evidence to provide:**
- Signed contract proving client agreed to services
- Email communication (quotes sent, client responses)
- Delivery confirmation (gallery delivered on X date)
- Invoice history showing payment schedule
- Photos showing you fulfilled the service

**Best practices:**
- Keep all contracts signed
- Document all communication
- Deliver on time as promised
- Have clear refund policy in contract

**Most chargebacks are resolved in photographer's favor** if you have good documentation!

### Tax Reporting

Stripe helps with tax reporting:

#### Form 1099-K

If you receive $20,000+ AND have 200+ transactions in a year, Stripe sends you (and the IRS) Form 1099-K reporting your income.

**What it shows:**
- Total gross payments received
- Breakdown by month

**What to do:**
- Include this income on your tax return
- Deduct business expenses (gear, software, mileage)
- Consult with accountant for proper filing

**Below thresholds?**
- No 1099-K issued
- You still must report income on taxes!
- Track it manually in ShootPath or accounting software

#### Accessing Tax Reports

**In Stripe Dashboard:**
1. Go to Reports > Tax
2. Select year
3. Download 1099-K (if applicable)
4. Download transaction reports for your records

**Pro tip:** Export monthly reports from Stripe and give them to your accountant. They'll have everything they need!

### Troubleshooting Common Issues

#### Issue 1: Stripe Connection Fails

**Symptoms:**
- "Unable to connect to Stripe"
- Redirected to Stripe but connection doesn't complete

**Solutions:**
- Clear browser cache and cookies
- Try different browser
- Disable browser extensions (ad blockers)
- Make sure you're clicking "Authorize" on Stripe's page
- Contact support if issue persists

#### Issue 2: Payouts Not Arriving

**Symptoms:**
- Clients paid days ago but money not in bank

**Check:**
- Stripe Dashboard > Payouts (shows estimated arrival date)
- Your bank account is correct in Stripe settings
- It hasn't been rejected (rare - wrong account number)

**Timeline:**
- Client pays Monday → Payout initiated Wednesday → Arrives Thursday/Friday

**If still missing after 5 business days:** Contact Stripe support!

#### Issue 3: High Decline Rate

**Symptoms:**
- Many clients' payments are failing

**Possible causes:**
- Your business is flagged as high-risk (rare for photographers)
- Amounts are unusually high (triggering fraud detection)
- Clients predominantly international (more fraud checks)

**Solutions:**
- Ensure your Stripe account is fully verified
- Add clear business description in Stripe settings
- Contact Stripe support to review account settings

#### Issue 4: Can't Find a Transaction

**Symptoms:**
- Client says they paid but you don't see it in ShootPath

**Check:**
1. Stripe Dashboard > Payments (search by amount or client name)
2. Filter by date range
3. Check "Failed payments" (maybe it didn't go through)

**If payment exists in Stripe but not ShootPath:**
- Refresh ShootPath page
- Check if webhook failed (rare technical issue)
- Contact ShootPath support

### Best Practices

**1. Complete Stripe Verification ASAP**

Don't wait! Verify your account as soon as you connect Stripe so you can accept payments immediately.

**2. Keep Bank Info Updated**

If you change banks, update Stripe settings immediately! Otherwise payouts will fail.

**3. Monitor Stripe Dashboard Weekly**

Quick 5-minute check ensures:
- Payouts are depositing correctly
- No disputes or issues
- Everything is running smoothly

**4. Save All Receipts**

Download transaction reports monthly for your bookkeeping and taxes.

**5. Respond to Disputes Quickly**

If you get a chargeback notice, respond within 7 days with evidence. Faster = better chance of winning!

**6. Test the Client Experience**

Go through the payment process yourself! See what clients see and ensure it's smooth.

### What's Next?

Now that you understand Stripe integration, you're ready to manage your payments with confidence!

**Need to track who's paid?** → [Tracking Payments](../invoices/tracking-payments) shows how to monitor invoice status.

**Want to understand invoicing basics?** → [Invoices Overview](../invoices/) covers the big picture.

**Ready to set up payment schedules?** → [Payment Schedules](../invoices/payment-schedules) explains automatic invoice generation.

**Need to create a custom invoice?** → [Creating Invoices](../invoices/creating-invoices) walks through manual invoices.

---

**Questions?** Look for the help links throughout ShootPath, or reach out to support if you need help!
