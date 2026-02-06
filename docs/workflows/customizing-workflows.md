---
sidebar_position: 3
---

# Customizing Workflows

## Quick Reference

ShootPath's default workflows work great out of the box, but you can customize them to match your exact business process. Create workflows that reflect how you actually work!

**What You Can Customize:**
- **Workflow stages** - Add, remove, or reorder stages
- **Stage transitions** - Define what moves jobs between stages
- **Automated emails** - Edit timing, content, and triggers
- **Workflow tasks** - Add custom tasks for your process
- **Conditional logic** - Set up if/then rules for different scenarios

**Common Customizations:**
- Create separate workflows for different job types (wedding, portrait, commercial)
- Add stages for your unique process (consultation calls, album design, etc.)
- Adjust email timing to match your communication style
- Add tasks for things you always do but the defaults don't include

**Quick Access:**
- **Settings > Workflows** - View and edit all workflows
- Clone existing workflows to create variations
- Test workflows with dummy jobs before going live

:::tip Start With Defaults First
Use the default workflows for 4-6 weeks before customizing. This helps you understand what actually needs to change based on real experience!
:::

---

## Detailed Guide

### Why Customize Workflows?

The default workflows cover the common photography business process, but every photographer is unique. You might:

**Have specific consultation steps:**
"I always do a phone consultation before sending a quote."

**Offer unique services:**
"I include engagement sessions with all wedding packages."

**Have different timelines:**
"I deliver mini session galleries within 3 days, not 2 weeks."

**Use different communication patterns:**
"I prefer to text clients instead of email for certain milestones."

**Work with teams:**
"My editor handles post-processing, so I need tasks assigned to them."

Customization lets you build workflows that match your reality, not a generic template.

### Accessing the Workflow Builder

**To open the workflow builder:**

1. Navigate to **Settings** (gear icon in sidebar)
2. Click **Workflows**
3. See list of all workflows (default + custom)
4. Click **"Edit"** on any workflow to modify it
5. Or click **"Create New Workflow"** to start from scratch

**What you'll see:**
- List of workflow stages (e.g., Contract Pending, Deposit Pending)
- Emails associated with each stage
- Tasks created at each stage
- Transition rules between stages

### Creating a New Workflow from Scratch

**When to do this:**
When your process is significantly different from defaults, or when you need a workflow for a specific job type (like mini sessions or commercial projects).

#### Step 1: Name Your Workflow

Give your workflow a descriptive name:
- "Wedding Photography Workflow"
- "Mini Session Workflow"
- "Commercial Project Workflow"
- "Family Portrait Workflow"

**Why names matter:**
When creating a job, you'll select which workflow to use. Clear names help you (and team members) choose the right one.

#### Step 2: Define Your Stages

Stages are the major phases your jobs go through. Think about your actual process:

**Example: Wedding Workflow Stages**
1. Contract Pending
2. Deposit Pending
3. Engagement Session Planning
4. Engagement Session Complete
5. Wedding Timeline Coordination
6. Final Payment (before wedding)
7. Wedding Day
8. Editing
9. Gallery Delivered
10. Album Design (if applicable)
11. Complete

**Example: Mini Session Workflow Stages**
1. Booked (no contract needed)
2. Paid (full payment upfront)
3. Session Day
4. Editing
5. Gallery Delivered
6. Print Sales Follow-Up
7. Complete

**Keep it simple:**
Don't create 20 stages. Focus on distinct phases where something meaningful changes or actions are needed.

**How to add a stage:**

1. Click **"Add Stage"** in workflow builder
2. Enter stage name
3. Optional: Add description (visible only to you)
4. Set stage order (drag to reorder)
5. Save

#### Step 3: Configure Each Stage

For each stage, define:

**1. Entry Trigger**
What causes the workflow to enter this stage?
- Manual (you move it)
- Automatic (triggered by an event)

**Examples:**
- "Contract Pending" stage starts when job is created
- "Deposit Pending" starts when contract is signed
- "Editing" starts when you mark session complete

**2. Exit Trigger**
What causes the workflow to move to the next stage?
- Manual (you mark as complete)
- Automatic (event occurs)
- Time-based (after X days)

**Examples:**
- "Contract Pending" exits when contract is signed
- "Deposit Pending" exits when payment is received
- "Editing" exits when you upload gallery

**3. Tasks to Create**
What action items should appear when this stage starts?

**Examples:**
- "Follow up if contract not signed within 3 days"
- "Confirm session location with client"
- "Edit photos (due 2 weeks from session date)"

**4. Emails to Send**
What automatic emails should go out?

