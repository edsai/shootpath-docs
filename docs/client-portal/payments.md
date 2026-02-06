---
sidebar_position: 5
---

# Client Payments

## Quick Reference

After signing the contract, clients can pay their invoices directly through the portal using Stripe. Payments are secure, automatic, and update your records in real-time.

**How Payment Works:**
1. Contract must be signed first (Contract-Before-Payment rule)
2. Client clicks portal link to view invoice
3. Stripe payment form loads in the portal
4. Client enters payment details (card or bank account)
5. Payment processes instantly
6. Both parties receive confirmation email
7. Invoice is marked as paid in ShootPath

**Payment Methods Supported:**
- Credit cards (Visa, Mastercard, Amex, Discover)
- Debit cards
- Apple Pay and Google Pay (if enabled)
- ACH bank transfers (optional, 3-5 day processing)

**What Clients See:**
- Clear invoice with amount due
- Breakdown of payment schedule
- Due dates for each payment
- "Pay Now" button with Stripe payment form
- Receipt after successful payment

**Next Steps:** Learn about [portal access](./portal-access) or [quote acceptance](./quote-acceptance).

---

## Detailed Guide

### How Client Payments Work

ShootPath integrates with Stripe to process payments. When a client submits payment through the portal, here's what happens:

**The Flow:**
1. Client opens invoice portal page
2. Reviews amount due and payment details
3. Clicks "Pay Now"
4. Stripe payment form appears (embedded in the portal)
5. Client enters card or bank details
6. Clicks "Submit Payment"
7. Stripe processes payment (takes 2-3 seconds)
8. Money transfers to your Stripe account
9. ShootPath receives confirmation from Stripe
10. Invoice is marked as paid
11. Both parties receive confirmation emails

**All of this happens automatically** - you don't need to manually track payments or mark invoices paid!

:::tip Security Note
Payment processing happens through Stripe, not ShootPath directly. This means credit card numbers never touch your server - they go straight to Stripe's PCI-compliant secure systems. This protects both you and your clients!
:::

### The Client Payment Experience

Let's walk through what your client sees when paying an invoice.

#### Receiving the Invoice Email

After signing the contract, your client receives an email:

```
Subject: Invoice from Sarah Photography

Hi Luna!

Your retainer payment of $1,000 is now due to secure your October 15th
wedding date.

[Pay Invoice]

Payment can be made securely online using a credit card, debit card,
or bank account. You'll receive a receipt immediately after payment.

Looking forward to your big day!
Sarah
```

**Email includes:**
- Amount due clearly stated
- Link to invoice portal page
- Due date (if applicable)
- Accepted payment methods

#### Landing on the Invoice Page

When clicking the portal link, clients see:

**Header:**
- Your business logo
- "Invoice for Luna Garcia"
- Job details (Wedding - October 15, 2024)
- Status: "Payment Due"

**Invoice Details:**
```
Invoice #12345

Retainer Payment for October 15, 2024 Wedding

Amount Due: $1,000.00
Due Date: Today (or specific date)

Payment Schedule:
✓ Retainer — $1,000 — Due today
○ Second Payment — $1,250 — Due August 1, 2024
○ Final Balance — $1,250 — Due October 1, 2024

Total Package Price: $3,500
```

