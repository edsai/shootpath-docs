---
sidebar_position: 3
---

# Template Variables

## Quick Reference

Template variables are placeholders in your contract templates that automatically populate with job-specific information. Write `\{clientName\}` once, and it becomes "Sarah Johnson" for every client!

**How Variables Work:**
- Write contract with variables: `\{clientName\}`
- ShootPath fills in real data: "Sarah Johnson"
- Every contract is personalized automatically
- Zero manual editing required

**Variable Syntax:**
- Use curly braces: `\{variableName\}`
- Case-sensitive: `\{clientName\}` not `\{ClientName\}`
- No spaces: `\{sessionDate\}` not `{session date}`
- Optional variables show nothing if data missing

**Common Variables:**
- `\{clientName\}` - Client's full name
- `\{sessionDate\}` - Job/event date
- `\{totalAmount\}` - Total price with currency
- `\{businessName\}` - Your business name
- `\{jobType\}` - Wedding, portrait, event, etc.

**Next Steps:** See the complete [variable reference](#complete-variable-reference) below, or learn how to [create contract templates](./contract-templates).

---

## Detailed Guide

### What Are Template Variables?

Template variables are smart placeholders that transform generic contract templates into personalized client agreements. They're the secret to professional, accurate contracts without manual copy-pasting!

**The magic:** You write your contract once with variables, and ShootPath fills in the actual data from each job automatically.

**Example:**

**Your template says:**
> "This agreement is made on \{signedDate\} between \{businessName\} and \{clientName\} for \{jobType\} photography services on \{sessionDate\} at \{venueName\}. Total investment: \{totalAmount\}."

**Client sees:**
> "This agreement is made on January 15, 2024 between Crashing Elegance Photography and Sarah Johnson for Wedding photography services on June 12, 2024 at Willow Creek Barn. Total investment: $4,500."

No manual editing. No chance of leaving the wrong client's name in the contract. Just accurate, personalized agreements every time!

### Why Use Template Variables?

**Without variables:**
1. Copy last client's contract
2. Search for "Michael Williams" → Replace with "Sarah Johnson" (hope you find every instance!)
3. Search for "$3,000" → Replace with "$4,500"
4. Search for "May 5" → Replace with "June 12"
5. Check for errors (did you miss any?)
6. Repeat for every single client

**With variables:**
1. ShootPath fills everything in automatically
2. That's it!

**Benefits:**

**Accuracy** - No more sending contracts with the wrong client name or date. Variables pull directly from job data, so they're always correct.

**Time savings** - What took 10-15 minutes per contract now happens instantly. That's hours saved per month!

**Consistency** - Every contract uses the same template, so you never forget important clauses or accidentally send different terms to different clients.

**Professionalism** - Personalized contracts show clients you're detail-oriented and organized.

### How to Use Variables in Templates

Using variables is simple: insert them anywhere in your contract template where you want dynamic content.

#### Basic Syntax

Variables use this format:
```
\{variableName\}
```

**Rules:**
- Always use curly braces `{ }`
- No spaces inside the braces
- Case-sensitive (use exact names from reference table)
- Can appear anywhere in text

#### Simple Examples

**Client information:**
```
Dear \{clientName\},

Thank you for choosing \{businessName\} for your \{jobType\} photography!
We're excited to work with you on \{sessionDate\}.
```

**Becomes:**
```
Dear Sarah Johnson,

Thank you for choosing Crashing Elegance Photography for your Wedding photography!
We're excited to work with you on June 12, 2024.
```

**Pricing details:**
```
Total Price: \{totalAmount\}
Deposit Due Now: \{depositAmount\}
Balance Due: \{balanceAmount\}
```

**Becomes:**
```
Total Price: $4,500
Deposit Due Now: $1,500
Balance Due: $3,000
```

#### Variables in Sentences

Variables flow naturally in sentences:

```
This agreement is between \{businessName\} (Photographer) and \{clientName\}
(Client) for photography services on \{sessionDate\} at \{venueName\}.
```

```
Client will receive a minimum of \{minimumPhotos\} professionally edited
high-resolution images delivered within \{deliveryWeeks\} weeks via online
gallery.
```

```
Payment schedule: $\{depositAmount\} due upon signing, $\{balanceAmount\} due
\{balanceDueDays\} days before the session date.
```

#### Variables in Lists

Use variables in bullet points or numbered lists:

```
Services include:
- \{sessionDuration\} hours of photography coverage
- Professional editing and color correction
- Minimum \{minimumPhotos\} high-resolution images
- Online gallery delivery within \{deliveryWeeks\} weeks
- Gallery access for \{galleryAccessDays\} days
```

### Complete Variable Reference

Here's every variable available in ShootPath contract templates, organized by category.

#### Client Variables

Information about your client.

| Variable | Description | Example Output |
|----------|-------------|----------------|
| `\{clientName\}` | Client's full name | "Sarah Johnson" |
| `\{clientFirstName\}` | Client's first name only | "Sarah" |
| `\{clientLastName\}` | Client's last name only | "Johnson" |
| `\{clientEmail\}` | Client's email address | "sarah@example.com" |
| `\{clientPhone\}` | Client's phone number | "(555) 123-4567" |
| `\{clientAddress\}` | Client's full address | "123 Main St, Austin, TX 78701" |
| `\{clientCity\}` | Client's city | "Austin" |
| `\{clientState\}` | Client's state/province | "TX" |
| `\{clientZip\}` | Client's ZIP/postal code | "78701" |

**When to use:**
- Agreement introduction (parties involved)
- Contact information sections
- Mailing address for physical deliveries
- Personalized greetings

**Example usage:**
```
This agreement is made between \{businessName\} and \{clientName\}, residing at
\{clientAddress\}. All correspondence will be sent to \{clientEmail\}.
```

#### Business Variables

Information about your photography business.

| Variable | Description | Example Output |
|----------|-------------|----------------|
| `\{businessName\}` | Your business/studio name | "Crashing Elegance Photography" |
| `\{businessOwner\}` | Your name (business owner) | "Emma Thompson" |
| `\{businessEmail\}` | Business email address | "hello@crashingelegance.com" |
| `\{businessPhone\}` | Business phone number | "(555) 987-6543" |
| `\{businessAddress\}` | Business address | "456 Studio Ln, Austin, TX 78702" |
| `\{businessWebsite\}` | Business website URL | "www.crashingelegance.com" |

**When to use:**
- Agreement introduction
- Contact information
- Payment instructions
- Portfolio references

**Example usage:**
```
Services provided by \{businessName\}, located at \{businessAddress\}.
For questions, contact us at \{businessEmail\} or \{businessPhone\}.
Visit our portfolio at \{businessWebsite\}.
```

#### Job Details Variables

Information about the specific photography job.

| Variable | Description | Example Output |
|----------|-------------|----------------|
| `\{jobType\}` | Type of photography | "Wedding" |
| `\{jobTitle\}` | Job name/title | "Johnson Wedding - June 2024" |
| `\{sessionDate\}` | Date of shoot/event | "June 12, 2024" |
| `\{sessionDateShort\}` | Shorter date format | "06/12/2024" |
| `\{sessionTime\}` | Start time (if specified) | "2:00 PM" |
| `\{sessionDuration\}` | Hours of coverage | "8 hours" |
| `\{venueName\}` | Location/venue name | "Willow Creek Barn" |
| `\{venueAddress\}` | Venue full address | "789 Creek Rd, Dripping Springs, TX" |
| `\{venueCity\}` | Venue city | "Dripping Springs" |

**When to use:**
- Service description sections
- Timeline definitions
- Location details
- Scope of work

**Example usage:**
```
Photographer will provide \{sessionDuration\} of \{jobType\} photography coverage
on \{sessionDate\} starting at \{sessionTime\} at \{venueName\}, located at
\{venueAddress\}.
```

#### Pricing Variables

Financial details from quotes and invoices.

| Variable | Description | Example Output |
|----------|-------------|----------------|
| `\{totalAmount\}` | Total job price with currency | "$4,500" |
| `\{totalAmountNumber\}` | Total as number only | "4500" |
| `\{depositAmount\}` | Deposit amount with currency | "$1,500" |
| `\{depositAmountNumber\}` | Deposit as number only | "1500" |
| `\{balanceAmount\}` | Remaining balance with currency | "$3,000" |
| `\{balanceAmountNumber\}` | Balance as number only | "3000" |
| `\{depositPercent\}` | Deposit as percentage | "33%" |
| `\{balancePercent\}` | Balance as percentage | "67%" |

**When to use:**
- Payment terms sections
- Pricing summaries
- Deposit requirements
- Invoice references

**Example usage:**
```
Total Price: \{totalAmount\}

Payment Schedule:
- Deposit: \{depositAmount\} (\{depositPercent\}) due upon signing
- Balance: \{balanceAmount\} (\{balancePercent\}) due 14 days before session

Late payment may result in rescheduling.
```

#### Payment Schedule Variables

Detailed payment timeline information.

| Variable | Description | Example Output |
|----------|-------------|----------------|
| `\{depositDueDate\}` | When deposit is due | "January 15, 2024" |
| `\{balanceDueDate\}` | When balance is due | "May 29, 2024" |
| `\{balanceDueDays\}` | Days before event balance due | "14" |
| `\{paymentCount\}` | Number of payment installments | "2" |

**When to use:**
- Payment schedule details
- Due date specifications
- Timeline planning

**Example usage:**
```
Payment #1 (Deposit): \{depositAmount\} due \{depositDueDate\}
Payment #2 (Balance): \{balanceAmount\} due \{balanceDueDate\}
(\{balanceDueDays\} days before the event)
```

#### Package and Service Variables

Details about selected packages and add-ons.

| Variable | Description | Example Output |
|----------|-------------|----------------|
| `\{packageName\}` | Selected package name | "Full Day Coverage" |
| `\{packageDescription\}` | Package description | "10 hours, 500+ photos, album" |
| `\{addOnsList\}` | List of selected add-ons | "Engagement Session, Second Photographer" |
| `\{minimumPhotos\}` | Minimum photos promised | "500" |
| `\{maxPhotos\}` | Maximum photos (if specified) | "750" |

**When to use:**
- Service descriptions
- Deliverables sections
- Package summaries

**Example usage:**
```
Client has selected the "\{packageName\}" package, which includes:
\{packageDescription\}

Additional services: \{addOnsList\}

Deliverables: Minimum \{minimumPhotos\} professionally edited high-resolution
digital images.
```

#### Timeline Variables

Delivery and scheduling details.

| Variable | Description | Example Output |
|----------|-------------|----------------|
| `\{deliveryWeeks\}` | Weeks until gallery delivery | "8" |
| `\{deliveryDate\}` | Estimated delivery date | "August 7, 2024" |
| `\{galleryAccessDays\}` | Days gallery stays active | "365" |
| `\{sneakPeekHours\}` | Hours until sneak peek (if offered) | "48" |

**When to use:**
- Delivery timeline sections
- Client expectation setting
- Gallery access terms

**Example usage:**
```
Timeline:
- Sneak peek: \{sneakPeekHours\} hours after session
- Full gallery: \{deliveryWeeks\} weeks from session date
- Estimated delivery: \{deliveryDate\}
- Gallery access: \{galleryAccessDays\} days from delivery
```

#### Date Variables

Important dates throughout the contract lifecycle.

| Variable | Description | Example Output |
|----------|-------------|----------------|
| `\{contractCreatedDate\}` | When contract was generated | "January 15, 2024" |
| `\{signedDate\}` | When client signed contract | "January 16, 2024" |
| `\{todayDate\}` | Current date | "January 20, 2024" |
| `\{currentYear\}` | Current year | "2024" |

**When to use:**
- Agreement date references
- Copyright statements
- Document tracking

**Example usage:**
```
This agreement is made on \{signedDate\} between \{businessName\} and
\{clientName\} for services to be performed on \{sessionDate\}.

© \{currentYear\} {businessName}. All rights reserved.
```

### Optional Variables

Some variables might not have data for every job. When a variable is empty, ShootPath handles it gracefully:

**How empty variables work:**

**Your template:**
```
Services will be provided at \{venueName\} in \{venueCity\}.
```

**If venue is filled in:**
```
Services will be provided at Willow Creek Barn in Dripping Springs.
```

**If venue is NOT filled in:**
```
Services will be provided at  in .
```

Notice the awkward empty spaces! To avoid this, use conditional text or phrase variables carefully.

#### Smart Optional Variable Usage

**Instead of:**
```
Services on \{sessionDate\} at \{venueName\} in \{venueCity\}.
```

**Use:**
```
Services on \{sessionDate\} {venueName}.
```
(Only include location if you know it's always filled in, or use conditional sections - see below)

**For addresses:**
```
\{clientName\}
\{clientAddress\}
\{clientCity\}, \{clientState\} \{clientZip\}
```

If any field is empty, you'll get blank lines. That's usually fine for addresses since the format is expected!

### Advanced: Conditional Sections

:::info Coming Soon
Full conditional logic (IF/THEN/ELSE) is on the roadmap! For now, use smart variable placement and optional sections.
:::

**Current workaround for optional sections:**

If a section only applies sometimes, create multiple templates or use manual editing as a last resort.

**Example:**

Wedding contracts might need travel fees, but portrait contracts don't. Instead of conditionals, create:
- "Wedding Contract - Local" template
- "Wedding Contract - Destination" template

Use the appropriate template based on the job!

### Custom Variables

:::info Coming Soon
Custom variable support is planned! Soon you'll be able to define your own variables for unique business needs.
:::

**Current workaround:**

If you need custom data in contracts:
1. Use the personal note field to include extra details
2. Create multiple template versions for different scenarios
3. Use job titles/descriptions to add context

**Requested custom variables (coming soon):**
- `\{photographerName\}` (for multi-photographer studios)
- `\{assistantName\}` (if second shooter has a name)
- `\{albumDeliveryWeeks\}` (custom timeline for physical products)
- `\{editingStyle\}` (light & airy, dark & moody, etc.)
- `{customField1}` through `{customField5}` (your own fields!)

### Variable Best Practices

#### 1. Always Use Variables for Changing Data

**Don't hard-code:**
```
This agreement is between Crashing Elegance Photography and [CLIENT NAME]
for services on [DATE].
```

**Use variables:**
```
This agreement is between \{businessName\} and \{clientName\} for services
on \{sessionDate\}.
```

#### 2. Test Variables Before Going Live

Create a test job and generate a contract to verify:
- All variables populate correctly
- No `\{variableName\}` shows in output (means typo or invalid variable)
- Formatting looks good with real data
- Spacing around variables is correct

#### 3. Use Descriptive Variable Names

ShootPath's variables are self-explanatory:
- `\{clientName\}` is obvious
- `\{sessionDate\}` is clear
- `\{depositAmount\}` tells you what it is

When custom variables arrive, name yours clearly too:
- `{customField1}` - Bad (what is it?)
- `\{secondShooterName\}` - Good (obvious!)

#### 4. Format Variables in Context

Some variables include formatting (like `\{totalAmount\}` includes "$"), others don't.

**Variables with built-in formatting:**
- `\{totalAmount\}` = "$4,500" (includes $ symbol)
- `\{depositAmount\}` = "$1,500"
- `\{sessionDate\}` = "June 12, 2024" (formatted date)

**Variables without formatting:**
- `\{totalAmountNumber\}` = "4500" (just the number)
- `\{clientName\}` = "Sarah Johnson" (just the name)

**Don't double-format:**

**Wrong:**
```
Total: $\{totalAmount\}
```
**Output:** "Total: $$4,500" (double dollar sign!)

**Right:**
```
Total: \{totalAmount\}
```
**Output:** "Total: $4,500"

#### 5. Handle Missing Data Gracefully

If a variable might be empty, structure sentences so they still make sense:

**Bad:**
```
Services at \{venueName\} in \{venueCity\}
```
(If empty: "Services at  in " - awkward!)

**Better:**
```
Services on \{sessionDate\}
Location: \{venueName\}
```
(If empty: Just shows session date, location line can be removed manually if needed)

### Common Variable Mistakes

**Mistake 1: Typos in Variable Names**

**Wrong:**
```
\{clienName\}  (missing 't')
\{sesionDate\}  (missing 's')
\{totlAmount\}  (missing 'a')
```

**Result:** The variable won't be replaced - it'll show as `\{clienName\}` in the final contract!

**Prevention:** Copy variable names from this reference guide, or use autocomplete (coming soon!).

---

**Mistake 2: Wrong Case**

**Wrong:**
```
\{ClientName\}  (capital C)
\{SESSIONDATE\}  (all caps)
\{clientname\}  (lowercase n)
```

**Right:**
```
\{clientName\}
\{sessionDate\}
\{clientName\}
```

Variables are case-sensitive! Use exact names from the reference table.

---

**Mistake 3: Spaces in Variables**

**Wrong:**
```
{client name}
{session date}
{total amount}
```

**Right:**
```
\{clientName\}
\{sessionDate\}
\{totalAmount\}
```

No spaces inside variable names!

---

**Mistake 4: Forgetting Currency Symbols**

**Wrong:**
```
Total: \{totalAmountNumber\}
```
**Output:** "Total: 4500" (no dollar sign, no commas)

**Right:**
```
Total: \{totalAmount\}
```
**Output:** "Total: $4,500"

Use formatted variables (`\{totalAmount\}`) instead of number-only versions (`\{totalAmountNumber\}`) in most cases.

---

**Mistake 5: Not Testing Variables**

Always generate a test contract before using a template with clients! You'll catch:
- Misspelled variables
- Wrong variables in wrong places
- Formatting issues
- Missing data fields

### Variable Examples by Contract Section

Here are real-world examples of how to use variables in different contract sections:

#### Introduction / Parties

```
PHOTOGRAPHY SERVICES AGREEMENT

This agreement ("Agreement") is made on \{signedDate\} between:

PHOTOGRAPHER: \{businessName\}
Address: \{businessAddress\}
Email: \{businessEmail\}
Phone: \{businessPhone\}

CLIENT: \{clientName\}
Address: \{clientAddress\}
Email: \{clientEmail\}
Phone: \{clientPhone\}

For \{jobType\} photography services on \{sessionDate\}.
```

#### Services Description

```
SERVICES PROVIDED

Photographer agrees to provide \{jobType\} photography services for Client's
event on \{sessionDate\} at \{venueName\}, located at \{venueAddress\}.

Package: \{packageName\}
Coverage: \{sessionDuration\}
Additional services: \{addOnsList\}

Services include:
- Professional photography during scheduled time
- Professional editing and color correction
- High-resolution digital image delivery
- Online gallery hosting
```

#### Deliverables

```
DELIVERABLES

Client will receive:

1. Digital Images: Minimum \{minimumPhotos\} professionally edited high-resolution
   images in JPEG format

2. Delivery Method: Private online gallery accessible via link

3. Delivery Timeline: Within \{deliveryWeeks\} weeks of \{sessionDate\}
   (estimated delivery: \{deliveryDate\})

4. Gallery Access: Gallery remains active for \{galleryAccessDays\} days from
   delivery date

5. Usage Rights: Unlimited personal use license (see Copyright section)
```

#### Pricing and Payment

```
PRICING AND PAYMENT TERMS

Total Price: \{totalAmount\}

Payment Schedule:
1. Deposit: \{depositAmount\} (\{depositPercent\} of total)
   Due: \{depositDueDate\} (upon signing this contract)

2. Balance: \{balanceAmount\} (\{balancePercent\} of total)
   Due: \{balanceDueDate\} (\{balanceDueDays\} days before session)

Payment Methods: Credit card, bank transfer, or check payable to \{businessName\}

Late Payment: Payments not received by due date may result in rescheduling or
cancellation of services.
```

#### Timeline

```
PROJECT TIMELINE

Booking: \{contractCreatedDate\}
Contract Signed: \{signedDate\}
Session Date: \{sessionDate\}
Sneak Peek: \{sneakPeekHours\} hours after session
Full Gallery Delivery: \{deliveryWeeks\} weeks after session (by \{deliveryDate\})
Gallery Access Expires: \{galleryAccessDays\} days after delivery
```

#### Copyright and Usage

```
COPYRIGHT AND USAGE RIGHTS

Photographer: \{businessName\} retains full copyright ownership of all images
created during this session.

Client: \{clientName\} receives an unlimited personal use license including:
- Posting to social media (Facebook, Instagram, personal websites)
- Printing for personal use
- Sharing with family and friends

Client may NOT use images for commercial purposes without written permission
from \{businessName\}.

Model Release: Client grants \{businessName\} permission to use images for
portfolio, website, social media, blog, and marketing materials.
```

#### Signatures

```
SIGNATURES

By signing below, both parties agree to all terms and conditions outlined
in this agreement.

CLIENT: \{clientName\}
Signature: _____________________ Date: __________

PHOTOGRAPHER: \{businessName\}
Signature: _____________________ Date: __________
```

### Troubleshooting Variables

**Problem: Variable shows as `\{variableName\}` in contract**

**Cause:** Variable name is misspelled or doesn't exist

**Fix:**
- Check spelling against reference table
- Verify case sensitivity (`\{clientName\}` not `\{ClientName\}`)
- Make sure no spaces inside braces

---

**Problem: Variable is blank/empty**

**Cause:** Data not filled in for that job

**Fix:**
- Check job details - is the field filled in?
- Some fields are optional (venue name, add-ons list)
- Rephrase contract so missing data doesn't create awkward gaps

---

**Problem: Date format is wrong**

**Cause:** ShootPath uses default date formatting

**Fix:** Use the date variable that fits your needs:
- `\{sessionDate\}` = "June 12, 2024" (long format)
- `\{sessionDateShort\}` = "06/12/2024" (short format)

---

**Problem: Currency symbol appears twice**

**Cause:** You typed `$\{totalAmount\}` and `\{totalAmount\}` already includes "$"

**Fix:** Use `\{totalAmount\}` alone, not `$\{totalAmount\}`

---

**Problem: Numbers have no formatting**

**Cause:** Using number-only variables like `\{totalAmountNumber\}`

**Fix:** Use formatted versions:
- `\{totalAmount\}` instead of `\{totalAmountNumber\}`
- `\{sessionDate\}` instead of date number values

### What's Next?

Now that you understand template variables, you're ready to:

**Create contract templates** → [Learn about Contract Templates](./contract-templates)

**Understand the signing process** → [Read about E-Signatures](./e-signatures)

**See contracts in action** → [Review Understanding Contracts](./index)

**Start using variables** → Go to Settings → Contract Templates in ShootPath!

---

**Quick Reference Card** - Save this for reference when writing templates:

**Most Common Variables:**
```
\{clientName\}          \{businessName\}         \{sessionDate\}
\{clientEmail\}         \{businessEmail\}        \{sessionTime\}
\{clientPhone\}         \{businessPhone\}        \{venueName\}
\{totalAmount\}         \{sessionDuration\}      \{deliveryWeeks\}
\{depositAmount\}       \{jobType\}              \{minimumPhotos\}
\{balanceAmount\}       \{packageName\}          \{signedDate\}
```

---

**Questions?** Look for the help links throughout ShootPath, or reach out to support if you need help!
