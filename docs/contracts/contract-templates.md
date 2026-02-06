---
sidebar_position: 2
---

# Contract Templates

## Quick Reference

Contract templates are reusable legal agreements that auto-populate with job details. Create once, use forever - no more copy-pasting or manual editing!

**What Templates Do:**
- Store your standard contract terms
- Auto-fill client/job details via variables
- Support different contract types (weddings, portraits, etc.)
- Default vs. custom templates for flexibility

**Template Essentials:**
- **Template name** - "Wedding Contract", "Portrait Session Agreement"
- **Contract content** - Your legal terms in plain text
- **Template variables** - Placeholders like `\{clientName\}` that auto-populate
- **Activation status** - Active templates appear in job workflows
- **Job type assignment** - Link templates to specific job types

**Quick Start:** Create a default template for general use, then add custom templates for specialized job types (commercial, real estate) that need different terms.

**Next Steps:** Learn about [template variables](./template-variables) to personalize contracts automatically, or see [e-signatures](./e-signatures) to understand how clients sign.

---

## Detailed Guide

### What Are Contract Templates?

Think of a contract template as a fill-in-the-blank version of your legal agreement. You write the contract terms once, insert placeholders for things that change (client name, session date, pricing), and ShootPath fills in the blanks automatically when you send a contract.

