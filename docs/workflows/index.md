---
sidebar_position: 1
---

# Workflows Overview

## Quick Reference

Workflows in ShootPath automate your business processes from inquiry to delivery. They're like having a personal assistant who reminds you what to do next, sends emails at the right time, and keeps your projects moving forward.

**What Workflows Do:**
- **Automate emails** - Send booking confirmations, reminders, and follow-ups automatically
- **Create tasks** - Generate checklists for each stage of your process
- **Track progress** - See exactly where each job or lead stands
- **Ensure consistency** - Never forget a step or miss a deadline

**Two Types of Workflows:**
- **Lead workflows** - Guide inquiries from first contact to booking
- **Job workflows** - Manage projects from contract signing to final delivery

**Quick Access:**
- View/edit workflows in **Settings > Workflows**
- See job workflow progress in each job's Workflow tab
- See lead workflow progress in each lead's detail page

**Key Benefits:**
- Save time by automating repetitive tasks
- Improve client experience with timely communication
- Never forget important steps
- Scale your business without working more hours

**Articles in This Section:**
- [Default Workflows](./default-workflows) - ShootPath's built-in workflows for leads and jobs
- [Customizing Workflows](./customizing-workflows) - Create and modify workflows for your process
- [Workflow Tasks](./workflow-tasks) - Understanding automatic task generation
- [Email Automation](./email-automation) - Setting up automated email sequences

---

## Detailed Guide

### What Are Workflows?

Think of a workflow as your business process mapped out step-by-step. Every time you work with a client, you probably do similar things in a similar order:

**For leads:**
1. Receive inquiry
2. Respond within 24 hours
3. Send quote
4. Follow up if no response
5. Either book them or mark as lost

**For jobs:**
1. Send contract
2. Collect deposit
3. Send questionnaire
4. Confirm session details
5. Conduct shoot
6. Edit photos
7. Deliver gallery
8. Collect final payment

These repeating processes are perfect candidates for automation. Instead of remembering "Oh, I need to send a questionnaire" or "Time to follow up on that contract," workflows do it for you!

### Why Workflows Matter

**Consistency**

Every client gets the same professional experience. You won't forget to send a booking confirmation to one client just because you were busy. The workflow ensures everyone gets the same touchpoints.

**Efficiency**

Instead of manually checking "who needs a follow-up email today?" your workflow tasks tell you exactly what needs to happen. This saves hours of mental energy every week.

**Scalability**

When you're managing 3 clients, it's easy to keep everything in your head. When you're managing 15 active jobs, workflows become essential. They help you scale without working 80-hour weeks.

**Professionalism**

Clients notice when you're on top of things. Automated confirmations, timely reminders, and consistent follow-through make you look organized and professional—because you are!

**Peace of Mind**

Ever wake up at 3am thinking "Did I send that reminder email?" With workflows, you know the system has you covered. You can focus on creative work instead of administrative anxiety.

### How Workflows Work

Let's break down the components that make workflows powerful.

#### Workflow Stages

Every workflow is divided into stages that represent key phases of your process.

**Lead workflow stages (example):**
- New Inquiry
- Quoted
- Follow-Up
- Booked or Lost

**Job workflow stages (example):**
- Contract Pending
- Deposit Pending
- Pre-Session Prep
- Session Complete
- Editing
- Gallery Delivered
- Final Payment
- Complete

Each stage represents a distinct phase with specific actions needed. When one stage completes, the workflow automatically moves to the next stage.

#### Stage Transitions

Transitions define what moves a lead or job from one stage to the next.

**Manual transitions:**
You click "Mark as Complete" on a task, or change the status manually.

**Automatic transitions:**
The system detects a change (contract signed, payment received) and automatically advances the workflow.

**Example:**
When a client signs their contract, the workflow automatically:
- Marks the "Contract Pending" stage complete
- Moves to "Deposit Pending" stage
- Sends a deposit invoice email
- Creates a task: "Follow up if deposit not paid within 3 days"

#### Automated Emails

Each workflow stage can trigger automatic emails based on specific conditions.

