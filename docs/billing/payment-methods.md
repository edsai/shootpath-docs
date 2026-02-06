---
sidebar_position: 3
---

# Payment Methods

## Quick Reference

Managing your payment methods in ShootPath is simple and secure. All billing transactions are processed through Stripe, a leading payment processor trusted by millions of businesses worldwide. Your payment information is encrypted and stored securely, and ShootPath never has direct access to your full credit card details.

**What You'll Learn:**
- How to add and update payment methods
- Managing multiple payment methods
- Handling failed payments
- Viewing and downloading invoices
- Understanding tax information
- Payment security and PCI compliance

**Quick Actions:**
- Add a payment method: **Settings → Billing → Payment Methods → Add Payment Method**
- Update billing address: **Settings → Billing → Payment Methods → Edit**
- Change primary payment method: **Settings → Billing → Payment Methods → Set as Default**
- Download invoice: **Settings → Billing → Invoice History → Download**
- Update tax information: **Settings → Billing → Tax Information**

:::tip Pro Tip
Keep a backup payment method on file to prevent service interruptions if your primary card expires or has insufficient funds. ShootPath will automatically try your backup method if the primary fails.
:::

---

## Detailed Guide

### Adding a Payment Method

To start a paid subscription after your trial or update your existing payment information:

**Step 1: Navigate to Billing Settings**
1. Click your profile picture in the top right
2. Select **Settings**
3. Click **Billing** in the left sidebar
4. Click the **Payment Methods** tab

**Step 2: Add Your Card**
1. Click **Add Payment Method**
2. Enter your card information:
   - Card number (16 digits)
   - Expiration date (MM/YY)
   - CVC security code (3-4 digits on back)
   - Cardholder name (as it appears on card)
3. Enter your billing address:
   - Street address
   - City
   - State/Province
   - ZIP/Postal code
   - Country
4. Check **Set as default** if this should be your primary payment method
5. Click **Save Payment Method**

**Supported Card Types:**
- Visa
- Mastercard
- American Express
- Discover
- Diners Club
- JCB
- UnionPay

**International Cards:**
ShootPath accepts cards from any country. Your card will be charged in USD, and your bank will handle the currency conversion if needed. Note that your bank may charge foreign transaction fees.

**Debit Cards:**
Debit cards with Visa/Mastercard logos work exactly like credit cards. However, be aware that:
- Funds are withdrawn immediately (not at the end of a billing cycle)
- Failed payments due to insufficient funds may result in overdraft fees from your bank
- Some banks block international transactions by default (call your bank to enable)

### Managing Multiple Payment Methods

You can add multiple payment methods to your account for flexibility and redundancy.

**Why Add Multiple Methods:**
- **Backup for failures:** If your primary card is declined, ShootPath automatically charges the backup
- **Different cards for different purposes:** Use a business card for subscription, personal card as backup
- **Expiration management:** Add a new card before the old one expires
- **Team flexibility:** Let billing admin use their preferred card

**Setting Your Default Method:**
1. Go to **Settings → Billing → Payment Methods**
2. Find the card you want to set as default
3. Click **Set as Default** next to that card
4. The default card will be used for all future charges

**Removing a Payment Method:**
1. Go to **Settings → Billing → Payment Methods**
2. Find the card you want to remove
3. Click **Remove** next to that card
4. Confirm the removal

:::warning Cannot Remove Default Method
You cannot remove your default payment method if you have an active subscription. First set a different card as default, then remove the old one.
:::

### Updating Billing Information

**When to Update:**
- Your card expires or is replaced
- Your billing address changes
- Your company name or tax ID changes
- You want to use a different card

**How to Update Card Details:**
1. Go to **Settings → Billing → Payment Methods**
2. Click **Edit** next to the card you want to update
3. Make your changes (you can update address, name, or replace the entire card)
4. Click **Save Changes**

**Updating Billing Address:**
Your billing address is used for:
- Credit card verification
- Invoice generation
- Tax calculation
- Legal and accounting records

To update your billing address:
1. Go to **Settings → Billing → Payment Methods**
2. Click **Edit** next to your payment method
3. Update the address fields
4. Click **Save Changes**

Your next invoice will reflect the new address. Previous invoices are not changed (they remain as historical records).