**Examples:**
- When entering "Contract Pending": Send contract email
- When entering "Gallery Delivered": Send gallery notification
- 3 days into "Contract Pending": Send reminder if not signed

#### Step 4: Set Up Email Automation

For each email, configure:

**Trigger:**
When should the email send?
- Immediately when entering a stage
- X days after entering a stage
- When a specific condition is met

**Template:**
Which email template to use? (You create templates separately in Email Templates section)

**Recipient:**
Who receives the email?
- Primary client
- Secondary client (for weddings)
- Both clients
- You (internal notification)

**Conditional Sending:**
Should this email only send in certain cases?
- Only if balance is due
- Only if questionnaire not completed
- Only if session is within 7 days

**Example Configuration:**

**Email:** "Please Sign Your Contract"
- **Trigger:** Immediately when job enters "Contract Pending" stage
- **Template:** Contract Signing Request
- **Recipient:** Primary client
- **Condition:** Contract status is "pending" (not already signed)

#### Step 5: Define Task Automation

For each task, configure:

**Task Title:**
Clear, actionable description
- "Send questionnaire to client"
- "Confirm session date and location"
- "Edit photos"

**Due Date:**
When should this be done?
- Relative to stage entry (e.g., "3 days from now")
- Relative to job event (e.g., "2 days before session date")
- Absolute date (rarely used)

**Assignee:**
Who is responsible?
- You (default)
- Specific team member
- Role-based (e.g., "Editor")

**Priority:**
How urgent is this task?
- High (red flag, urgent)
- Normal (standard tasks)
- Low (nice-to-have)

**Example Configuration:**

**Task:** "Follow up if contract not signed"
- **Due Date:** 3 days after stage entry
- **Assignee:** Job owner (you)
- **Priority:** High
- **Conditional:** Only create if contract still pending

#### Step 6: Test Your Workflow

Before using your custom workflow with real clients, test it!

**How to test:**

1. Create a "test job" with dummy client data
2. Assign your new custom workflow to it
3. Walk through each stage manually
4. Verify emails send correctly (to your test email)
5. Check that tasks appear at the right time
6. Confirm transitions work as expected

**What to check:**
- Do emails send when expected?
- Is the wording clear and professional?
- Do tasks have realistic due dates?
- Are transitions smooth?
- Does conditional logic work?

**Fix issues:**
If something's wrong, edit the workflow and test again. Don't deploy to real clients until you're confident it works!

### Cloning and Modifying Existing Workflows

Instead of starting from scratch, clone an existing workflow and modify it.

**When to clone:**

**Creating variations:**
You like the default job workflow but want a faster version for mini sessions.

**Different job types:**
Start with the wedding workflow, clone it for portrait sessions, and simplify.

**A/B testing:**
Clone a workflow, make changes, and compare results.

**How to clone:**

1. Go to **Settings > Workflows**
2. Find the workflow you want to copy
3. Click **"⋯" (three dots)** → **"Duplicate"**
4. Workflow copied with "(Copy)" appended to name
5. Rename it (e.g., "Mini Session Workflow")
6. Edit stages, tasks, and emails as needed

**Benefits of cloning:**
- Faster than starting from scratch
- Preserves working logic while allowing tweaks
- Easy to compare old vs. new

### Customizing Email Timing

One of the most common customizations is adjusting when automated emails send.

#### Default Timing

**Lead workflow:**
- Follow-up #1: 5 days after quote
- Follow-up #2: 10 days after quote

**Job workflow:**
- Pre-session reminder: 7 days before session
- Post-session update: Immediately after session marked complete

#### Custom Timing Examples

**Faster follow-ups:**
Some photographers prefer more aggressive follow-up:
- Follow-up #1: 3 days after quote
- Follow-up #2: 6 days after quote
- Final follow-up: 9 days after quote

**Longer turnarounds:**
If you have a longer editing timeline:
- Post-session update: "Photos will be ready in 4 weeks" (instead of 2 weeks)

**Additional touchpoints:**
Add extra emails:
- 14 days before session: "Preparing for Your Session" guide
- 2 days after gallery delivery: "How are you enjoying your photos?"

**How to change email timing:**

1. Edit the workflow
2. Click on the email you want to adjust
3. Change the trigger from "5 days after" to "3 days after" (for example)
4. Save changes

### Adding Custom Stages

Let's walk through adding a custom stage to an existing workflow.

#### Example: Adding "Consultation Call" Stage

**Scenario:** You always schedule a phone consultation before sending quotes. You want to track this in your workflow.

**Steps:**

