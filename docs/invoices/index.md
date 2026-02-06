---
sidebar_position: 1
---

# Invoices Overview

## Quick Reference

Invoices are your payment requests that collect money from clients based on your payment schedule. They're automatically generated when a quote is accepted, or you can create them manually for additional charges.

**What is an Invoice?**
- Payment request tied to a specific job
- Shows amount due, due date, and payment link
- Sent automatically when payment schedule triggers
- Client pays securely via Stripe credit card processing
- Tracks payment status (pending, paid, overdue)

**Invoice Lifecycle:**
1. **Created** - Invoice generated from payment schedule or created manually
2. **Sent** - Client receives email with secure payment link
3. **Viewed** - Client opens the invoice (you get notified)
4. **Paid** - Client submits payment via Stripe
5. **Recorded** - Payment tracked in job history

**Common Invoice Types:**
- **Deposit Invoice** - Secures the booking (typically 25-50% of total)
- **Balance Invoice** - Final payment before service or delivery
- **Installment Invoice** - One of multiple scheduled payments
- **Custom Invoice** - Additional charges (travel fees, extra hours, rush delivery)

**Next Steps:** Learn about [payment schedules](./payment-schedules) to understand how invoices are created automatically, or jump to [creating invoices](./creating-invoices) to add custom charges.

---

## Detailed Guide

### What Are Invoices in ShootPath?

An invoice is a formal payment request that tells a client exactly how much they owe and when it's due. Unlike quotes (which are proposals), invoices are commitments based on signed agreements.

**Think of invoices as your "it's time to pay" notices.** They:
- Reference the signed contract and accepted quote
- Specify the exact amount due
- Include a secure payment link
- Show the due date clearly
- Track whether payment has been received

When a client accepts a quote in ShootPath, the system automatically creates invoices based on your payment schedule. If your payment schedule says "50% deposit at booking, 50% balance two weeks before the session," ShootPath creates two invoices with those amounts and due dates. No manual work required!

### Why Proper Invoicing Matters

**From a Client's Perspective:**

Clients appreciate clear, professional invoices because:
- **No confusion** - They know exactly what they owe and when
- **Easy payment** - One-click payment links (no writing checks or finding Venmo)
- **Automatic receipts** - Instant confirmation when payment processes
- **Payment history** - They can see what they've paid and what's still due

**From Your Business Perspective:**

Professional invoicing helps you:
- **Get paid faster** - Clear due dates and payment links remove friction
- **Track cash flow** - Know exactly who owes what and when
- **Reduce no-shows** - Deposits secure bookings and demonstrate commitment
- **Stay organized** - All payment records in one place
- **Avoid disputes** - Written record of what was agreed upon

**Real-world impact:** Photographers who use automated invoicing with clear payment schedules collect payments 40% faster on average than those who send informal payment requests or wait for clients to ask "how do I pay?"

### How Invoices Work in ShootPath

#### Automatic Invoice Generation

When a client accepts a quote, ShootPath looks at your payment schedule and creates invoices automatically:

**Example: Wedding Package with 50/50 Split**

Quote accepted January 1st for a May 15th wedding with payment schedule:
- 50% deposit due at booking
- 50% balance due April 1st (6 weeks before wedding)

**What happens automatically:**
1. **Deposit invoice created** - $2,500 due January 1st
2. **Client receives email** - "Your deposit payment is ready"
3. **Balance invoice created** - $2,500 due April 1st (but marked as "future")
4. **Reminder sent** - Client gets email March 25th: "Balance due soon"
5. **Due date arrives** - April 1st, invoice status changes to "Due Now"

You don't create these invoices manually or send reminder emails manually - ShootPath handles it based on the payment schedule you configured!

#### Manual Invoice Creation

Sometimes you need to charge for something outside the original quote:

**Common scenarios:**
- Client books 3 hours but session runs to 5 hours (extra time)
- Location changes from 20 miles away to 100 miles away (travel fee)
- Client requests gallery delivery in 1 week instead of 4 weeks (rush fee)
- Client wants printed album that wasn't in original package (add-on product)
- Replacement fee for lost or damaged equipment at event

For these situations, you create a manual invoice with the amount, description, and due date. The invoice works exactly the same as automatic ones - the client receives an email with a payment link and you track the status.

### Invoice Status Flow

Every invoice moves through these statuses:

#### Future
**What it means:** Payment isn't due yet. The invoice exists but the client doesn't need to worry about it right now.