**Examples:**
- **Quote sent** → Send email with quote link and "here's what's included" message
- **Contract signed** → Send "Thanks for signing! Here's your deposit invoice" email
- **3 days after quote with no response** → Send "Just checking in!" follow-up email
- **Gallery uploaded** → Send "Your photos are ready!" notification

These emails use templates you customize with your voice and brand. They include dynamic content like client names, dates, and links.

#### Workflow Tasks

Tasks are the action items that guide you through each stage.

**Examples:**
- "Send booking confirmation email"
- "Confirm session date and location with client"
- "Edit photos"
- "Create gallery"
- "Follow up on unsigned contract"

Tasks can be:
- **Automatic** - Created by the workflow when you reach a stage
- **Manual** - You add them as needed for specific jobs
- **Recurring** - Repeat for every job (like "send thank you card after delivery")
- **Conditional** - Only appear if certain conditions are met (like "collect final payment" only if balance is outstanding)

### Default vs. Custom Workflows

ShootPath comes with sensible default workflows that work for most photographers. But you can customize them to match your specific process.

#### Default Workflows

Out of the box, you get:

**Lead Workflow:**
- New → Quoted → Follow-Up → Won/Lost
- Automated quote emails and follow-up reminders
- Tasks for responding quickly and tracking quote status

**Job Workflow:**
- Contract → Deposit → Pre-Session → Session → Editing → Delivery → Complete
- Automated booking confirmations, questionnaires, and gallery notifications
- Tasks for each major milestone

These defaults are based on common photography business practices. Many photographers use them as-is!

#### Custom Workflows

You can create custom workflows for different types of photography:

**Wedding Workflow** (more complex):
- Engagement session planning stage
- Multiple payment milestones
- Timeline coordination tasks
- Vendor communication reminders
- Album design phase

**Mini Session Workflow** (streamlined):
- Skip the contract (signed during booking)
- Single payment upfront
- Quick 1-week delivery timeline
- Automated print sales follow-up

**Commercial Workflow** (formal):
- SOW (statement of work) instead of contract
- Net 30 payment terms
- Usage rights documentation
- More formal communication templates

[Learn how to create custom workflows →](./customizing-workflows)

### Workflow Triggers

Triggers are the "if this happens, do that" logic behind workflows.

#### Time-Based Triggers

**Relative to an event:**
- 3 days after quote sent → Send follow-up email
- 1 week before session → Send "getting excited!" reminder
- 2 weeks after gallery delivered → Send print sales follow-up

**Absolute dates:**
- 30 days after job created → Check if job is progressing normally
- On session date → Send "good luck today!" message

#### Action-Based Triggers

**Client actions:**
- Quote accepted → Send contract and create job
- Contract signed → Send deposit invoice
- Payment received → Send receipt and next steps
- Gallery viewed → Track engagement

**Your actions:**
- Mark task complete → Move to next workflow stage
- Upload gallery → Send client notification
- Change job status → Trigger appropriate emails

**System actions:**
- Payment due date passes → Send overdue reminder
- Quote expires → Mark lead as lost (optionally)
- Session date arrives → Update job status

### Real-World Workflow Examples

Let's look at how workflows actually work in practice.

#### Example 1: Lead Converts to Booking

**Initial state:**
- Sarah inquires about wedding photography
- You create a lead for Sarah
- Lead workflow begins in "New Inquiry" stage

**Day 0 - Quote sent:**
- You send Sarah a quote
- Workflow moves to "Quoted" stage
- Automatic email: "Here's your custom quote!"
- Task created: "Follow up if no response by Day 5"

**Day 3:**
- Sarah hasn't viewed the quote yet
- Task reminder: "Check in with Sarah"

**Day 5:**
- Sarah still hasn't responded
- Automatic email: "Just wanted to make sure you received the quote!"
- Task created: "Final follow-up on Day 10"

**Day 7:**
- Sarah accepts the quote! 🎉
- Lead marked as "Won"
- Job automatically created
- Job workflow begins in "Contract Pending" stage
- Automatic email: "So excited to work with you! Please sign your contract"
- Contract link sent to Sarah