The invoice clearly shows:
- What this specific payment is for
- How much is due
- When it's due
- The full payment schedule (so they know what's coming)

**If multiple payments are due:**
Clients must pay ALL due amounts together. They can't cherry-pick individual payments. For example:
- Retainer was due June 1 (past due)
- Second payment due July 1 (due today)
- Client must pay $2,250 total ($1,000 + $1,250)

This is ShootPath's **Forced Payment Rule** - protects you from clients trying to skip earlier payments!

#### The Payment Form

Below invoice details, clients see a **"Pay Now"** button. Clicking it reveals the Stripe payment form:

**Payment Form Includes:**
- **Email field** (pre-filled with client's email)
- **Card information** (number, expiration, CVC)
- **Billing address** (name, address, zip code)
- **"Submit Payment"** button

**Stripe's Smart Features:**
- **Auto-complete** - Form suggests address based on zip code
- **Card detection** - Automatically identifies card type (Visa, Mastercard, etc.)
- **Error detection** - Highlights invalid card numbers before submission
- **Mobile optimization** - Numeric keyboard on phones, large touch-friendly fields

**Visual Security Indicators:**
- Padlock icon in browser (HTTPS)
- "Secured by Stripe" badge
- Card logos showing supported payment types

These signals reassure clients their payment is secure!

#### Alternative Payment Methods

Depending on your Stripe settings, clients might also see:

**Apple Pay / Google Pay (if enabled):**
- Shows as option on compatible devices
- One-tap payment using saved card
- Extra convenient for mobile users

**ACH Bank Transfer (if enabled):**
- Option to pay directly from bank account
- Lower fees for you (0.8% vs 2.9% for cards)
- Takes 3-5 business days to process
- Great for large payments (like $5,000 wedding balances)

**Link by Stripe (if enabled):**
- Save payment info for faster checkout
- Autofills details on future payments
- Secure storage managed by Stripe

Most photographers stick with card payments only (simpler for clients), but bank transfers can save money on large invoices!

#### Submitting Payment

When the client clicks "Submit Payment":

**Processing (2-3 seconds):**
- Stripe validates card information
- Checks for sufficient funds
- Processes the charge
- Loading spinner shows payment is processing

**Success:**
```
✓ Payment Successful!

Thank you! Your $1,000 retainer payment has been received.

Receipt #: 78910
Transaction ID: ch_abc123xyz789

A receipt has been sent to luna@email.com.

Your October 15th wedding date is now officially secured!
```

**What happens behind the scenes:**
- Money moves to your Stripe account
- Stripe sends webhook to ShootPath
- Invoice is marked as "Paid"
- You receive notification
- Client receives receipt email
- Payment appears in job's payment history

#### Payment Receipt

Both you and your client receive receipt emails from Stripe:

**Client Receipt Includes:**
- Amount paid
- Date and time
- Payment method (last 4 digits of card)
- Business name (your photography business)
- Transaction ID (for their records)
- What the payment was for ("Retainer for October 15, 2024 Wedding")

**Your Notification Includes:**
- Client name
- Amount received
- Job it's attached to
- Net amount (after Stripe fees)
- Link to view in Stripe dashboard

Clients can also download receipt PDFs from the portal or Stripe confirmation email!

### Payment Failures

Sometimes payments fail. Here's how ShootPath handles it:

#### Common Failure Reasons

**Declined Card:**
- Insufficient funds
- Card expired
- Incorrect CVC code
- Bank flagged as suspicious

**Technical Issues:**
- Network timeout
- Browser crashed mid-payment
- Stripe service interruption (rare)

**Client-Side Errors:**
- Closed browser before completing
- Entered wrong card number
- Typo in billing address

#### What Clients See

If payment fails, an error message appears:

```
⚠ Payment Failed

Your card was declined. Reason: Insufficient funds

Please try a different payment method or contact your bank.

[Try Again]
```

**Error messages are specific** to help clients fix the problem:
- "Card expired" → Use a different card
- "Incorrect CVC" → Check the 3-digit code on back
- "Insufficient funds" → Add money to account or use different card

#### What You See

When a payment fails:
- No notification (since no payment was received)
- Invoice remains "Unpaid" in your dashboard
- You don't see the failed attempt (ShootPath only records successful payments)

**If a client reports a failed payment:**
- Ask them to try again
- Suggest a different card or payment method
- Offer to process payment over the phone (if you have a card reader)
- Check your Stripe dashboard for more details on the failure

:::tip Pro Tip
If a client's card keeps getting declined, they can call their bank and let them know they're making a large purchase to a photography business. Banks sometimes flag unusual charges as fraud!
:::

### Payment Schedule Management

ShootPath enforces payment schedules to protect your business:

#### How Payment Schedules Work

When you create a quote, you define a payment schedule:

**Example: Wedding Photography ($3,500 total)**
- **Retainer:** $1,000 — Due at booking (immediately after contract signing)
- **Second Payment:** $1,250 — Due 3 months before wedding
- **Final Balance:** $1,250 — Due 2 weeks before wedding

**Each payment has:**
- **Amount** - How much is due
- **Due Date** - When it must be paid
- **Description** - What it covers ("Retainer," "Final Balance," etc.)

#### Due Date Enforcement

**Before due date:**
- Payment button is available but not urgent
- Invoice shows "Due on [Date]"
- Client can pay early if they want

**On due date:**
- Invoice shows "Due Today"
- Client can pay immediately
- You might send a reminder

**After due date:**
- Invoice shows "Overdue"
- Late fee might apply (if in your contract)
- You should follow up

#### Multiple Payments Due

If a client is behind on payments, ShootPath enforces the **Forced Payment Rule**:

**Example:**
- Retainer ($1,000) was due June 1 → 30 days overdue
- Second payment ($1,250) due today → now also due
- Client sees: "Total Due: $2,250" (can't pay just one)

**Why force combined payments?**
- Prevents cherry-picking ("I'll skip the retainer and just pay the balance")
- Ensures you're not chasing multiple overdue payments
- Protects your cash flow

**Client experience:**
```
Amount Due: $2,250

This includes:
- Retainer Payment — $1,000 (Overdue)
- Second Payment — $1,250 (Due Today)

Both payments must be submitted together.
```

Clear messaging helps clients understand why the amount is higher than expected!

### Payment History and Tracking

Clients can view their payment history in the portal:

**What They See:**
```
Payment History

✓ Retainer — $1,000 — Paid June 15, 2024
○ Second Payment — $1,250 — Due August 1, 2024
○ Final Balance — $1,250 — Due October 1, 2024

Total Paid: $1,000
Remaining Balance: $2,500
```

**Visual indicators:**
- ✓ Green checkmark for paid
- ○ Gray circle for upcoming
- ⚠ Red warning for overdue

**Details for each payment:**
- Amount
- Due date
- Status (paid, pending, overdue)
- Payment method (if paid)
- Transaction ID (if paid)

This transparency helps clients plan and budget!

### What You See in Your Dashboard

When a client submits payment, your admin dashboard updates:

#### Dashboard Notifications

**Activity Feed Shows:**
```
💳 Luna Garcia paid $1,000
   Retainer for October 15, 2024 Wedding
   3 minutes ago
```

**Revenue Metrics Update:**
- "Monthly Revenue" increases by payment amount
- "Year-to-Date Revenue" increases
- Cash flow charts update in real-time

#### Job Details

In the specific job:

**Payment Section Shows:**
- Status: "Retainer Paid" (or "Partially Paid" if more payments pending)
- Payment history with dates and amounts
- Remaining balance
- Next payment due date

**Invoice Section Shows:**
- Invoice marked as "Paid"
- Payment date and time
- Transaction ID from Stripe
- Link to view in Stripe dashboard

#### Stripe Integration

All payment data syncs with your Stripe dashboard:
- View transaction details
- See payment method used
- Check for refund history
- Access settlement reports
- Download payment receipts

**You can view:**
- Gross amount (what client paid)
- Stripe fees (2.9% + $0.30 per transaction)
- Net amount (what you receive)

ShootPath displays the gross amount to clients and the net amount to you!

### Refunds and Adjustments

Sometimes you need to refund a payment:

#### Issuing Refunds

**From Stripe Dashboard:**
1. Find the payment in Stripe
2. Click "Refund"
3. Choose full or partial refund
4. Confirm refund

**What happens:**
- Money returns to client's card (3-5 business days)
- ShootPath receives refund webhook
- Invoice status updates to "Refunded" (or "Partially Refunded")
- Client receives refund confirmation email

**Why refund from Stripe?**
- Ensures money actually goes back to client
- Creates proper audit trail
- Updates all records automatically

#### Partial Refunds

If you need to refund part of a payment (e.g., client canceled but you keep $500 retainer):

1. Refund specific amount in Stripe
2. ShootPath updates invoice showing partial refund
3. Client sees reduced balance

**Example:**
- Client paid $1,000 retainer
- You refund $500 (keeping $500 as cancellation fee)
- Invoice shows: "Paid: $1,000 | Refunded: $500 | Net: $500"

#### Invoice Adjustments

If pricing changes after payment:

**Client owes more:**
- Create a new invoice for the difference
- Or adjust the next scheduled payment

**Client overpaid:**
- Issue partial refund
- Or apply credit to next payment

**Always communicate adjustments clearly** to avoid confusion and disputes!

### Contract-Before-Payment Rule

ShootPath enforces this critical rule: **Clients cannot pay until they've signed the contract.**

**Why this rule exists:**
- **Legal protection** - Signed contract proves client agreed to terms before paying
- **Prevents disputes** - Client can't claim "I didn't know about the cancellation policy"
- **Professional standard** - It's best practice in any service business

**What happens if client tries to pay before signing:**
- Payment button is disabled
- Message displays: "Please sign the contract before submitting payment"
- Portal redirects them to contract page

**Sequence is enforced:**
1. Accept Quote
2. Sign Contract ← Must happen before step 3
3. Submit Payment

No shortcuts allowed!

:::warning Important
Never manually process payments (cash, check, Venmo) without a signed contract! Always follow the proper sequence to protect your business legally.
:::

### Payment Reminders and Follow-Up

While ShootPath can send automatic reminders, you'll often follow up manually:

#### Before Due Date (1 week out)

```
Hi Luna!

Quick reminder that your second payment of $1,250 is due on August 1st
(one week from today).

You can pay anytime through your client portal - just click the link
in the original invoice email or let me know if you need me to resend it!

Looking forward to your October wedding!
Sarah
```

**Friendly, helpful tone** - not demanding or pushy.

#### On Due Date

```
Hey Luna!

Your second payment of $1,250 is due today. You can submit it through
the client portal using the link from my previous email.

Let me know if you have any questions or need help accessing the portal!

Thanks!
Sarah
```

**Professional but casual** - acknowledge the due date without being aggressive.

#### After Due Date (3-5 days overdue)

```
Hi Luna,

I wanted to reach out about your second payment of $1,250, which was
due on August 1st. I haven't received it yet and wanted to make sure
there weren't any issues!

If there's a problem with the payment portal or you need to discuss
a different payment plan, please let me know. I'm here to help!

Thanks!
Sarah
```

**Assumes positive intent** - maybe they forgot or had a technical issue.

#### Seriously Overdue (2+ weeks)

```
Hi Luna,

Your second payment of $1,250 is now 15 days overdue. According to
our signed contract, late payments may incur fees and could affect
my ability to fulfill our agreement.

I want to work with you to resolve this, but I need to hear from you.
Please reach out as soon as possible so we can get this sorted out.

Thank you,
Sarah
```

**Firmer tone but still professional** - reference the contract and consequences.

:::tip Payment Collection Strategy
Start friendly and get progressively more formal if payments remain outstanding. Most clients just forgot or had a technical issue - give them the benefit of the doubt first!
:::

### Payment Methods and Fees

Understanding payment options and costs:

#### Credit/Debit Cards

**Stripe Fee:** 2.9% + $0.30 per transaction

**Example:**
- Client pays: $1,000
- Stripe fee: $29.30
- You receive: $970.70

**Pros:**
- Instant processing (money in your account in 2 days)
- Widely accepted (everyone has a card)
- Familiar to clients

**Cons:**
- Higher fees
- Chargeback risk (though rare with signed contracts)

#### ACH Bank Transfers

**Stripe Fee:** 0.8% + $0 (capped at $5)

**Example:**
- Client pays: $1,000
- Stripe fee: $5 (capped)
- You receive: $995

**Pros:**
- Much lower fees (especially for large payments)
- Lower chargeback risk
- Good for high-value invoices ($3,000+)

**Cons:**
- Takes 3-5 business days to process
- Not all clients are comfortable entering bank details online
- More complex setup for clients

#### Apple Pay / Google Pay

**Stripe Fee:** Same as credit cards (2.9% + $0.30)

**Example:**
- Same fees as card payment
- Just faster/easier for client

**Pros:**
- Extremely convenient on mobile
- Clients don't have to type card numbers
- Feels modern and secure

**Cons:**
- Only works on Apple/Android devices
- Requires saved payment method
- Same fees as regular cards

**Most photographers accept all payment types** and let clients choose what's easiest for them!

### Handling Special Payment Situations

#### Client Wants to Pay by Check

While ShootPath integrates with Stripe for online payments, some clients prefer checks:

**If you accept checks:**
1. Client mails check to your business address
2. You receive and deposit check
3. Manually mark invoice as "Paid" in ShootPath
4. Add note: "Paid by check #1234 on [date]"

**Pros:**
- No processing fees
- Some older clients prefer checks

**Cons:**
- Slower (mail time + bank processing)
- Manual tracking required
- Check could bounce

**Best practice:** Encourage online payment for speed and convenience, but accept checks if clients insist.

#### Client Wants to Pay Cash

**If you accept cash:**
1. Meet in person to collect cash
2. Provide handwritten receipt
3. Manually mark invoice as "Paid" in ShootPath
4. Add note: "Paid in cash on [date]"

**Important:** Always give a receipt when accepting cash, and track it for tax purposes!

#### Client Wants to Use Venmo/PayPal/Zelle

These apps aren't integrated with ShootPath:

**If you accept these:**
1. Client sends money via app
2. You manually mark invoice as "Paid" in ShootPath
3. Add note: "Paid via Venmo on [date]"

**Be aware:**
- These apps don't have the same fraud protection as Stripe
- Harder to track for tax purposes
- No automatic integration with ShootPath

**Recommendation:** Encourage Stripe portal payment as the primary method, but be flexible for clients who really want to use alternative methods.

### Best Practices for Client Payments

#### Set Clear Expectations

**In your contract:**
- State accepted payment methods
- Define due dates clearly
- Explain late payment consequences
- Outline refund policy

**In your communications:**
- Remind clients of upcoming due dates
- Send payment links proactively
- Answer payment questions promptly

#### Make Payment Easy

**Remove friction:**
- Send direct links to invoice portal page
- Offer multiple payment methods
- Accept early payments (don't restrict)
- Provide clear instructions

**The easier you make it to pay, the faster you get paid!**

#### Follow Up Consistently

**Create a follow-up schedule:**
- 1 week before due date: Friendly reminder
- On due date: Gentle nudge
- 3 days overdue: Check-in message
- 1 week overdue: Firmer reminder
- 2 weeks overdue: Formal notice

**Be predictable and professional** in your follow-up approach.

#### Track Everything

**Keep records of:**
- All payments received (automatically tracked in ShootPath)
- All payment reminders sent
- Any payment arrangements or adjustments
- Refunds issued

**Good records protect you** if there's ever a dispute or tax audit!

#### Stay Professional

**Even when frustrated:**
- Don't get emotional about late payments
- Stick to the facts and contract terms
- Offer solutions, not ultimatums (until truly necessary)
- Remember most clients want to pay - they just need reminders

**Your demeanor affects your reputation** - stay cool and professional!

### Common Questions About Payments

#### "Can I charge a deposit via Stripe but accept the balance in cash?"

Yes! ShootPath tracks each payment separately. You can:
- Process first payment via Stripe portal
- Accept later payments in cash or check
- Manually mark subsequent invoices as paid
- Mix and match payment methods per job

#### "What if a client disputes a charge?"

Credit card disputes (chargebacks) are rare but can happen:

**If you receive a dispute:**
1. Stripe notifies you via email
2. You have 7-10 days to respond
3. Provide evidence: signed contract, email communications, proof of services
4. Stripe reviews and makes a decision

**With ShootPath:**
- You have a signed contract as proof
- Email logs show communications
- Much stronger case than businesses without contracts

Most disputes are resolved in your favor if you have proper documentation!

#### "Can I offer payment plans beyond the standard schedule?"

Yes! You can create custom payment schedules:
- Weekly payments for mini sessions
- Monthly payments for weddings booked a year out
- Flexible schedules for clients with budget constraints

Just edit the payment schedule in the job details and the invoice will update!

#### "What happens if I need to refund after delivering photos?"

**If services were completed:**
- Refunds are at your discretion
- Check your contract's refund policy
- Issue refunds through Stripe dashboard
- ShootPath updates invoice status automatically

**If services weren't completed:**
- Refer to cancellation policy in contract
- Refund appropriate amount per policy
- Document everything for your records

#### "Can clients pay more than what's due?"

Technically yes, but it's uncommon. If a client wants to pay ahead:
- They can submit the next scheduled payment early
- Or pay the full balance upfront
- ShootPath records overpayments and applies them to future invoices

Most photographers don't encourage this (cash flow is better when payments are spread out), but it's possible!

### What's Next?

Now that you understand client payments, explore other portal features:

**Contract Signing** - [Learn how clients sign contracts before paying](./contract-signing)

**Portal Access** - [Understand portal tokens and security](./portal-access)

**Quote Acceptance** - [See how clients accept quotes](./quote-acceptance)

**Questionnaires** - [Learn about questionnaires in the portal](./questionnaires)

---

**Questions?** Look for the help links throughout ShootPath, or reach out to support if you need a hand!