**Example:** You're shooting a wedding on June 1st. The balance is due May 1st. It's currently March - the balance invoice exists but shows as "Future."

**Client experience:** They can see the invoice in their portal, but it says "Due May 1st" - no urgency yet.

**Your view:** You see it listed, but it's grayed out to indicate it's not urgent.

#### Due Soon
**What it means:** Payment is due within 7 days. Time to send a friendly reminder!

**Example:** Balance is due May 1st, it's now April 25th. Invoice status changes to "Due Soon."

**Client experience:** They receive an automatic reminder email: "Your balance payment of $2,500 is due in 6 days."

**Your view:** Invoice highlighted yellow to show it needs attention soon.

#### Due Now
**What it means:** Payment is due today. Client should pay immediately.

**Example:** It's May 1st and the balance is due today.

**Client experience:** Email says "Your payment is due today" with prominent "Pay Now" button.

**Your view:** Invoice highlighted orange - follow up if not paid by end of day.

#### Overdue
**What it means:** Due date has passed without payment. Time to follow up firmly.

**Example:** It's May 5th and the May 1st balance payment still hasn't been received.

**Client experience:** Email says "Your payment is overdue" - more urgent tone.

**Your view:** Invoice highlighted red. You should contact the client immediately.

#### Paid
**What it means:** Payment received! Money is on its way to your bank account.

**Example:** Client paid the $2,500 balance on April 30th.

**Client experience:** They receive instant receipt via email showing payment confirmation.

**Your view:** Invoice shows green checkmark, payment date, and transaction details. Funds arrive in your bank in 2-3 business days.

#### Partially Paid
**What it means:** Some payment received, but full amount still owed.

**Example:** Client owes $3,000 but only paid $1,000. (This usually happens when you manually record a partial payment or apply a partial refund.)

**Client experience:** They see remaining balance due with updated amount.

**Your view:** Shows $1,000 paid, $2,000 still owed.

:::tip Status Changes Happen Automatically
You don't have to manually change invoice statuses. ShootPath updates them based on due dates and payment events. Your job is just to follow up when you see "Due Now" or "Overdue" statuses!
:::

### Understanding Automatic vs. Manual Invoices

ShootPath handles two types of invoices differently:

#### Automatic Invoices (From Payment Schedule)

**Created when:** Quote is accepted and converted to job

**Based on:** Payment schedule attached to the quote/package

**Examples:**
- Deposit invoice (50% of total due at booking)
- Balance invoice (remaining 50% due 2 weeks before session)
- Installment 1, 2, 3 for multi-payment plans

**How they work:**
1. Quote accepted → Job created
2. Payment schedule analyzed
3. Invoice(s) created with amounts and due dates from schedule
4. Reminders sent automatically based on due dates
5. You don't do anything - it's all automatic!

**Can you edit them?**
Yes, you can adjust amounts or due dates if needed. Common reasons:
- Client negotiated a discount
- You're offering a payment plan extension
- Session date moved, so payment dates need to shift

#### Manual Invoices (Custom Charges)

**Created when:** You need to charge for something outside the original quote

**Based on:** You decide the amount, description, and due date

**Examples:**
- Extra hours: $300 × 2 hours = $600
- Travel fee: Changed location adds $200
- Rush delivery: $500 for 1-week turnaround
- Physical product: Client wants a $400 album not in original package

**How they work:**
1. You click "Add Invoice" in the job
2. Enter amount, description, due date
3. Invoice created and sent to client
4. Works exactly like automatic invoices from there

**When to use them:**
- Any charge not in the original quote
- Flexible payment arrangements (client needs to split a payment)
- Refunds or credits (create negative invoice to adjust balance)

### Invoice Components

Every invoice includes these elements:

#### Invoice Number
Unique identifier for tracking and bookkeeping. Format: `INV-{jobId}-{sequenceNumber}`