**Day 8:**
- Sarah signs the contract
- Workflow moves to "Deposit Pending" stage
- Automatic email: "Contract signed! Here's your deposit invoice"
- Deposit invoice link sent

**Day 9:**
- Sarah pays deposit
- Workflow moves to "Pre-Session Prep" stage
- Task created: "Send questionnaire"
- Task created: "Confirm session date/location"

From here, the workflow continues through the entire job lifecycle—all with minimal manual work from you!

#### Example 2: Portrait Session Workflow

**Week 1 - Booking:**
- Client accepts quote for family portrait session
- Job created with "Portrait Session" workflow
- Automatic email: "Booking confirmed! Session is [date] at [time]"
- Contract sent automatically
- Task: "Follow up if contract not signed within 3 days"

**Week 2 - Pre-Session:**
- Contract signed, deposit paid
- Automatic email: "Please fill out your questionnaire" with link
- Task: "Confirm location and wardrobe suggestions with client"
- Automatic email (7 days before session): "Session coming up! Here's what to expect"

**Week 3 - Session Day:**
- Session happens (you mark it complete in the app)
- Workflow moves to "Editing" stage
- Task: "Edit photos (due in 2 weeks)"
- Automatic email to client: "Session was wonderful! Photos will be ready in 2 weeks"

**Week 4 - Editing Complete:**
- You upload gallery
- Workflow moves to "Gallery Delivered" stage
- Automatic email: "Your gallery is ready! View and download your photos"
- Task: "Follow up if final payment not received within 5 days"

**Week 5 - Final Payment:**
- Client pays balance
- Workflow moves to "Complete" stage
- Automatic email: "Thank you for trusting me with your family portraits!"
- Task: "Send thank you card and request review"

**Week 6 - Follow-Up:**
- Task reminder: "Reach out about print products"
- Job marked complete

This entire workflow happened mostly automatically, with you only handling the creative work and a few manual tasks. That's the power of workflows!

### Getting Started with Workflows

If you're new to workflows, here's how to start:

#### Step 1: Use the Defaults

Don't overthink it initially! Start with ShootPath's default workflows. They're based on what works for most photographers, so they'll get you 80% of the way there.

#### Step 2: Track What's Missing

As you work through jobs, note when you think "I wish the workflow reminded me to..." or "I always do X but the workflow doesn't include it."

#### Step 3: Customize Gradually

After a few weeks, customize your workflows to match your actual process. Add stages, tasks, or emails that reflect how you really work.

#### Step 4: Create Specialized Workflows

Once you're comfortable, create custom workflows for specific types of photography (weddings vs. portraits vs. commercial).

:::tip Start Simple
You can always add complexity later. Start with basic workflows and let them evolve as you understand what you actually need!
:::

### Common Workflow Patterns

Here are workflow patterns that work well for most photographers.

#### The "Booking Funnel" Pattern (Leads)

**Purpose:** Convert inquiries to bookings systematically

**Stages:**
1. New Inquiry → Respond within 24 hours
2. Quoted → Follow up every 3-5 days
3. Won → Convert to job, celebrate!
4. Lost → Learn and move on

**Key emails:**
- Quote sent with enthusiasm and next steps
- Follow-up #1: "Any questions?"
- Follow-up #2: "Quote expires soon!"
- Won: "So excited to work with you!"

**Why it works:** Balances persistence with professionalism, ensuring no lead falls through the cracks.

#### The "Booking to Session" Pattern (Jobs)

**Purpose:** Get from contract to successful shoot

**Stages:**
1. Contract Pending → Get signature
2. Deposit Pending → Collect payment
3. Pre-Session Prep → Questionnaire, confirm details
4. Session Day → Execute the shoot

**Key emails:**
- Contract sent with clear next steps
- Deposit invoice after contract signed
- Questionnaire 2-3 weeks before session
- Reminder 1 week before session

**Why it works:** Clear milestones ensure nothing is forgotten before the session.

#### The "Delivery & Close" Pattern (Jobs)

**Purpose:** Deliver gallery and complete the job