**Updating Company Name:**
If your business name changes or you initially entered a personal name instead of your business name:
1. Go to **Settings → Billing → Billing Information**
2. Update the **Company Name** field
3. Click **Save Changes**

This name appears on all invoices. Update it before your next billing cycle to ensure proper invoices for accounting.

### Failed Payments

If ShootPath cannot charge your payment method, we'll send you an email notification and give you time to resolve the issue before suspending your account.

**Common Reasons for Failed Payments:**
- **Insufficient funds** - Not enough balance on the card
- **Expired card** - Card has passed its expiration date
- **Incorrect card details** - Typo in card number or CVC
- **Bank declined** - Bank flagged the transaction as suspicious or exceeded daily limit
- **Invalid billing address** - Address doesn't match what the bank has on file
- **Card reported lost/stolen** - Card was cancelled for security reasons
- **International transaction blocked** - Bank requires authorization for international charges

**What Happens After a Failed Payment:**

**Day 0 (Payment Due Date):**
- First charge attempt fails
- You receive an email notification
- Your account remains active
- ShootPath automatically retries in 3 days

**Day 3:**
- Second charge attempt
- Another email notification if this fails
- Account still active
- Retry scheduled for 7 days later

**Day 10:**
- Final charge attempt
- Final email warning
- If this fails, account is suspended after 24 hours

**Day 11:**
- Account suspended (cannot create new leads, send emails, or access client portal)
- You can still log in and view existing data
- You can update payment method to reactivate

**How to Resolve a Failed Payment:**

**Step 1: Check Your Email**
Look for the failed payment notification from ShootPath. It will specify the reason for the failure if known.

**Step 2: Update Your Payment Method**
1. Go to **Settings → Billing → Payment Methods**
2. Either:
   - Edit your existing payment method to correct the issue
   - Add a new payment method and set it as default
3. Click **Save**

**Step 3: Retry the Payment**
After updating your payment method:
1. Go to **Settings → Billing**
2. You'll see a banner: "Payment failed. Click here to retry."
3. Click **Retry Payment**
4. If successful, your account is immediately reactivated

**Step 4: Contact Your Bank**
If the payment still fails:
- Call your bank to authorize the transaction
- Ask if they're blocking international charges (ShootPath processes through Stripe in the US)
- Verify your daily spending limit hasn't been exceeded
- Confirm the billing address matches what the bank has on file

**Step 5: Contact Support**
If you've tried everything and still can't resolve the issue:
- Email [billing@shootpath.com](mailto:billing@shootpath.com)
- Include: Account email, last 4 digits of card, and error message if any
- We'll work with you to find a solution

:::tip Avoid Service Interruptions
Add a backup payment method before your card expires. ShootPath will automatically charge the backup if the primary fails, preventing any downtime.
:::

### Invoices and Receipts

ShootPath automatically generates an invoice for every payment. These invoices are available in your account and sent to your email address.

**Accessing Your Invoices:**
1. Go to **Settings → Billing**
2. Click the **Invoice History** tab
3. You'll see a list of all invoices with:
   - Invoice number
   - Date
   - Amount charged
   - Payment status
   - Download link

**Downloading Invoices:**
- Click **Download PDF** next to any invoice
- The PDF includes:
  - Your company name and billing address
  - ShootPath's business information
  - Invoice number and date
  - Itemized charges
  - Payment method (last 4 digits)
  - Total amount paid

**Invoice Details:**

Each invoice shows:
- **Invoice Number:** Unique identifier for accounting (format: INV-2025-001234)
- **Issue Date:** When the invoice was generated
- **Due Date:** When payment was due (usually the same as issue date for subscriptions)
- **Billing Period:** The month(s) covered by this payment
- **Line Items:**
  - Subscription plan name
  - Number of users (if applicable)
  - Prorated charges (if plan changed mid-month)
  - Credits applied (if any)
- **Subtotal:** Total before taxes
- **Tax:** Sales tax or VAT (if applicable)
- **Total:** Final amount charged

**Email Receipts:**
After each successful payment, ShootPath sends a receipt email to:
- The account owner's email
- Any additional billing contact emails you've configured (see **Settings → Billing → Billing Contacts**)

The email includes:
- Amount charged
- Date
- Payment method used
- Download link for the full invoice PDF