Example: `INV-5234-01` (first invoice for job #5234)

#### Amount Due
The exact payment amount in dollars and cents.

**Displayed as:** $2,500.00 (not "around $2,500" or "$2.5k")

**Calculated from:**
- Payment schedule percentage × job total
- OR custom amount you entered
- Minus any discounts or credits applied

#### Due Date
The date by which payment should be received.

**Common due dates:**
- "Due upon receipt" (deposit invoices)
- "Due [date]" (specific calendar date)
- "Due X days before session/event"

**Best practices:**
- Give clients at least 3-5 days notice for large amounts
- Don't make final payment due the day of the session (awkward!)
- For weddings, final payment typically due 2-4 weeks before event

#### Description
What the payment is for.

**Good descriptions:**
- "Deposit for Wedding Photography Services - May 15, 2026"
- "Balance Payment - Portrait Session"
- "Additional 2 Hours Coverage at Reception"

**Bad descriptions:**
- "Payment" (too vague)
- "Money owed" (unprofessional)
- Blank (confusing for client and your bookkeeping)

#### Payment Link
Unique, secure URL that takes the client to the Stripe payment page.

**How it works:**
- Link embedded in email client receives
- Can be copied and sent via text/DM if needed
- Remains active until invoice is paid
- Links to client's portal showing invoice details

**Security:**
- Each link is unique and tied to that specific invoice
- Contains a secure token that can't be guessed
- Only accessible by someone with the link (no public indexing)

#### Payment Status
Current state of the invoice (Future, Due Soon, Due Now, Overdue, Paid).

**Displayed prominently** so both you and the client know where things stand at a glance.

### The Payment Collection Process

Let's walk through a typical invoice payment flow from creation to completion:

#### Step 1: Invoice Created

**Trigger:** Quote accepted OR you create manual invoice

**What happens:**
- Invoice record created in ShootPath
- Amount, due date, and description set
- Status set based on due date (Future if not due yet, Due Now if due immediately)

**Your role:** Review to ensure accuracy before sending

#### Step 2: Invoice Sent

**Trigger:** You click "Send Invoice" OR automatic email scheduled

**What happens:**
- Client receives email with subject: "Invoice from [Your Business Name]"
- Email includes invoice details and "View Invoice" button
- Invoice marked as "Sent" in your system

**Client receives:**
```
Hi Sarah,

Your invoice for Portrait Session is ready.

Amount: $750.00
Due: April 15, 2026

[View Invoice and Pay]

Questions? Reply to this email!

[Your Business Name]
```

#### Step 3: Client Views Invoice

**Trigger:** Client clicks "View Invoice" link in email

**What happens:**
- Opens their portal (no login required - link contains secure token)
- Shows invoice details, due date, and "Pay Now" button
- You receive notification that they viewed it

**What client sees:**
- Invoice number and description
- Amount due and due date
- Job details (session type, date)
- Payment history (if they've made payments already)
- Big "Pay Now" button

#### Step 4: Client Pays

**Trigger:** Client clicks "Pay Now"

**What happens:**
- Redirects to Stripe-hosted payment page
- Client enters credit card details
- Stripe processes payment (takes 2-3 seconds)
- Success! Money is on the way to your account

**What client experiences:**
```
Pay Invoice - INV-5234-01
Amount: $750.00

Card Number: [____-____-____-____]
Expiration: [MM/YY]
CVC: [___]

[Submit Payment]

🔒 Secured by Stripe
```

**Security note:** Client never sees your merchant account details, and you never see their full card number. Stripe handles everything securely!

#### Step 5: Payment Confirmed

**Trigger:** Stripe successfully processes the payment

**What happens:**
- Client receives instant email receipt
- You receive notification: "Sarah paid $750 for Portrait Session"
- Invoice status changes to "Paid"
- Payment recorded in job history
- Funds deposited to your bank in 2-3 business days

**Client receives:**
```
Payment Received - $750.00

Thank you for your payment!

Invoice: INV-5234-01
Amount: $750.00
Paid: April 12, 2026 at 3:42 PM
Card ending in: 4242

[Download Receipt]
```

**You see:**
- Green checkmark on invoice
- Payment date and time
- Last 4 digits of card used
- Stripe transaction ID
- Expected deposit date

### Multiple Due Payments: The Forced Payment Rule

Here's an important rule in ShootPath: **If multiple payments are due or overdue at the same time, clients must pay ALL due amounts together.**

#### Why This Rule Exists

Without it, clients could cherry-pick which invoices to pay, creating confusion:
- "I paid the balance but not the deposit" (backwards!)
- "I paid invoice #2 but skipped invoice #1" (out of order)
- "I paid half of each invoice" (partial payments everywhere)

The forced payment rule keeps things simple and clear: pay everything that's currently due, then you're all caught up.

#### How It Works

**Example Scenario:**

Sarah has a wedding package with three invoices:
1. Retainer: $1,500 due January 5 (**OVERDUE** - it's now January 10)
2. Payment 2: $1,500 due January 10 (**DUE TODAY**)
3. Final: $2,000 due March 15 (Future - not due yet)

**What Sarah sees in her portal:**

```
Total Due Now: $3,000

Pay All Due Invoices
- Retainer: $1,500 (overdue)
- Payment 2: $1,500 (due today)

[Pay $3,000 Now]
```

She CANNOT:
- Pay just the retainer ($1,500)
- Pay just payment 2 ($1,500)
- Pay some other amount

She MUST:
- Pay both together ($3,000 total)

**After she pays:** Her account is current. The future payment ($2,000 due March 15) can be paid individually when it comes due.

#### When Multiple Payments Bundle

Payments bundle together when:
- Due date is today or earlier
- Status is "Due Now" or "Overdue"

Payments DO NOT bundle when:
- Status is "Future" (not due yet)
- Already paid
- Client is current on all previous payments

**Example of NO bundling:**

John has these invoices:
1. Deposit: $500 (PAID January 5)
2. Balance: $500 due February 1 (DUE TODAY - it's February 1)

John sees: "Pay $500" for the balance only. The deposit is already paid, so it doesn't bundle.

**Why clients appreciate this:**

It simplifies decision-making! Instead of "Which should I pay first?" they just see "Here's what you owe right now" with one button. Done.

:::tip Communicating This to Clients
If a client asks "Can I just pay the deposit first?", explain: "To keep payments organized, the system asks you to pay all current amounts together. Once you're caught up, you can pay future invoices individually as they come due!"
:::

### Invoice Best Practices

#### Set Realistic Due Dates

**DON'T:**
- Balance due the day of the session (awkward!)
- Balance due same day as session (what if payment fails?)
- Final payment due the day you deliver gallery (you lose leverage!)

**DO:**
- Balance due 1-2 weeks BEFORE session (gives you buffer if payment fails)
- Final payment due before delivery (maintain leverage)
- Build in grace period for payment processing time

**Example - Wedding Photography:**
- Deposit: Due at booking (secures date)
- Payment 2: Due 3 months before wedding (checks client is still engaged)
- Final: Due 2 weeks before wedding (fully paid before the big day)

#### Send Invoices Promptly

The longer you delay sending an invoice, the longer you wait to get paid!

**Timing matters:**
- Send deposit invoice within 24 hours of quote acceptance
- Send balance reminders 7-10 days before due date
- Send overdue notices within 24 hours of missed due date

**Pro tip:** ShootPath can automate all of this for you! Set up automatic invoice emails and reminders so you never have to think about it.

#### Include Clear Descriptions

Help clients understand what they're paying for:

**Vague:**
- "Payment"
- "Invoice #2"
- "Balance due"

**Clear:**
- "Deposit - Wedding Photography Package - June 15, 2026"
- "Balance Payment - Family Portrait Session"
- "Final Payment - 8-Hour Wedding Coverage + Engagement Session"

#### Track Payment Status Daily

Make it a habit to review your invoice dashboard every morning:

**Check for:**
- Overdue payments (follow up immediately)
- Payments due today (send friendly reminder)
- Payments due in next 7 days (make sure client has payment link)

**Takes 2 minutes, prevents problems!**

#### Follow Up on Overdue Invoices

Don't let overdue invoices sit! Follow up quickly but professionally:

**Day 1 (due date):**
"Hi Sarah! Just a reminder that your balance payment of $1,500 is due today. Here's the payment link: [link]. Let me know if you have any questions!"

**Day 3 (3 days overdue):**
"Hi Sarah, following up on the payment that was due on [date]. I need to receive this before we can proceed with the session. Can you let me know when I can expect payment?"

**Day 7 (1 week overdue):**
"Sarah, your payment is now 7 days overdue. Per our contract, payment is required before the session. Please submit payment by [date] or we'll need to reschedule."

**Day 14+ (2 weeks overdue):**
Enforce contract terms - reschedule session, hold gallery delivery, charge late fees (if contract allows), or consider canceling booking.

#### Record Non-Stripe Payments

If clients pay outside Stripe (cash, check, Venmo, Zelle), record it in ShootPath:

1. Find the invoice
2. Click "Record Payment"
3. Select payment method
4. Enter amount and date
5. Add notes if needed

This keeps your records accurate and shows the invoice as paid.

### Common Invoicing Scenarios

#### Scenario 1: Client Needs a Payment Plan

**Situation:** Client can't afford $3,000 deposit, asks to split it into $1,000 × 3 payments.

**Solution:**
1. Agree on new payment structure
2. Edit original deposit invoice to $1,000
3. Create two manual invoices for $1,000 each with staggered due dates
4. Send payment plan confirmation email

**Contract consideration:** Make sure your contract allows payment plan modifications, or create an addendum!

#### Scenario 2: Session Runs Over Time

**Situation:** You booked 3 hours but session went 5 hours. Contract says additional hours are $300/hour.

**Solution:**
1. Discuss with client before leaving: "We're over time - I'll send an invoice for the extra 2 hours per our contract"
2. Create manual invoice: "Additional 2 Hours - Session Extension" for $600
3. Set due date (1 week is reasonable)
4. Send invoice with friendly note explaining the charge

**Pro tip:** Most clients won't mind if you communicated clearly upfront and provided great service!

#### Scenario 3: Client Wants to Prepay Everything

**Situation:** Client asks "Can I just pay the full amount now instead of waiting for payment schedule?"

**Solution:**
- Absolutely! This is great for cash flow.
- Client can pay multiple invoices at once if they're all marked "due"
- OR you can create one consolidated invoice for the full amount and void the scheduled ones

**How to handle:**
"Sure! I can send you a link to pay the full $5,000 now if you prefer. It'll mark all your scheduled invoices as paid."

#### Scenario 4: Client Requests a Refund

**Situation:** Client cancels 2 months before wedding. Contract says deposit is non-refundable, but you're being nice and offering 50% back.

**Solution:**
1. Find the paid deposit invoice ($1,500)
2. Click "Refund"
3. Select "Partial Refund"
4. Enter $750 (50%)
5. Add note: "Cancellation per contract - partial refund offered as courtesy"
6. Process refund (appears in client's account in 5-10 days)

**Bookkeeping:** Original invoice shows $1,500 paid, $750 refunded, net $750 retained.

#### Scenario 5: Payment Fails

**Situation:** Client tries to pay $2,500 balance, but card is declined.

**What happens:**
- Stripe declines the transaction
- Client sees error message: "Payment failed - please check card details"
- Invoice remains unpaid
- You receive notification: "Payment failed for [Client Name]"

**Your response:**
"Hi Sarah, I noticed the payment didn't go through. This usually means the card was declined or there was a technical issue. Can you try again or use a different card? Let me know if you need help!"

**Common reasons for decline:**
- Insufficient funds
- Expired card
- Incorrect card details entered
- Bank fraud protection (client needs to call bank)
- International card (some banks block international transactions)

### Invoice Reports and Tracking

ShootPath provides several ways to track invoices:

#### Invoice Dashboard

**What you see:**
- All invoices across all jobs
- Filter by status (overdue, due soon, paid, etc.)
- Sort by due date, amount, or client
- Quick actions (send reminder, view details, record payment)

**Use it for:**
- Daily payment tracking
- Following up on overdue amounts
- Cash flow forecasting

#### Job-Level Invoice View

**What you see:**
- All invoices for a specific job
- Payment schedule timeline
- Total collected vs. total owed
- Payment history with dates

**Use it for:**
- Client conversations (what have they paid? what's due?)
- Preparing for upcoming sessions (are they current?)
- End-of-job review (final amounts collected)

#### Financial Reports

**Available reports:**
- Revenue by month (total invoices paid)
- Outstanding invoices (money you're waiting on)
- Payment method breakdown (card vs. cash vs. check)
- Client payment history (who pays on time vs. late)

**Use them for:**
- Tax preparation
- Business planning
- Cash flow management
- Identifying payment trends

### What's Next?

Now that you understand invoice basics, dive deeper into specific topics:

**Want to automate your payment collection?** → [Payment Schedules](./payment-schedules) explains how to set up automatic invoicing based on deposits, balances, and installments.

**Need to create a one-off invoice?** → [Creating Invoices](./creating-invoices) walks through manual invoice creation for custom charges.

**Ready to track who's paid and who hasn't?** → [Tracking Payments](./tracking-payments) covers the payment dashboard, status tracking, and follow-up strategies.

**Curious about how Stripe works?** → [Stripe Integration](./stripe-integration) explains payment processing, fees, security, and the client checkout experience.

---

**Questions?** Look for the help links throughout ShootPath, or reach out to support if you need help!