**Stages:**
1. Editing → Get photos ready
2. Gallery Delivered → Send notification
3. Final Payment → Collect balance
4. Complete → Close and follow up

**Key emails:**
- "Photos coming soon!" after session
- "Gallery ready!" with link
- "Payment due" if not paid
- "Thank you!" after completion

**Why it works:** Keeps clients informed and ensures they're delighted with the final delivery.

### Workflow Best Practices

**Be Client-Centric**

Design workflows from your client's perspective. What information do they need at each stage? What would make their experience better?

**Set Realistic Timelines**

Don't promise 1-week turnaround if you need 3 weeks. Build realistic buffer time into your workflow stages.

**Communicate Proactively**

Clients should never wonder "Where are my photos?" Your workflow should keep them informed automatically.

**Keep It Simple**

Complicated workflows with 15 stages and 50 tasks are overwhelming. Start simple and add complexity only if needed.

**Review and Refine**

Every few months, review your workflows. What's working? What's annoying? What could be automated better?

**Personalize When It Matters**

Automated emails are great, but personal touches matter. Add a quick personal line to automated messages when you have time.

**Test Before Activating**

Before rolling out a new workflow, test it with a "test job" to make sure emails send correctly and tasks appear as expected.

### Measuring Workflow Effectiveness

How do you know if your workflows are working?

**Lead Conversion Rate**

Are your lead workflows helping you book more clients? Track conversion rate before and after implementing workflows.

**Response Time**

Workflows should help you respond faster. Measure average time from inquiry to quote, or from contract sent to signature.

**Client Satisfaction**

Do clients comment on how organized and professional you are? That's a sign workflows are improving their experience.

**Time Saved**

Track how much time you spend on administrative tasks. Good workflows should reduce admin time by 30-50%.

**Completion Rate**

Are you marking jobs complete faster? Are fewer jobs getting stuck in limbo? Workflows should keep things moving.

**Email Open Rates**

Check which automated emails clients are opening and which they ignore. Refine messaging based on engagement.

### Workflows and Team Collaboration

If you have a team (assistants, second shooters, editors), workflows become even more valuable.

**Task Assignment**

Assign specific workflow tasks to team members:
- "Email client" → You
- "Edit photos" → Your editor
- "Create gallery" → Your assistant

**Visibility**

Everyone sees the same workflow progress, so there's no confusion about where each job stands.

**Consistency**

Team members follow the same process regardless of who's handling the job, ensuring consistent client experience.

**Communication**

Task comments let team members communicate about specific steps without cluttering email or texts.

[Learn more about team features →](../team/)

### Troubleshooting Workflows

**Workflow not advancing automatically?**

Check if the trigger condition is met. For example, "move to Deposit Pending after contract signed" won't work if the contract isn't actually marked as signed in the system.

**Emails not sending?**

Verify your email settings in Settings > Integrations > Email. Make sure your SMTP or Gmail integration is working.

**Too many tasks?**

Simplify your workflow. You don't need a task for every tiny action—focus on key milestones.

**Clients confused by automated emails?**

Review your email templates. Make sure they're clear, friendly, and include all necessary context.

**Workflow feels too rigid?**

Remember: workflows guide you, but you're always in control. Skip tasks, move stages manually, or pause automation when needed.

### What's Next?

Ready to dive deeper into workflows? Explore these articles:

**[Default Workflows](./default-workflows)** - Learn about ShootPath's built-in lead and job workflows

**[Customizing Workflows](./customizing-workflows)** - Create workflows that match your specific business process

**[Workflow Tasks](./workflow-tasks)** - Master automatic task creation and management

**[Email Automation](./email-automation)** - Set up email sequences that nurture clients automatically

Or explore related topics:

**[Email Templates](../email-templates/)** - Create the email templates used in workflows

**[Jobs Overview](../jobs/)** - Understand how workflows integrate with job management

**[Leads Overview](../leads/)** - See how workflows help convert inquiries to bookings

---

**Questions?** Look for the help links throughout ShootPath, or use the support widget if you need assistance!