**Requesting Past Invoices:**
If you need invoices from before you started using ShootPath (for example, during onboarding):
1. Contact [billing@shootpath.com](mailto:billing@shootpath.com)
2. Specify the date range you need
3. We'll email you a ZIP file with all invoices for that period

**Invoice Corrections:**
If you notice an error on an invoice:
1. Email [billing@shootpath.com](mailto:billing@shootpath.com) within 30 days
2. Include the invoice number and description of the error
3. We'll investigate and issue a corrected invoice if needed

Corrected invoices are marked with "Revised" and reference the original invoice number.

### Tax Information

ShootPath collects sales tax or VAT based on your location as required by law.

**Who Pays Tax:**

**United States:**
- Sales tax is collected for customers in states where ShootPath has a tax obligation
- Tax rate is based on your billing address
- Tax-exempt organizations can submit documentation (see below)

**European Union:**
- VAT is collected for all EU customers
- Rate depends on your country
- Businesses with a valid VAT ID are reverse-charged (no tax collected)

**Other Countries:**
- Most countries do not require ShootPath to collect tax
- You may need to self-report and pay tax according to your local laws
- Consult your accountant for guidance

**Adding Your Tax ID:**

If you're a business with a tax exemption number or VAT ID:

1. Go to **Settings → Billing → Tax Information**
2. Enter your tax ID:
   - **US:** Federal EIN or state sales tax exemption certificate number
   - **EU:** VAT number (format: GB123456789)
   - **Other:** Business registration number
3. Upload supporting documentation:
   - US tax-exempt organizations: Upload your 501(c)(3) determination letter or resale certificate
   - EU businesses: Upload VAT registration certificate
4. Click **Submit for Verification**

**Verification Process:**
- ShootPath (via Stripe) verifies tax IDs automatically for most countries
- Verification typically takes 1-3 business days
- You'll receive an email when verification is complete
- Once verified, future invoices will reflect your tax exemption

**If Verification Fails:**
- Check that your tax ID is entered correctly (no spaces or special characters)
- Ensure the billing address matches the address on your tax registration
- Contact [billing@shootpath.com](mailto:billing@shootpath.com) for help

**Correcting Tax Status:**
If you were charged tax but should have been exempt:
1. Add your tax ID and get it verified
2. Email [billing@shootpath.com](mailto:billing@shootpath.com) with:
   - Invoice numbers that should be corrected
   - Your verified tax ID
3. We'll issue a credit for the incorrectly charged tax

Credits are applied to your next invoice. If you've cancelled, we'll process a refund.

### Payment Security

ShootPath takes payment security seriously. Your financial information is protected by multiple layers of security.

**Stripe Integration:**
All payment processing is handled by Stripe, a PCI Level 1 certified payment processor. This is the highest level of security certification in the payments industry, the same level required for Visa and Mastercard.

**What This Means for You:**
- ShootPath never stores your full credit card number
- Card data is encrypted in transit and at rest
- Stripe's infrastructure is monitored 24/7 for security threats
- Regular third-party security audits

**PCI Compliance:**
ShootPath is PCI DSS compliant, meaning we follow strict security standards for handling card data:
- Secure network architecture
- Encrypted data transmission
- Access controls and monitoring
- Regular security testing
- Strict data retention policies

**What You See in ShootPath:**
- Last 4 digits of your card (for identification)
- Card brand (Visa, Mastercard, etc.)
- Expiration date
- Cardholder name
- Billing address

We NEVER display or store:
- Full card number
- CVC security code
- Card magnetic stripe data

**Security Best Practices:**

**Protect Your Account:**
- Use a strong, unique password
- Enable two-factor authentication (Settings → Security)
- Don't share your login credentials
- Log out on shared computers

**Monitor Your Billing:**
- Review invoices monthly
- Check for unauthorized charges
- Update card information promptly when cards are replaced
- Remove old payment methods you're no longer using

**Report Suspicious Activity:**
If you notice any unauthorized charges or suspicious activity:
1. Email [billing@shootpath.com](mailto:billing@shootpath.com) immediately
2. Change your password
3. Review your invoice history for unauthorized charges
4. Contact your bank to dispute fraudulent charges

**Data Breach Notification:**
In the unlikely event of a data breach affecting payment information, ShootPath will:
- Notify affected users within 72 hours
- Provide guidance on protecting your accounts
- Work with Stripe and law enforcement to investigate
- Offer credit monitoring if appropriate