1. Open Lead Workflow
2. Click **"Add Stage"** after "New Inquiry"
3. Name it "Consultation Scheduled"
4. Set entry trigger: Manual (you move leads here)
5. Set exit trigger: Manual (you move to "Quoted" after call)
6. Add task: "Complete consultation call"
7. Add task: "Send quote after call"
8. Add email (optional): "Consultation Scheduled Confirmation" with call details
9. Save stage

**Result:**
Your workflow now has an extra step between inquiry and quote. This reminds you to complete the call before quoting!

#### Example: Adding "Engagement Session" Stage to Wedding Workflow

**Scenario:** All your wedding packages include an engagement session. You want a dedicated stage for planning and executing it.

**Steps:**

1. Open Wedding Workflow
2. Click **"Add Stage"** after "Deposit Pending"
3. Name it "Engagement Session Planning"
4. Add task: "Schedule engagement session with client"
5. Add task: "Send engagement questionnaire"
6. Add email: "Let's Plan Your Engagement Session!"
7. Set exit trigger: Manual (when session is booked and confirmed)
8. Add another stage: "Engagement Session Complete"
9. Add task: "Edit engagement photos"
10. Add email: "Engagement Gallery is Ready!"
11. Save

**Result:**
Your wedding workflow now has a built-in engagement session phase with reminders and automation.

### Conditional Logic and Branching

Advanced workflows can branch based on conditions.

#### Example: Print Orders

**Scenario:** If a client orders prints, you want a different follow-up than if they don't.

**Logic:**
- If print order = yes → Stage: "Print Order Fulfillment"
- If print order = no → Skip to "Complete"

**How to set this up:**

1. Add stage: "Print Order Fulfillment"
2. Set entry condition: "If print order exists"
3. Add tasks for print processing
4. Add email: "Print Order Confirmation"
5. Set exit trigger: When prints are delivered
6. For jobs without print orders, stage is automatically skipped

#### Example: Payment Plan vs. Full Payment

**Scenario:** Some clients pay in full upfront, others use payment plans. You want different workflows.

**Logic:**
- If payment plan → Stages for each installment
- If full payment → Skip installment stages

**How to set this up:**

1. Add conditional check at "Deposit Pending" stage
2. If balance remaining = 0 → Skip "Final Payment" stages
3. If balance remaining > 0 → Continue through payment stages

### Creating Workflow Variations by Job Type

Different types of photography need different workflows. Here's how to create optimized workflows for each.

#### Wedding Workflow

**Unique needs:**
- Longer timeline (often 6-12 months)
- Multiple payment milestones
- Engagement session
- Timeline coordination
- Vendor communication
- Album design

**Stages:**
1. Contract Pending
2. Retainer Paid
3. Engagement Session Scheduled
4. Engagement Session Complete
5. Timeline Planning (3 months before)
6. 2nd Payment Due (1 month before)
7. Final Payment Due (1 week before)
8. Wedding Day
9. Editing (4-6 weeks)
10. Gallery Delivered
11. Album Design
12. Complete

**Key automation:**
- Multiple payment reminders at different intervals
- Timeline coordination task 3 months out
- Vendor contact sharing 2 weeks out
- Post-wedding "thank you" email

#### Mini Session Workflow

**Unique needs:**
- Short timeline (usually 1-2 weeks)
- No contract (often signed in person)
- Full payment upfront
- Quick turnaround (3-7 days)
- Print sales follow-up

**Stages:**
1. Booked & Paid
2. Session Day
3. Editing
4. Gallery Delivered
5. Print Sales Follow-Up
6. Complete

**Key automation:**
- Session reminder 2 days before
- Fast turnaround task (due in 3 days)
- Print promotion email 1 week after gallery

#### Portrait Session Workflow

**Unique needs:**
- Moderate timeline (2-4 weeks)
- Simple payment (deposit + balance)
- Questionnaire for session planning
- Standard turnaround (2 weeks)

**Stages:**
1. Contract Pending
2. Deposit Pending
3. Pre-Session Prep
4. Session Complete
5. Editing
6. Gallery Delivered
7. Final Payment (if balance due)
8. Complete

**Key automation:**
- Questionnaire sent 2 weeks before
- Session reminder 3 days before
- Gallery notification with payment link
- Thank you email after completion

#### Commercial/Corporate Workflow

**Unique needs:**
- Formal SOW (statement of work)
- Net 30 or Net 60 payment terms
- Usage rights documentation
- Specific deliverable requirements
- Invoicing instead of online payments

**Stages:**
1. SOW Pending
2. SOW Signed
3. Project Kickoff
4. Shoot Day(s)
5. Editing & Deliverables
6. Client Review
7. Final Deliverables
8. Invoice Sent (Net 30)
9. Payment Received
10. Complete