**Without templates:**
- Copy last client's contract
- Find/replace client name (hope you don't miss one!)
- Update session date manually
- Change pricing manually
- Paste into PDF editor
- Save, attach, send
- Repeat for every single client

**With templates:**
- Write contract terms once
- Add template variables for dynamic content
- ShootPath fills in client details automatically
- Every contract is accurate and personalized
- Zero manual work per booking

Templates save hours of admin work and eliminate errors like sending Client A a contract with Client B's name!

### Default vs. Custom Templates

ShootPath supports two template types:

#### Default Templates

**Purpose:** General contracts that work for most job types.

**When to use:**
- You're just getting started
- Most of your work is similar (all portraits, all weddings)
- You want one standard agreement for everything

**How it works:**
- Create one "Photography Services Agreement" template
- All job types use this template unless overridden
- Perfect for photographers who offer one main service type

**Example:**
Sarah shoots family portraits and headshots exclusively. She creates one "Portrait Session Contract" as her default. Every job gets this contract - simple!

#### Custom Templates

**Purpose:** Specialized contracts for specific job types with different terms.

**When to use:**
- Different job types need different legal terms
- Commercial work requires work-for-hire clauses
- Real estate has specific usage rights
- Events have different liability concerns than portraits

**How it works:**
- Create job-type-specific templates
- Assign each to relevant job types in Settings → Job Types
- ShootPath uses the custom template when you create jobs of that type
- Falls back to default template if no custom template assigned

**Example:**
Mike shoots weddings, corporate events, and real estate. He creates:
- "Wedding Contract" (extensive model release, 8-week delivery)
- "Corporate Event Contract" (commercial usage rights, faster delivery)
- "Real Estate Contract" (usage rights transfer to agent/seller)
- Each contract addresses the unique needs of that work type

### Creating Your First Template

Let's build a contract template step by step.

#### Step 1: Access Template Settings

1. Go to **Settings** (⚙️ icon in main navigation)
2. Click **Contract Templates** in the sidebar
3. Click **Create Template** button

You'll see the template editor with two main fields: Template Name and Contract Content.

#### Step 2: Name Your Template

Choose a descriptive name that tells you what it's for:

**Good names:**
- "Wedding Photography Contract"
- "Portrait Session Agreement"
- "Commercial Photography Contract"
- "Real Estate Shoot Agreement"

**Avoid vague names:**
- "Contract" (which one?)
- "Template 1" (doesn't tell you anything)
- "Main" (main for what?)

You'll see this name when assigning templates to job types, so make it clear!

#### Step 3: Write Your Contract Content

This is the legal agreement itself. Write in plain English, breaking content into clear sections:

**Essential sections to include:**

**1. Introduction / Parties**
```
This Photography Services Agreement ("Agreement") is made on \{signedDate\}
between \{businessName\} ("Photographer") located at \{businessAddress\}, and
\{clientName\} ("Client") located at \{clientAddress\}.
```

**2. Services Description**
```
Photographer agrees to provide photography services for Client's \{jobType\}
on \{sessionDate\} at \{venueName\} (if provided). Services include:

- \{sessionDuration\} hours of professional photography coverage
- Professional editing and color correction
- Online gallery delivery within \{deliveryWeeks\} weeks
- Minimum of \{minimumPhotos\} fully edited high-resolution images
```

**3. Pricing and Payment**
```
Total Price: \{totalAmount\}

Payment Schedule:
- Deposit: \{depositAmount\} due upon signing this contract
- Balance: \{balanceAmount\} due \{balanceDueDays\} days before the session date

Late payments may result in rescheduling or cancellation.
```

**4. Deliverables**
```
Client will receive:
- High-resolution digital files via secure online gallery
- Personal use license for all delivered images
- Gallery access for \{galleryAccessDays\} days from delivery
- Print authorization for personal use
```

**5. Timeline**
```
- Session date: \{sessionDate\}
- Sneak peek (if offered): 48 hours after session
- Full gallery delivery: Within \{deliveryWeeks\} weeks of session
- Gallery remains active for \{galleryAccessDays\} days
```

**6. Cancellation Policy**
```
Photographer Cancellation:
If Photographer cannot fulfill services due to emergency, illness, or
unforeseen circumstances, Client will receive a full refund or be offered
a qualified replacement photographer.

Client Cancellation:
- More than 90 days before session: Full refund minus $100 admin fee
- 60-90 days before session: 50% refund
- Less than 60 days before session: No refund (deposit is non-refundable)

Rescheduling:
First reschedule is free if made 30+ days in advance. Subsequent
reschedules or those made within 30 days incur a $150 fee.
```

**7. Copyright and Usage Rights**
```
Photographer retains full copyright ownership of all images. Client receives
an unlimited personal use license including:
- Social media posting
- Printing for personal use
- Sharing with family and friends

Client may NOT:
- Use images for commercial purposes without written permission
- Sell or license images to third parties
- Remove copyright watermarks (if present)
- Claim ownership or creation of images
```

**8. Model Release**
```
Client grants Photographer permission to use photographs from this session
for portfolio, website, social media, blog, advertising, and promotional
materials. Photographer will use images tastefully and respectfully.

If you prefer your images NOT be used for marketing purposes, initial here: _____
```

**9. Liability Limitations**
```
Photographer will use professional equipment and maintain backup systems.
However, Photographer is not liable for:
- Missed photos due to venue restrictions, poor lighting, or guest obstruction
- Equipment failure despite backup equipment being present
- Data loss in the unlikely event of catastrophic failure of all backup systems

Maximum liability for any claim is limited to a full refund of amounts paid.
```

**10. Force Majeure**
```
Neither party is liable for failure to perform due to circumstances beyond
reasonable control including natural disasters, pandemic, venue closure,
or government restrictions. In such cases, rescheduling will be offered at
no additional charge.
```

**11. Entire Agreement**
```
This Agreement constitutes the entire agreement between parties and supersedes
all prior negotiations, representations, or agreements. Modifications must be
made in writing and signed by both parties.

Client Signature: _____________________  Date: __________
Photographer Signature: _____________________  Date: __________
```

:::tip Start with a Template
Many photography organizations (PPA, ASMP, local photographer groups) offer contract templates as member benefits. Start with one of those, then customize for your business. Don't create from scratch unless you're working with a lawyer!
:::

#### Step 4: Add Template Variables

As you write your contract, insert template variables wherever content should be auto-filled. Variables use this format: `\{variableName\}`

**Common variables:**
- `\{clientName\}` - Client's full name
- `\{businessName\}` - Your business name
- `\{sessionDate\}` - Job/session date
- `\{totalAmount\}` - Job total price
- `\{jobType\}` - Type of photography (wedding, portrait, etc.)

See the full list in [Template Variables](./template-variables).

**How to use variables:**

Instead of writing:
> "This agreement is between [YOUR BUSINESS NAME] and [CLIENT NAME] for services on [DATE]"

Write:
> "This agreement is between \{businessName\} and \{clientName\} for services on \{sessionDate\}"

When you send the contract to Sarah Johnson for her October 15 wedding:
> "This agreement is between Crashing Elegance Photo and Sarah Johnson for services on October 15, 2024"

ShootPath fills in the blanks automatically!

#### Step 5: Preview Your Template

Before saving, preview how the contract will look to clients:

1. Click **Preview** button in template editor
2. Review formatting (line breaks, spacing, bold/italic)
3. Check that variables are positioned correctly
4. Read through for typos or unclear language

The preview shows placeholder values for variables so you can see the structure.

#### Step 6: Save and Activate

1. Click **Save Template**
2. Toggle **Active** to enable this template
3. Inactive templates aren't available when creating contracts

You can have multiple templates but only activate the ones you currently use. This keeps your template list clean!

### Editing Existing Templates

Life changes, your business evolves, and your contracts should too!

**To update a template:**

1. Go to Settings → Contract Templates
2. Click the template you want to edit
3. Make your changes
4. Click **Save**

**Important:** Changes only apply to future contracts. Existing signed contracts are never modified (they're legal documents!).

**When to update templates:**
- You change your cancellation policy
- Delivery timelines change
- Pricing structure changes
- You add new services
- State laws change
- Your lawyer recommends revisions

:::warning Annual Review
Review your contract templates at least once per year. Laws change, your business changes, and past client issues might reveal gaps in your contract that need addressing.
:::

### Assigning Templates to Job Types

Custom templates need to be assigned to specific job types to be used automatically.

**To assign templates:**

1. Go to Settings → Job Types
2. Click the job type you want to customize (e.g., "Wedding", "Real Estate")
3. Find **Contract Template** dropdown
4. Select the custom template
5. Click **Save**

Now when you create a job of that type, ShootPath automatically uses that template!

**Example workflow:**
1. Create "Commercial Contract" template with work-for-hire clause
2. Go to Settings → Job Types → "Commercial"
3. Set Contract Template to "Commercial Contract"
4. Every commercial job now uses this specialized contract automatically

### Default Template Setup

The default template is your fallback for any job type that doesn't have a custom template assigned.

**To set a default template:**

1. Create a general-purpose contract template
2. Name it clearly (e.g., "Standard Photography Contract")
3. Go to Settings → Contract Templates
4. Mark it as **Default Template**
5. Activate it

Now any job type without a custom template uses this one!

**Best practice:** Always have a default template. Even if you use mostly custom templates, you need a fallback for one-off job types or when you're testing new offerings.

### Template Formatting Best Practices

Well-formatted contracts are easier to read and more likely to be signed!

#### Use Clear Headings

Break your contract into numbered sections with bold headings:

```
1. Services and Deliverables
2. Pricing and Payment Terms
3. Timeline and Delivery
4. Cancellation and Rescheduling
5. Copyright and Usage Rights
6. Liability Limitations
```

#### Use Short Paragraphs

**Bad:**
> "Photographer will provide professional photography services including but not limited to capturing images during the specified event or session using professional-grade equipment and will deliver edited images via online gallery within the specified timeframe subject to the terms outlined in this agreement regarding payment and client cooperation with timeline and location requirements."

**Good:**
> "Photographer will provide professional photography services during the specified event or session using professional-grade equipment.
>
> Edited images will be delivered via online gallery within the specified timeframe, subject to payment and client cooperation."

#### Use Bullet Points

Lists are easier to scan:

**Instead of:**
> "Services include professional photography, professional editing, color correction, online gallery delivery, and high-resolution digital files."

**Use:**
> Services include:
> - Professional photography
> - Professional editing and color correction
> - Online gallery delivery
> - High-resolution digital files

#### Use Plain English

**Legal jargon:**
> "The parties hereto agree that in the event of breach of the aforementioned terms..."

**Plain English:**
> "If either party breaks these terms..."

Your clients aren't lawyers. Write contracts they can understand without a legal dictionary!

#### Include a Table of Contents

For long contracts (4+ pages), add a table of contents at the top:

```
Table of Contents
1. Services and Deliverables ...................... Page 1
2. Pricing and Payment Terms ....................... Page 1
3. Timeline and Delivery ........................... Page 2
4. Cancellation Policy ............................. Page 2
5. Copyright and Usage Rights ...................... Page 3
6. Liability Limitations ........................... Page 3
7. Model Release ................................... Page 4
8. Signatures ...................................... Page 4
```

### Contract Template Examples by Genre

Different photography genres need different contract terms. Here's what to emphasize for each:

#### Wedding Contracts

**Unique elements:**
- Backup photographer clause (what if you're sick?)
- Detailed shot list discussion (client provides, but photographer isn't liable for missed shots)
- Longer delivery timeline (8-12 weeks typical)
- Travel fees if destination wedding
- Alcohol policy (you won't drink at events)
- Cooperation clause (venue access, timeline cooperation)

**Sample clause:**
> "Wedding photography involves dynamic, unpredictable environments. While Photographer will capture key moments (ceremony, first dance, cake cutting), Photographer is not liable for missed shots due to guest obstruction, venue restrictions, or poor lighting. Client may provide a shot list, but it serves as guidance only and is not a guarantee."

#### Portrait Contracts

**Unique elements:**
- Weather cancellation policy (outdoor shoots)
- What to wear / preparation guidance
- How many outfit changes included
- Retouching policy (included vs. additional fee)
- Shorter delivery timeline (2-4 weeks)
- Print ordering process

**Sample clause:**
> "If weather prevents outdoor shooting, session will be rescheduled to a mutually agreed date at no additional charge. Indoor studio alternative may be offered if available."

#### Commercial Contracts

**Unique elements:**
- Usage rights transfer (client often needs commercial usage)
- Work-for-hire considerations
- Image licensing terms
- Brand/product guidelines compliance
- Faster turnaround times
- Raw file delivery options
- Exclusivity clauses

**Sample clause:**
> "Client receives full commercial usage rights for delivered images including advertising, marketing, website, print materials, and social media. Photographer retains copyright but grants unlimited usage license. Raw files are not included unless specified in pricing."

#### Real Estate Contracts

**Unique elements:**
- Usage rights transfer to agent/seller
- Fast turnaround (24-48 hours typical)
- Reshoot policy if property doesn't show well
- MLS compliance (specific image requirements)
- Twilight/drone considerations

**Sample clause:**
> "Images will be delivered within 24 hours of shoot completion. Usage rights transfer to listing agent and property seller for purposes of marketing and selling the property. Photographer retains copyright for portfolio use only."

#### Event Contracts

**Unique elements:**
- Specific coverage hours
- Overtime rate clearly defined
- Meal provision requirement (for long events)
- Parking/access requirements
- Same-day preview options
- Corporate/organization branding usage

**Sample clause:**
> "Coverage includes \{hours\} hours starting at \{startTime\}. Additional coverage beyond contracted hours is available at $\{overtimeRate\}/hour, subject to photographer availability and client approval before overtime begins."

### Common Contract Template Mistakes

**Mistake 1: Too Vague**

**Bad:**
> "Photographer will deliver photos in a reasonable timeframe."

**Good:**
> "Photographer will deliver a minimum of \{minimumPhotos\} edited images within \{deliveryWeeks\} weeks of the session date."

Be specific! "Reasonable" means different things to different people.

**Mistake 2: One-Sided Liability**

**Bad:**
> "Photographer is not liable for anything that goes wrong, ever, for any reason."

**Good:**
> "Photographer will use professional equipment, backup systems, and best practices. However, liability is limited to a full refund in the event of equipment failure, data loss, or inability to deliver images."

Courts may not uphold completely one-sided contracts. Be fair!

**Mistake 3: Missing Cancellation Policy**

If your contract doesn't address cancellations, you have no recourse when a client cancels 3 days before a wedding. Always include:
- Photographer cancellation (emergency/illness)
- Client cancellation (with refund schedule)
- Rescheduling policy
- Force majeure (pandemic, natural disaster)

**Mistake 4: Unclear Usage Rights**

**Bad:**
> "Client can use photos."

**Good:**
> "Client receives unlimited personal use license including social media, printing, and sharing with family. Commercial use requires written permission and licensing fee."

Define "personal" vs. "commercial" explicitly!

**Mistake 5: No Model Release**

Always include model release language giving you permission to use photos for marketing. Make it opt-out (they initial if they DON'T want photos used) rather than opt-in.

**Mistake 6: Forgetting Template Variables**

If you type "John Smith" instead of `\{clientName\}`, every contract will say "John Smith"! Use variables for everything that changes per client.

### Template Variable Best Practices

**Use variables for anything that changes per job:**
- Client info (name, email, phone, address)
- Session details (date, time, location)
- Pricing (total, deposit, balance)
- Deliverables (number of photos, delivery weeks)
- Job type (wedding, portrait, event)

**Don't use variables for:**
- Your business terms (standard clauses that never change)
- Legal language
- Liability limitations
- Copyright information

**Smart variable usage:**

Instead of hard-coding:
> "Client will receive 500 edited photos delivered within 8 weeks"

Use variables:
> "Client will receive a minimum of \{minimumPhotos\} edited photos delivered within \{deliveryWeeks\} weeks"

Now you can adjust per job! A mini session might be 15 photos in 1 week, while a wedding might be 500 photos in 10 weeks.

Learn more in [Template Variables](./template-variables).

### Handling Special Contract Requests

Sometimes clients ask to modify your contract. Here's how to handle it:

**Request: "Can we remove the model release clause?"**

**Response:** "Absolutely! I'll add an addendum noting you prefer your photos not be used for marketing. Everything else remains the same."

**How to handle:** Create a simple addendum document that modifies just that clause, signed by both parties.

**Request: "Can we change the delivery timeline from 8 weeks to 4 weeks?"**

**Response:** "I can offer rush delivery for an additional $300. Would you like me to send an updated quote?"

**How to handle:** Don't give away rush services for free! Update the quote with rush delivery as an add-on.

**Request: "We need commercial usage rights for these photos."**

**Response:** "My standard personal-use contract doesn't include commercial licensing. I can send you a commercial contract with full usage rights - there's an additional licensing fee of $500."

**How to handle:** Use your commercial contract template with appropriate pricing.

**Request: "Can you make 20 edits to this contract?"**

**Response:** "I'm happy to discuss specific concerns! However, I can't do extensive custom contracts for standard sessions. If your needs are highly specialized, I recommend consulting with your own attorney to draft an agreement, and I'll review it."

**How to handle:** Don't let clients rewrite your entire contract. If they need something completely different, refer them elsewhere or charge a consultation fee.

:::warning Don't Let Clients Edit Contracts Directly
If a client crosses out clauses and initials them, that creates legal ambiguity about what you both agreed to. Instead, discuss their concerns and create a formal addendum if needed. Never accept a hand-edited contract!
:::

### Testing Your Templates

Before using a template with real clients, test it!

**Testing checklist:**

1. **Create a test lead/job**
   - Use realistic test data
   - Fill in all fields that map to variables

2. **Generate a contract from the template**
   - Check that all variables populate correctly
   - Look for any `\{variableName\}` that didn't get replaced (means that variable doesn't exist or is misspelled)

3. **Review formatting**
   - Line breaks in right places?
   - Spacing consistent?
   - Bold/italic preserved?
   - Page breaks sensible?

4. **Read through entirely**
   - Does it make sense?
   - Are there contradictions?
   - Is everything spelled correctly?
   - Does anything feel confusing?

5. **Test the signing flow**
   - Send to your own email
   - Go through client signing experience
   - Verify signed PDF looks correct

6. **Have someone else read it**
   - Fresh eyes catch mistakes you miss
   - Ask "is anything confusing?"
   - Bonus: Have a lawyer review it!

### Managing Multiple Templates

As your business grows, you might have several templates:

**Template organization tips:**

**Use clear naming:**
- "Wedding - Standard"
- "Wedding - Premium (includes album)"
- "Portrait - Studio"
- "Portrait - Outdoor"
- "Commercial - Product Photography"
- "Commercial - Headshots"

**Keep them organized:**
- Archive old templates rather than deleting them
- Mark active templates clearly
- Deactivate templates you're not currently using

**Version control:**
If you make significant changes, consider creating a new template version rather than editing the existing one:
- "Portrait Contract v1" (original)
- "Portrait Contract v2" (updated cancellation policy)
- "Portrait Contract v3" (added rush delivery terms)

This helps you track which clients signed which version if issues arise later!

### Contract Template Legal Considerations

:::warning Not Legal Advice
I'm a photography software company, not a lawyer! This guide provides general information, but you should consult with an attorney to ensure your contracts are enforceable in your jurisdiction.
:::

**State-specific requirements:**
- Some states have specific contract requirements
- Statutes of limitations vary by state
- Consumer protection laws differ
- Small claims court limits vary

**Consider having a lawyer review your template if:**
- You're doing high-value work ($5k+ per project)
- You're doing commercial work with complex usage rights
- You're working across multiple states
- You've had client disputes in the past
- You want peace of mind!

**Resources:**
- Professional Photographers of America (PPA) offers legal resources
- American Society of Media Photographers (ASMP) has contract templates
- Local photographers' associations often provide templates
- State bar associations sometimes have small business resources

### What's Next?

Now that you understand contract templates, you're ready to:

**Personalize contracts automatically** → [Learn about Template Variables](./template-variables)

**Understand how clients sign** → [Read about E-Signatures](./e-signatures)

**See the big picture** → [Review Understanding Contracts](./index)

**Start building contracts** → Go to Settings → Contract Templates in ShootPath!

---

**Questions?** Look for the help links throughout ShootPath, or reach out to support if you need help!