**Questions About Security:**
- Review our [Security & Privacy Policy](https://shootpath.com/privacy)
- View Stripe's security documentation: [stripe.com/security](https://stripe.com/security)
- Contact [security@shootpath.com](mailto:security@shootpath.com) with specific questions

---

## Common Questions

**Can I use PayPal or other payment methods?**
Currently, ShootPath only accepts credit and debit cards through Stripe. We're evaluating additional payment methods based on customer demand. If you'd like to see PayPal, ACH, or other options, let us know at [feedback@shootpath.com](mailto:feedback@shootpath.com).

**Why was I charged twice?**
Duplicate charges are rare but can happen if:
- You clicked "Retry Payment" multiple times (the second charge will be refunded automatically within 5-7 business days)
- Your subscription renewed while we were processing a manual retry for a previous failed payment
- A technical glitch occurred (contact billing support for immediate refund)

Check your invoice history to see if one charge is marked as "Refunded."

**Can I get a refund if my card was charged incorrectly?**
Yes. If you were charged incorrectly due to:
- A billing error on our part
- Duplicate charge
- Charge after cancellation
- Wrong plan amount

Contact [billing@shootpath.com](mailto:billing@shootpath.com) with the invoice number, and we'll issue a refund within 5-7 business days.

Note: Standard subscription charges are non-refundable per our terms of service. See our [Cancellation Policy](./cancellation) for details.

**How do I add someone else's credit card?**
You can add any valid credit or debit card to your account. The cardholder doesn't need to be the account owner. Just:
1. Enter the card details as you normally would
2. Make sure the billing address matches what the card issuer has on file
3. The cardholder should be aware the card is being used for ShootPath subscription

For shared business accounts, consider:
- Using a company card in the business owner's name
- Adding multiple payment methods for different team members
- Setting up a dedicated business credit card for SaaS subscriptions

**Can I pay by invoice or bank transfer?**
For annual plans over $2,000, we can accommodate invoice payment for an additional $100 processing fee. Contact [billing@shootpath.com](mailto:billing@shootpath.com) to arrange this. We require:
- Payment within 30 days of invoice date
- Bank account information for ACH/wire transfer
- Signed annual agreement

Monthly plans must be paid by credit card due to processing overhead.

**What if my card expires?**
Add your new card before the old one expires:
1. Go to **Settings → Billing → Payment Methods**
2. Click **Add Payment Method**
3. Enter your new card information
4. Click **Set as Default**
5. Remove the old card

If your card expires before you update it:
- ShootPath will attempt to charge the expired card
- The charge will fail
- You'll receive an email notification
- Follow the failed payment process above to add a new card

**Do you store my card information?**
No. ShootPath uses Stripe's secure tokenization system. When you add a card:
1. Your browser sends card details directly to Stripe (encrypted)
2. Stripe returns a secure token to ShootPath
3. ShootPath stores only the token, not your actual card data
4. When processing a charge, we send the token to Stripe
5. Stripe handles the actual card transaction

This means:
- Your full card number never touches ShootPath's servers
- Even if ShootPath's database was compromised, your card data would be safe
- Only Stripe (a PCI Level 1 compliant processor) handles your actual card information

**Can I pause my subscription instead of cancelling?**
Yes! If you need a temporary break:
1. Go to **Settings → Billing**
2. Click **Pause Subscription**
3. Choose how long to pause (1-6 months)
4. Your account is frozen (no charges, but you keep your data)
5. Subscription automatically resumes after the pause period

See our [Cancellation Policy](./cancellation) for full details on pausing vs. cancelling.

---

## Need Help?

**Billing Support:**
- Email: [billing@shootpath.com](mailto:billing@shootpath.com)
- Response time: Within 24 hours (usually much faster)

**For Urgent Issues:**
- Failed payment preventing access: Email billing support and mention "urgent" in subject
- Unauthorized charges: Email immediately and CC [security@shootpath.com](mailto:security@shootpath.com)
- Account suspended due to payment issue: Email billing support with your account email

**Include in Your Email:**
- Your account email address
- Invoice number (if applicable)
- Last 4 digits of card used
- Description of the issue
- Screenshots if helpful

Our billing team is here to help resolve any payment issues quickly so you can focus on running your photography business.