**Key automation:**
- Formal email language (less casual)
- Usage rights reminder at delivery
- Invoice follow-up at Net 30 deadline
- Quarterly check-in for future projects

### Best Practices for Custom Workflows

**Start simple, add complexity gradually:**
Don't create a 15-stage workflow on day one. Start with 5-7 key stages and add more as needed.

**Test thoroughly:**
Always test new workflows with dummy jobs before using with real clients.

**Use clear naming:**
Stage and task names should be obvious. "Editing" is better than "Post-Production Phase 2."

**Set realistic deadlines:**
Don't promise 1-week turnaround if you need 3 weeks. Build in buffer time!

**Keep emails client-friendly:**
Even automated emails should sound warm and personal, not robotic.

**Document your process:**
Add descriptions to stages explaining why they exist. This helps if you hire team members later!

**Review and refine:**
Every 3-6 months, review your workflows. What's working? What's annoying? Adjust!

**Don't over-automate:**
Some things should stay personal (like thank you notes or referral requests). Don't automate everything!

### Common Customization Scenarios

#### Scenario 1: Add a Consultation Call

**Problem:** You always do a consultation call before quoting, but the default workflow doesn't include this.

**Solution:**
- Add "Consultation Scheduled" stage after "New Inquiry"
- Add task: "Complete consultation call with [client name]"
- Add email: "Your Consultation is Scheduled" with call details
- Manual transition to "Quoted" after call is complete

#### Scenario 2: Different Turnaround Times

**Problem:** You deliver mini sessions in 3 days but weddings take 6 weeks. Default workflow uses one timeline.

**Solution:**
- Create separate workflows: "Mini Session Workflow" and "Wedding Workflow"
- In mini session workflow: Editing task due in 3 days
- In wedding workflow: Editing task due in 6 weeks
- Assign appropriate workflow when creating job

#### Scenario 3: Album Design Phase

**Problem:** You offer albums, but the default workflow ends at gallery delivery.

**Solution:**
- Add "Album Design" stage after "Gallery Delivered"
- Entry trigger: Manual (only if client orders album)
- Add task: "Send album design draft to client"
- Add task: "Make revisions based on feedback"
- Add email: "Your Album Proof is Ready for Review"
- Exit trigger: Album approved and sent to print

#### Scenario 4: Team Member Tasks

**Problem:** You have an editor who handles post-processing, but tasks are assigned to you.

**Solution:**
- Edit "Editing" stage
- Change task assignment from "Job Owner" to specific team member (your editor)
- Add internal email: Notify editor when session is complete and files are uploaded
- Editor marks task complete when editing is done, triggering next stage

#### Scenario 5: Multiple Follow-Ups for High-Value Leads

**Problem:** Wedding inquiries are high-value, so you want more persistent follow-up than the default 2 attempts.

**Solution:**
- Clone Lead Workflow → "Wedding Lead Workflow"
- Add follow-up #3 at 12 days
- Add follow-up #4 at 18 days
- Extend "mark as lost" deadline to 21 days
- Use this workflow only for wedding inquiries

### Troubleshooting Custom Workflows

**Emails not sending?**
- Check email template exists
- Verify trigger conditions are met
- Confirm email integration is working (Settings > Integrations)

**Tasks not appearing?**
- Check task creation trigger (is the condition met?)
- Verify stage was entered correctly
- Ensure due date calculation is valid

**Workflow stuck in a stage?**
- Check exit trigger—is condition met?
- Manually advance if needed (you're always in control)
- Review transition rules

**Too many tasks?**
- Simplify! You don't need a task for every tiny action
- Focus on key milestones
- Combine related tasks

**Clients confused by emails?**
- Review email templates for clarity
- Make sure emails include context (what, why, next steps)
- Consider fewer but more meaningful emails

### Measuring Workflow Effectiveness

After customizing, track whether your changes are helping:

**Lead conversion rate:**
Did customized follow-up timing improve booking rates?

**Time saved:**
Are you spending less time on admin tasks?

**Client satisfaction:**
Do clients comment on how organized and professional you are?

**Completion rate:**
Are jobs moving through stages faster?

**Task completion:**
Are you actually completing tasks, or do they pile up? (If piling up, simplify!)

### What's Next?

Now that you know how to customize workflows, explore these topics:

**[Workflow Tasks](./workflow-tasks)** - Deep dive into task creation, assignment, and management

**[Email Automation](./email-automation)** - Master automated email sequences and templates

**[Default Workflows](./default-workflows)** - Review the built-in workflows to understand the foundation

**[Email Templates](../email-templates/)** - Create the email templates used in your custom workflows

---

**Questions?** Look for the help links throughout ShootPath, or use the support widget if you need assistance!
