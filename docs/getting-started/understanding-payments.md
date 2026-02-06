# Understanding Payments

## Quick Reference

Payment schedules in ShootPath help you collect deposits, balances, and custom payment plans from your clients throughout the booking process.

**What is a Payment Schedule?**
- Structured plan for collecting money from clients
- Set up when creating a quote (before booking is confirmed)
- Common structures: 50/50 split, retainer + balance, full upfront
- Managed automatically by ShootPath via Stripe integration

**Payment Flow:**
1. **Schedule Created** - Define payment amounts and due dates in the quote
2. **Contract Signed** - Client must sign before they can pay (protects both parties)
3. **Payment Link Sent** - Client receives secure link to pay via credit card
4. **Payment Processed** - Stripe handles the transaction, funds deposited to your account
5. **Job Progresses** - Once payments are received, work continues toward delivery

**Why Payment Schedules Matter:**
- Collect deposits to secure bookings and protect your time
- Manage cash flow (don't wait until after delivery to get paid!)
- Split large amounts into manageable chunks for clients
- Track what's paid vs. what's due at a glance

**Next Steps:** [Learn about Stripe integration](#) or [explore contract requirements](./understanding-contracts).

---

## Detailed Guide

### What is a Payment Schedule?

A payment schedule is your plan for collecting money from a client. Instead of just "pay $3,000 when you book," you define exactly when payments happen and how much each one should be.

**Why use payment schedules instead of a single payment?**

**1. Cash Flow**
Waiting until after a wedding to collect $5,000 means you've fronted costs for 6+ months. Payment schedules let you collect deposits upfront and final payments before delivery.

**2. Client Commitment**
A non-refundable deposit ensures the client is serious. It protects your time - you've blocked out your calendar for them, turned away other inquiries, and started planning.

**3. Risk Management**
If a client ghosts after the shoot, at least you've collected a deposit. If you haven't been paid anything, you're out all that time and effort.

**4. Affordability**
Large amounts can be intimidating. Breaking a $4,000 wedding package into $2,000 deposit + $2,000 final payment feels more manageable for clients.

**Real-world example:** Emma books a newborn session for $800. Your payment schedule is 50% ($400) deposit to book, 50% ($400) due before the session. Emma pays the deposit when she signs the contract, securing your time. Two weeks before the session, she pays the final $400. You show up to the shoot knowing you've been fully paid - no awkward "so about payment..." conversations!

### Common Payment Structures

Different photography niches use different payment schedules. Here are the most popular:

#### 50/50 Split
**Structure:** 50% deposit to book, 50% balance before session/delivery

**Best for:**
- Portrait sessions
- Family photos
- Senior portraits
- Engagement sessions

**Why it works:** Simple and fair. Client pays half upfront to secure the booking, half before you deliver. Easy to understand and easy to communicate.

**Example:** $1,500 portrait session
- Deposit: $750 (due when contract is signed)
- Balance: $750 (due 1 week before session)

#### Retainer + Balance
**Structure:** Fixed retainer to book, remainder before session/delivery

**Best for:**
- Weddings (where total cost is high)
- Multi-day events
- Destination shoots

**Why it works:** A flat retainer amount (like $1,000 or $1,500) is easier to budget for than "50% of whatever the total is." It also protects you if the client upgrades their package later - the retainer stays fixed, only the balance changes.

**Example:** $5,000 wedding package
- Retainer: $1,500 (due when contract is signed)
- Balance: $3,500 (due 2 weeks before wedding)

:::tip Pro Tip
For weddings, many photographers collect the final balance 2-4 weeks BEFORE the wedding day. This ensures you're fully paid before the big day, so you can focus on photography instead of worrying about collecting money.
:::

#### Full Payment Upfront
**Structure:** 100% due when booking

**Best for:**
- Mini sessions (lower price point)
- Events (corporate, parties)
- Last-minute bookings

**Why it works:** For shorter, simpler shoots or lower prices, collecting everything upfront is easiest. No need to chase down a second payment for a $300 mini session.

**Example:** $250 mini session
- Full payment: $250 (due when contract is signed)
- No balance due later

#### Custom Multi-Payment Plans
**Structure:** 3+ payments spread over time

**Best for:**
- High-value packages ($5k+)
- Long booking windows (6-12 months out)
- Clients who request payment plans

**Why it works:** Spreading a $10,000 wedding package across 4-5 payments over 10 months makes it more affordable for clients. You get steady cash flow throughout the engagement.

**Example:** $8,000 wedding package (booked 9 months out)
- Retainer: $2,000 (due at booking)
- Payment 2: $2,000 (due 6 months before wedding)
- Payment 3: $2,000 (due 3 months before wedding)
- Final: $2,000 (due 2 weeks before wedding)

:::warning Payment Plan Considerations
Custom payment plans are great for affordability, but they require more management. Make sure your contract states what happens if a client misses a payment! Most photographers require all payments to be current before the session/delivery.
:::

### When Payments Are Due vs. When They're Collected

This trips up new photographers! Understanding the difference is important:

#### Due Date
The date by which a payment SHOULD be made, according to your schedule. This is when you WANT the money.

#### Collection Date
The date the client ACTUALLY pays. Could be on the due date, before it, or after it (ugh).

**Example:**
- Deposit due: January 15
- Client pays: January 12 (early - great!)
- Balance due: March 1
- Client pays: March 8 (late - not ideal)

**What ShootPath shows you:**
- Upcoming: Due date is in the future
- Due: Due date is today
- Overdue: Due date has passed and payment not received
- Paid: Payment received (shows the actual payment date)

You set the due dates when creating the quote. ShootPath tracks them and reminds clients when payments are coming up.

### The Forced Payment Rule

Here's an important rule in ShootPath: **If multiple payments are overdue or due now, clients must pay ALL due amounts together.**

**Why this rule exists:**
Without it, clients might cherry-pick which invoices to pay, leaving you with partial payment and confusion about what's owed. The forced payment rule keeps things clean and clear.

**Example scenario:**

Sarah has a wedding package with these payments:
- Retainer: $1,500 (due Jan 5 - **OVERDUE**)
- Balance: $1,500 (due Jan 10 - **DUE TODAY**)

When Sarah logs into her payment portal, she sees:
"**Total Due: $3,000**" with one "Pay Now" button for both invoices combined.

She CANNOT pay just the retainer or just the balance. She must pay both ($3,000 total) to bring her account current.

**Once she's current:**
Future payments can be paid individually. If there's a third payment due next month, she can pay that one by itself when it comes due.

**Why clients appreciate this:**
It actually simplifies things! They don't have to think about which invoice to pay first or worry about paying them out of order. One button, all current amounts, done.

:::tip Payment Grace Periods
Some photographers give a 3-5 day grace period before marking payments "overdue." You can send a friendly reminder on the due date: "Your final payment is due today! Here's the link..." before sending a more urgent "Your payment is overdue" follow-up.
:::

### Stripe Integration Basics

ShootPath uses Stripe to process payments. Here's what you need to know:

#### Setting Up Stripe
1. Go to Settings > Integrations > Stripe
2. Click "Connect Stripe Account"
3. Follow the prompts to create or connect your Stripe account
4. Complete Stripe's verification (bank details, tax info, identity verification)
5. You're ready to accept payments!

**Stripe fees:** 2.9% + $0.30 per transaction (standard for credit card processing)

**Example:** Client pays $1,000
- Stripe fee: $29.30
- You receive: $970.70
- Funds deposited to your bank in 2-3 business days

#### What Stripe Handles
- **Payment processing** - Securely collects credit card info
- **PCI compliance** - You never touch card numbers (major security win!)
- **Fraud detection** - Flags suspicious transactions
- **Automatic receipts** - Clients get email confirmation instantly
- **Refunds** - Process through ShootPath or Stripe dashboard

#### Client Payment Experience
When a client pays:
1. Receives email with "Pay Your Invoice" link
2. Clicks link to secure payment page
3. Enters credit card details (or uses saved card)
4. Submits payment
5. Gets instant email receipt
6. Payment shows as "Paid" in ShootPath

No accounts to create, no complicated checkout process. Just click, pay, done.

:::tip Payment Links
Each invoice has a unique payment link. You can copy this link and send it via text, email, or DM if clients have trouble finding the original email. The link stays active until the invoice is paid.
:::

### Payment Tracking in Jobs

Once a job is created, the job page shows all payments at a glance:

#### Invoices Section
You'll see:
- **Deposit invoice** - Status (paid/unpaid), amount, due date
- **Balance invoice** - Status (paid/unpaid), amount, due date
- **Custom invoices** - Any additional payments you've added

#### Status Colors
- **Green** - Paid (hooray!)
- **Yellow** - Due today or soon
- **Red** - Overdue (time to follow up)
- **Gray** - Future payment (not due yet)

#### Payment Actions
For each unpaid invoice:
- **Copy Payment Link** - Send to client via text or email
- **Send Reminder** - Automated reminder email to client
- **Mark as Paid** - If they paid outside Stripe (cash/check/Venmo)
- **Adjust Amount** - If you need to add a discount or fee

#### Payment History
See exactly when each payment was received:
- Deposit: $1,000 paid Jan 5, 2026 at 3:42 PM
- Balance: $1,000 paid Feb 10, 2026 at 11:23 AM

This history is invaluable for bookkeeping and client records.

### Payment Schedule Examples by Job Type

Let's look at real-world payment schedules for different photography niches:

#### Wedding Photography ($5,000 package)
**Option 1 - Simple Split:**
- Retainer: $2,000 (due at booking)
- Balance: $3,000 (due 2 weeks before wedding)

**Option 2 - Multi-Payment:**
- Retainer: $1,500 (due at booking)
- Payment 2: $1,500 (due 3 months before wedding)
- Final: $2,000 (due 2 weeks before wedding)

**Why this works:** Spreads cost for clients, gives you steady cash flow, final payment collected before the big day.

#### Portrait Session ($1,200 package)
**Standard 50/50:**
- Deposit: $600 (due at booking)
- Balance: $600 (due 1 week before session)

**Why this works:** Simple, easy to explain, final payment collected before you show up with your gear.

#### Newborn Session ($800 package)
**Option 1 - 50/50:**
- Deposit: $400 (due at booking)
- Balance: $400 (due at session)

**Option 2 - Full Upfront:**
- Full payment: $800 (due at booking)
- Nothing due later

**Why this works:** Newborn timing is unpredictable (baby arrives 2 weeks late, etc.). Collecting full payment upfront means you don't chase down new parents for money!

#### Mini Session ($300 package)
**Full Payment:**
- Full payment: $300 (due at booking)

**Why this works:** Lower price point, short timeline. Collect everything upfront and move on to shooting!

#### Commercial/Brand Shoot ($3,000 project)
**Net 30 Terms:**
- Invoice sent after shoot completion
- Payment due 30 days from invoice date

**OR Deposit + Net 30:**
- Deposit: $1,000 (due at booking)
- Balance: $2,000 (due 30 days after shoot)

**Why this works:** Commercial clients often expect NET 30 (pay within 30 days), but a deposit protects your time in case they cancel.

:::tip Adjust for Your Market
These are guidelines, not rules! Survey other photographers in your area to see what payment structures are standard. Match or slightly improve on the norm to stay competitive.
:::

### Contract-Before-Payment Rule

In ShootPath, **clients cannot pay until they sign the contract.** This is a critical protection for your business.

**Why this rule exists:**

**1. Legal Protection**
The contract outlines terms, cancellation policy, usage rights, and delivery timeline. If a client pays before signing, they might argue later "I didn't agree to those terms!" With the contract signed first, you have proof they read and agreed.

**2. Informed Consent**
Clients should understand what they're paying for before handing over money. The contract makes everything explicit - no surprises, no confusion.

**3. Professional Standards**
Requiring contract signature before payment is standard business practice. It signals "I run a professional operation" and builds client trust.

**The flow:**
1. Client accepts quote
2. Contract generated and sent
3. Client reviews and signs contract
4. Payment button becomes active
5. Client can now pay

If they try to pay before signing, ShootPath redirects them to the contract page with a message: "Please sign the contract before making payment."

**Can you disable this?**
Technically yes, but we strongly recommend against it. Collecting payment before a signed contract puts you at legal risk and opens the door for disputes.

:::warning Don't Skip the Contract
Even for small shoots or clients you know personally, require a signed contract before payment. It's not about lack of trust - it's about running a professional business that protects everyone involved.
:::

### What Happens if a Client Doesn't Pay?

Despite your best efforts, sometimes clients don't pay on time (or at all). Here's how to handle it:

#### Step 1: Send a Friendly Reminder (Due Date)
"Hi Sarah! Just a reminder that your final payment of $1,000 is due today. Here's the payment link: [link]. Let me know if you have any questions!"

#### Step 2: Follow Up (3-5 Days Overdue)
"Hi Sarah, I wanted to follow up on the final payment that was due on [date]. I need to receive this before we can proceed with the session/gallery delivery. Can you let me know when I can expect payment?"

#### Step 3: Firm Reminder (1 Week Overdue)
"Sarah, your payment is now 7 days overdue. Per the contract you signed, full payment is required before [session/delivery]. Please submit payment by [date] or we'll need to reschedule."

#### Step 4: Enforce Contract Terms (2+ Weeks Overdue)
At this point, refer to your contract:
- Reschedule the session until payment is received
- Hold gallery delivery until final payment is made
- Charge late fees (if specified in contract)
- Consider canceling the booking and keeping the deposit (extreme cases)

**Document everything:** Save all communication about late payment. If you ever need to take legal action or dispute a chargeback, this documentation is essential.

:::tip Prevention is Key
Most late payments happen because:
1. Client forgot (set up automatic reminders!)
2. Payment link got buried in email (resend it)
3. Financial situation changed (discuss payment plans)
4. They're avoiding you (red flag - enforce contract terms)

Proactive communication prevents most late payment issues!
:::

### Gallery Delivery & Final Payments

Many photographers tie gallery delivery to final payment. Here's how that works:

**Before Delivery:**
- Client must pay all invoices marked "due before delivery"
- Payment status checked automatically by ShootPath
- If unpaid, gallery download buttons are disabled

**After Payment:**
- Client receives "Your gallery is ready!" email
- Can view, download, share, and order prints
- Access remains active for the duration you've set (30 days, 90 days, forever, etc.)

**Why tie delivery to payment?**
It ensures you're paid for your work before the client has the final product. Once they have all the high-res files, leverage is gone - collecting payment becomes much harder.

**Alternative approach:**
Some photographers deliver the gallery with low-res previews visible, but high-res downloads locked until final payment. This lets clients see the work (builds excitement!) while maintaining leverage for payment collection.

**Your choice:** ShootPath supports both approaches. Choose the one that fits your business philosophy and client relationships.

### Adding Unexpected Costs

Sometimes you need to charge for something that wasn't in the original quote:

**Extra Hours**
Client books 3 hours but the session runs to 5 hours. Your contract states additional hours are $300 each. Add a new invoice for $600.

**Travel Fees**
Client moves the session location from 20 miles away to 100 miles away. Add an invoice for the additional travel fee.

**Rush Delivery**
Client needs the gallery in 1 week instead of 4 weeks. Your rush delivery fee is $500. Add an invoice.

**How to add custom invoices:**
1. Open the job in ShootPath
2. Go to Invoices section
3. Click "Add Invoice"
4. Enter amount, description, due date
5. Send to client

**Communication is key:** Before adding surprise charges, discuss with the client! Explain the situation: "The session went longer than expected, which was great for photos but means I need to charge for the extra time per our contract. I'm adding an invoice for $600 for the 2 extra hours."

Most clients are understanding if you explain charges clearly and reference the contract they signed.

### Refunds & Cancellations

Your contract should define the refund policy, but here are common scenarios:

#### Client Cancels (Before Session)
- **More than 30 days notice:** Refund deposit minus processing fees OR offer to reschedule
- **14-30 days notice:** Forfeit 50% of deposit, refund remainder
- **Less than 14 days notice:** Deposit fully forfeited (you've turned away other clients)

#### Client Cancels (After Session, Before Delivery)
- No refund - work has been completed

#### You Cancel
- Full refund of all payments - you failed to deliver on the contract

#### Weather Cancellation (Outdoor Shoots)
- Reschedule to another date, no refund needed (services will still be provided)

#### No-Show
- Deposit forfeited, balance not owed (since session didn't happen)

**Processing refunds in ShootPath:**
1. Find the payment in job history
2. Click "Refund"
3. Choose full or partial refund
4. Stripe processes the refund (appears in client account in 5-10 business days)

:::warning Refunds & Chargebacks
If a client disputes a charge with their credit card company (chargeback), Stripe will investigate. Your signed contract and communication history are your evidence that the charge was legitimate. This is why documentation matters!
:::

### Tips for Payment Success

**Be Clear from the Start**
State your payment terms clearly in your quote and contract. No surprises = no conflicts.

**Send Payment Links Proactively**
Don't wait for clients to ask. Send the payment link as soon as it's due: "Your final payment is due this week - here's the link!"

**Offer Payment Plans for High-Value Packages**
A $7,000 wedding package is steep. Offering 3-4 payments over 8 months makes it more accessible and increases bookings.

**Set Realistic Due Dates**
Don't make the balance due the day of the session. Give clients at least 1-2 weeks notice so they can plan financially.

**Track Payments in Real Time**
Check your ShootPath dashboard regularly. If a payment is overdue, follow up immediately - the longer you wait, the harder it is to collect.

**Automate Reminders**
ShootPath can send automatic payment reminders (7 days before due, on due date, 3 days overdue). Use them! It saves you from having to remember to follow up manually.

**Accept Multiple Payment Methods**
Stripe handles credit and debit cards. Some photographers also accept Venmo, Zelle, or cash for clients who prefer it (though card payments are easier to track!).

**Thank Clients for Prompt Payment**
A quick "Thank you for the payment! Looking forward to your session!" email builds goodwill and reinforces positive behavior.

### What's Next?

Now that you understand payment schedules, you're ready to manage the financial side of your photography business with confidence!

**Want to learn about contracts?** Read [Understanding Contracts](./understanding-contracts) to see how contracts and payments work together.

**Need to set up Stripe?** Head to Settings > Integrations > Stripe and connect your account.

**Curious about what happens after payments?** Check out [Understanding Jobs](./understanding-jobs) to see the full workflow from booking to delivery.

**Just getting started?** Go back to [Creating a Lead](./creating-a-lead) to build your client pipeline first.

---

**Questions?** Look for the help links throughout ShootPath, or reach out to support if you need help!
