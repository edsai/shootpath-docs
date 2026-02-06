---
sidebar_position: 3
---

# Job Workflows

## Quick Reference

Workflows are automated task checklists that guide you through each job from booking to delivery. Think of them as your process, formalized and tracked in ShootPath.

**How Workflows Work:**

- Each job type (wedding, portrait, event) has a default workflow
- Workflows consist of tasks that trigger at specific milestones
- Tasks can be manual to-dos or automatic actions (emails, contract generation)
- Mark tasks complete as you go to track progress
- Customize workflows in Settings to match your process

**Example Portrait Workflow:**
1. ✅ Quote Accepted
2. 📧 Send Contract
3. ⏳ Await Contract Signature
4. 💳 Deposit Payment Received
5. 📋 Send Client Questionnaire
6. 📸 Confirm Session Details
7. 📸 Conduct Photo Session
8. 🎨 Edit Photos
9. 📤 Deliver Gallery
10. ✅ Job Complete

**Benefits:**
- Never forget important steps in your process
- Consistent client experience across all jobs
- See at-a-glance where each job stands
- Automated reminders and actions

**Next Steps:** Learn how to [work with workflow tasks](#working-with-tasks) and [customize workflows](#customizing-workflows) for your business.

---

## Detailed Guide

### What Are Workflows?

A workflow is a series of tasks that need to happen for a job, in a specific order, often triggered by certain events. It's your standard operating procedure, but automated and tracked.

**Without workflows:**
- You rely on memory or manual checklists
- Easy to forget steps like "send questionnaire" or "confirm final details"
- Inconsistent experience for clients
- Hard to see progress across multiple jobs

**With workflows:**
- Every job follows your proven process automatically
- ShootPath prompts you at the right time for each step
- Clients get a consistent, professional experience
- You can see exactly where each job stands in the pipeline

### How Workflows are Assigned

When a job is created (either from an accepted quote or manual creation), ShootPath automatically assigns the appropriate workflow based on the job type:

- **Wedding jobs** → Wedding workflow
- **Portrait jobs** → Portrait workflow
- **Event jobs** → Event workflow
- **Maternity jobs** → Maternity workflow
- **Custom job types** → Default workflow (or custom if you've created one)

You can also change a job's workflow manually if needed (e.g., a portrait client upgrades to a more complex package).

### Workflow Tasks

Tasks are the individual steps in a workflow. Each task has:

**Task Name** - What needs to be done (e.g., "Send Booking Confirmation")

**Task Type:**
- **To-Do** - Manual action you need to take
- **Auto Email** - Automatically sends an email when triggered
- **Auto Contract** - Automatically generates and sends the contract
- **Auto Questionnaire** - Sends a questionnaire to the client
- **Milestone** - Marks a significant event (e.g., "Session Completed")

**Trigger:**
- **Job Created** - Task activates when job is created
- **Quote Accepted** - When client accepts quote
- **Contract Signed** - After client signs contract
- **Payment Received** - When a payment comes in
- **All Due Paid** - When all currently due invoices are paid
- **Session Date** - On or near the session date
- **Task Completed** - When a previous task is marked complete
- **Manual** - You trigger it manually when ready

**Status:**
- **Pending** - Not started yet (waiting for trigger)
- **Due** - Trigger has occurred, action is needed
- **Completed** - Task is done
- **Skipped** - Task was skipped (optional tasks or changed plans)

**Dependencies** - Some tasks must be completed before others unlock

:::tip Workflow Visualization
The workflow tab in each job shows a visual progress indicator—see how far along you are at a glance!
:::

### Working with Tasks

#### Viewing Tasks

Open any job and go to the **Workflow** tab. You'll see:

- List of all tasks in the workflow
- Current status of each (pending, due, completed, skipped)
- Progress bar showing percentage complete
- Quick actions for each task

Tasks are typically shown in chronological order, matching the flow of your process.

#### Marking Tasks Complete

When you finish a task, mark it complete:

1. Find the task in the workflow list
2. Click the checkbox or "Mark Complete" button
3. Optionally add a note (e.g., "Sent booking confirmation via email")
4. Task status changes to completed ✅
5. Progress bar updates

**When to mark tasks complete:**
- As soon as you finish the action
- Don't wait—mark it immediately while it's fresh
- If a task has multiple sub-actions, complete it when ALL are done

**Why it matters:**
- Keeps you organized and focused on what's next
- Shows clients (via portal) that things are progressing
- Helps you see stuck jobs (tasks not progressing)

#### Skipping Tasks

Sometimes a task doesn't apply to a specific job. You can skip it:

**Reasons to skip:**
- Client doesn't want a questionnaire (rare, but happens)
- Task was already handled outside ShootPath
- Job changed and task no longer applies
- Workflow has optional tasks

**How to skip:**
1. Find the task
2. Click "Skip Task" or similar action
3. Optionally add a reason
4. Task is marked skipped and won't block progress

Skipped tasks don't count toward completion percentage.

:::warning Use Sparingly
Only skip tasks if truly unnecessary. If you find yourself skipping the same task repeatedly, customize the workflow to remove it instead!
:::

#### Automatic Tasks

Some tasks execute automatically when triggered. You don't need to do anything—ShootPath handles it.

**Auto Email Example:**

**Task:** "Send Booking Confirmation"
**Trigger:** Contract Signed
**Action:** Email sent to client with booking details

When the trigger occurs (client signs contract), the email is automatically sent and the task is marked complete. You get a notification, but no manual action required!

**Auto Contract Example:**

**Task:** "Generate Contract"
**Trigger:** Quote Accepted
**Action:** Contract created from template and sent to client

The moment a client accepts the quote, ShootPath creates the contract and sends it for signing. You just need to wait for the client to sign.

**Benefits of automatic tasks:**
- Instant response (client gets booking confirmation immediately)
- No manual work for you
- Consistent timing (emails always sent at the right moment)
- Reduces human error (won't forget to send)

### Task Dependencies

Some tasks depend on others being completed first. You can't start editing photos before the session happens!

**Example dependencies:**

- "Send Contract" → Must happen before "Await Contract Signature"
- "Contract Signed" → Must happen before "Accept Deposit"
- "Session Completed" → Must happen before "Edit Photos"
- "Edit Photos" → Must happen before "Deliver Gallery"

Dependencies are shown visually in the workflow. Locked tasks (not yet available) appear grayed out or with a lock icon until the previous task is complete.

**Why dependencies matter:**
- Enforce logical order of operations
- Prevent mistakes (can't deliver gallery if session hasn't happened!)
- Guide you through the process step-by-step

### Common Workflow Patterns

Different photography types have different typical workflows. Here are common patterns:

#### Portrait Session Workflow

**Pre-Session:**
1. Quote Accepted → Job Created
2. Contract Generated & Sent
3. Await Contract Signature
4. Deposit Invoice Sent
5. Await Deposit Payment
6. Send Booking Confirmation (auto email)
7. Send Client Questionnaire
8. Confirm Session Details (date, location, what to wear)

**Session & Delivery:**
9. Conduct Photo Session
10. Edit Photos
11. Create Gallery
12. Send Gallery to Client
13. Await Final Payment (if balance due)
14. Job Complete

**Timeline:** 2-6 weeks from booking to delivery

#### Wedding Workflow

**Booking Phase:**
1. Quote Accepted → Job Created
2. Contract Generated & Sent
3. Await Contract Signature
4. Retainer Invoice Sent
5. Await Retainer Payment
6. Send Booking Confirmation

**Planning Phase:**
7. Send Wedding Questionnaire
8. Schedule Planning Call
9. Receive Wedding Timeline from Client
10. Coordinate with Venue/Vendors
11. Second Payment Due (3 months before)
12. Await Second Payment

**Pre-Wedding:**
13. Final Payment Due (2 weeks before)
14. Await Final Payment
15. Confirm Wedding Day Timeline
16. Prepare Shot List
17. Confirm Arrival Time & Location

**Wedding Day & Delivery:**
18. Wedding Day Coverage
19. Deliver Sneak Peeks (1-3 days after)
20. Full Editing Process
21. Create Wedding Gallery
22. Deliver Final Gallery (4-8 weeks)
23. Follow Up for Reviews/Referrals
24. Job Complete

**Timeline:** 6-12 months from booking to delivery

#### Event Photography Workflow

**Booking Phase:**
1. Quote Accepted → Job Created
2. Contract Generated & Sent
3. Await Contract Signature
4. Full Payment Due (often upfront for events)
5. Await Payment
6. Send Booking Confirmation

**Pre-Event:**
7. Confirm Event Details (date, time, location)
8. Receive Event Schedule/Agenda
9. Coordinate with Event Organizer
10. Confirm Arrival Time

**Event & Delivery:**
11. Event Coverage
12. Deliver Preview/Highlights (same day or next day)
13. Edit Full Gallery
14. Deliver Final Gallery (1-2 weeks)
15. Job Complete

**Timeline:** 1-4 weeks from booking to delivery

### Customizing Workflows

Every photographer works differently. ShootPath lets you customize workflows to match YOUR process.

**To customize workflows:**

1. Go to **Settings > Workflows**
2. Select the job type to edit (or create a new workflow)
3. Add, remove, or reorder tasks
4. Configure triggers and dependencies
5. Save changes

**What you can customize:**

**Add tasks** - Include steps unique to your business:
- "Send Style Guide" (for weddings)
- "Schedule Wardrobe Consultation" (for styled shoots)
- "Coordinate with Hair/Makeup Artist"
- "Send Album Design Preview"
- "Ship Prints"

**Remove tasks** - If you don't use something:
- Don't send questionnaires? Remove that task
- Don't offer sneak peeks? Remove early delivery task
- Simple process? Strip down to essentials

**Reorder tasks** - Match your preferred sequence:
- Send questionnaire before or after deposit?
- Confirm details closer to or farther from session?
- Your choice!

**Configure triggers** - When should each task activate:
- Immediately when job created
- After specific events (contract signed, payment received)
- X days before session
- Manually when you're ready

**Set dependencies** - What must happen first:
- Gallery delivery requires editing to be complete
- Final payment requires sneak peeks delivered (if that's your policy)

:::tip Start Simple
Don't over-complicate your first workflows. Start with 6-8 essential tasks and add more as you identify gaps in your process.
:::

### Workflow Templates

ShootPath includes default workflow templates for common job types. These are starting points you can customize:

**Portrait Workflow (Default)**
- 8 tasks covering booking → session → delivery
- Suitable for: family portraits, senior portraits, couples sessions

**Wedding Workflow (Default)**
- 16 tasks covering booking → planning → wedding day → delivery
- Suitable for: full-day wedding coverage, elopements (simplified)

**Event Workflow (Default)**
- 10 tasks covering booking → coordination → event → fast delivery
- Suitable for: corporate events, parties, fundraisers

**Maternity Workflow (Default)**
- Similar to portrait workflow with maternity-specific touches
- Suitable for: maternity and newborn sessions

You can use these as-is or customize them. Or create entirely new workflows from scratch if your process is unique!

### Creating Custom Workflows

**When to create a custom workflow:**

- You offer a unique service not covered by defaults (e.g., boudoir, dance photography)
- Your process is significantly different from the defaults
- You want separate workflows for similar job types (e.g., "Mini Session" vs. "Full Session")

**How to create a custom workflow:**

1. Go to **Settings > Workflows**
2. Click **"Create New Workflow"**
3. Name it (e.g., "Boudoir Workflow" or "Commercial Shoot Workflow")
4. Add tasks one by one:
   - Task name
   - Task type (to-do, auto email, etc.)
   - Trigger
   - Dependencies
5. Assign to job types (select which job types use this workflow)
6. Save and activate

Now when you create jobs of that type, they'll use your custom workflow!

:::tip Workflow Versioning
If you change a workflow, existing jobs keep the old workflow version (they don't change mid-flight). Only NEW jobs get the updated workflow. This prevents disruption to active projects.
:::

### Workflow Progress Tracking

The workflow tab shows visual progress indicators:

**Progress Bar** - Percentage of tasks completed (e.g., 6 of 10 tasks = 60%)

**Status Summary:**
- X tasks completed
- Y tasks in progress
- Z tasks pending

**Estimated Timeline** - Based on typical duration for each task (if configured)

**Bottleneck Indicators** - Tasks that are overdue or stuck (warning icons)

Use this to quickly assess job health. A job with 2 of 15 tasks complete and session tomorrow? That's a red flag—something is stuck!

### Troubleshooting Workflow Issues

**Problem: Task won't mark as complete**

**Possible causes:**
- Task has dependencies that aren't complete yet
- Task is locked by workflow rules
- Browser or connection issue

**Solution:**
- Check dependencies (complete those first)
- Refresh the page
- Try from job detail view instead of list view

**Problem: Automatic task didn't execute**

**Possible causes:**
- Trigger condition not actually met
- Email template not configured
- System error

**Solution:**
- Verify trigger (did contract actually get signed? Check status)
- Go to Settings > Email Templates and ensure template exists for that task
- Check email logs (Settings > Logs) for errors
- Manually execute the task if needed

**Problem: Wrong workflow assigned to job**

**Possible causes:**
- Job type changed after creation
- Workflow configuration error
- Manual workflow override

**Solution:**
- Go to job settings and change workflow manually
- Tasks from old workflow remain; you can skip irrelevant ones
- Future jobs will use correct workflow once config is fixed

**Problem: Client says they didn't receive an email from auto task**

**Possible causes:**
- Email went to spam
- Wrong email address on file
- Email template has errors

**Solution:**
- Check client email address in their profile
- Ask them to check spam/junk folder
- Check email logs to confirm it was sent
- Resend manually if needed

### Best Practices for Workflows

**Keep it simple** - Don't create 30-task workflows. Focus on critical steps that matter most.

**Use descriptive task names** - "Send Contract" is better than "Step 2" or "Contract Stuff"

**Leverage automation** - Use auto-email and auto-contract tasks to reduce manual work

**Review and refine** - After completing a few jobs, review: Did the workflow work? What would you change?

**Communicate with clients** - Let clients know what to expect: "After signing, you'll receive a booking confirmation and questionnaire within 24 hours"

**Don't skip important tasks** - Contract signing, payment collection, session confirmation—these are critical. Don't skip them to move things faster.

**Use milestones** - Mark significant events like "Session Completed" or "Gallery Delivered" even if they don't trigger actions. They provide clear markers in the timeline.

**Set realistic triggers** - Don't auto-send a gallery 1 day after session if you need 2 weeks to edit. Set triggers that match your realistic turnaround.

**Test new workflows** - Before using a new custom workflow with real clients, test it with a dummy job to make sure tasks trigger correctly.

### Workflow Notifications

You'll receive notifications when:
- A task becomes due (trigger activated)
- An automatic task executes (so you know it happened)
- A task is overdue (you forgot to complete it)
- A client completes their part (signs contract, pays invoice, submits questionnaire)

Configure notification preferences in **Settings > Notifications** to control what you're alerted about.

:::tip Mobile Notifications
Enable push notifications on the ShootPath mobile app so you're alerted about important workflow events even when away from your desk!
:::

### Workflow Reports

In the Reports section, you can analyze workflow performance:

**Average Time to Complete** - How long does each workflow take?

**Bottleneck Analysis** - Which tasks take the longest or cause delays?

**Skip Rate** - Are certain tasks skipped often? Maybe they don't belong in the workflow.

**Completion Rate** - Do jobs make it all the way through, or do they stall?

Use these insights to refine your workflows and improve efficiency over time.

### What's Next?

Now that you understand workflows, explore related topics:

**[Timeline & Scheduling](./timeline-and-scheduling)** - Manage session dates and reminders

**[Job Files](./job-files)** - Handle files created by workflow tasks (contracts, questionnaires)

**[Managing Jobs](./managing-jobs)** - See how workflows fit into overall job management

Or dive into specific workflow components:

**[Email Templates](../email-templates/)** - Customize automated emails sent by workflow tasks

**[Contracts](../contracts/)** - Set up contract templates for auto-contract tasks

**[Questionnaires](../questionnaires/)** - Create questionnaires sent by auto-questionnaire tasks

---

**Questions?** Use the help widget in ShootPath or reach out to support for assistance with workflows!
