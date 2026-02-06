---
sidebar_position: 2
---

# Default Workflows

## Quick Reference

ShootPath comes with pre-configured workflows that work for most photography businesses right out of the box. You don't need to set anything up—just start using them!

**What's Included:**

**Lead Workflow:**
- New Inquiry → Quoted → Follow-Up → Won/Lost
- Automatic quote emails and follow-up reminders
- Tracks days pending to prompt timely follow-ups

**Job Workflow:**
- Contract Pending → Deposit → Pre-Session → Session → Editing → Delivery → Complete
- Automated booking confirmations and milestone emails
- Tasks for each major phase of the job

**Key Features:**
- Email automation at each stage
- Automatic task creation
- Smart transitions based on client actions
- Customizable to fit your process

**Quick Actions:**
- View workflows in **Settings > Workflows**
- Edit workflow stages and emails
- Enable/disable specific automation
- Clone defaults to create custom versions

:::tip Just Getting Started?
The default workflows are designed to work well for most photographers immediately. Use them as-is for your first few jobs, then customize based on your experience!
:::

---

## Detailed Guide

### Understanding Default Workflows

When you create your ShootPath account, two workflows are automatically set up and ready to use:

1. **Lead Workflow** - Manages inquiries from first contact to booking decision
2. **Job Workflow** - Manages bookings from contract signing to final delivery

These workflows were designed based on industry best practices and feedback from hundreds of photographers. They represent the "standard" process most photographers follow, with sensible automation and milestones.

**The goal:** Save you time while delivering a professional client experience. You shouldn't need to customize anything initially—the defaults should just work.

### The Default Lead Workflow

Let's walk through the lead workflow stage by stage.

#### Stage 1: New Inquiry

**When it starts:**
As soon as you create a new lead in the system.

**What happens:**
- Lead appears in your "New" leads list
- Task created: "Respond to inquiry within 24 hours"
- No automatic emails (you respond personally to the inquiry)

**Your action:**
Review the inquiry details, respond to the client with enthusiasm, ask qualifying questions (budget, timeline, vision), and gather information to create an accurate quote.

**Why no automated email here?**
First impressions matter! Your initial response should be personal and specific to their inquiry. Generic automated responses feel cold and unprofessional at this stage.

**Best practice:**
Respond within 24 hours. Studies show photographers who respond within a day are 7x more likely to book the client.

#### Stage 2: Quoted

**When it starts:**
When you send a quote to the client.

**What happens automatically:**
- Lead moves to "Quoted" status
- Email sent: "Your Custom Quote for [Job Type]"
- Task created: "Follow up if no response within 5 days"
- Tracking begins: Days pending counter starts

**The automatic email includes:**
- Direct link to view the quote
- Summary of packages offered
- Clear next steps ("Review and accept to book")
- Your contact info for questions

**Workflow logic:**
The workflow now waits for the client to respond. It tracks how many days have passed since sending the quote, which helps you prioritize follow-ups.

**Client perspective:**
They receive a professional email with a clear call-to-action. The quote link opens a beautiful, easy-to-review presentation of your packages.

#### Stage 3: Follow-Up (5 Days After Quote)

**When it triggers:**
5 days after sending the quote with no client response.

**What happens automatically:**
- Email sent: "Just Checking In - Quote for [Client Name]"
- Task created: "Follow up again if no response by day 10"
- Lead stays in "Quoted" status but flagged for attention

**The automatic follow-up email:**
- Friendly, not pushy tone
- "I wanted to make sure you received the quote..."
- "Do you have any questions?"
- Reminder that you're here to help

**Why 5 days?**
It's long enough to give them time to review without being pushy, but not so long that they've forgotten about you or booked someone else.

**Manual override:**
You can skip this automated email if you've already followed up personally, or if you know they're still deciding.

#### Stage 4: Final Follow-Up (10 Days After Quote)

**When it triggers:**
10 days after sending the quote with no response or acceptance.

**What happens automatically:**
- Email sent: "Your Quote is Expiring Soon"
- Task created: "Mark as lost if no response by day 14"
- Creates sense of urgency (quote expiration)

**The final follow-up email:**
- Mentions quote expiration date
- "I'd love to work with you!"
- Offers to jump on a call to discuss
- Last friendly prompt before closing the lead

**Why final follow-up?**
After 3 attempts (quote + 2 follow-ups), you've done your due diligence. Further follow-ups feel desperate and waste your time that could be spent on warm leads.

**What if they don't respond?**
After 14 days with no response, manually mark the lead as "Lost" and move on. Some photographers don't book—that's normal!

#### Stage 5: Won

**When it starts:**
Client accepts the quote (clicks "Accept" button).

**What happens automatically:**
- Lead marked as "Won"
- Job record created
- Job workflow begins (contract sent)
- Email sent: "You're Booked! Next Steps"
- Lead moves out of active pipeline

**The booking confirmation email:**
- Celebration of the booking ("So excited to work with you!")
- What happens next (contract, deposit, session planning)
- Link to client portal
- Your contact info for questions

**Behind the scenes:**
ShootPath creates a job record with all the details from the quote: client info, package selected, pricing, session date, and more. The job workflow immediately starts with the "Contract Pending" stage.

**Your action:**
Follow up personally to thank them and start building the relationship!

#### Stage 6: Lost

**When it starts:**
You manually mark the lead as "Lost."

**What happens:**
- Lead moves to "Lost" status
- No automatic emails
- Lead archived but preserved for data
- Workflow stops

**Why mark as lost instead of deleting?**
- They might come back later
- They might refer friends
- Historical data helps you improve conversion rate
- You can analyze why leads are lost

**When to mark lost:**
- Client explicitly says no
- 14+ days with no response after multiple follow-ups
- They booked another photographer
- Not a good fit (budget, style, etc.)

**Add a note why:**
"Went with another photographer - price was the issue" or "Needed a date I wasn't available." These notes help you identify patterns over time.

### The Default Job Workflow

Once a lead converts to a job, the job workflow takes over. Let's walk through each stage.

#### Stage 1: Contract Pending

**When it starts:**
Immediately after lead is marked "Won" and job is created.

**What happens automatically:**
- Job created in "Production" status
- Contract generated from template
- Email sent: "Please Review and Sign Your Contract"
- Task created: "Follow up if contract not signed within 3 days"

**The contract email includes:**
- Direct link to view and sign contract
- Brief overview of contract terms
- Explanation of e-signature process
- Encouragement to reach out with questions

**Workflow logic:**
The job cannot move forward until the contract is signed. This stage acts as a gatekeeper—no deposit invoice is sent until legal agreement is in place.

**Client perspective:**
They receive a clear, professional email explaining what to do next. Clicking the link takes them to a portal where they can read and sign the contract electronically.

**Your action:**
If 3 days pass without signature, the workflow task reminds you to follow up. A quick text or call often gets it done: "Hey! Just wanted to make sure you saw the contract email. Let me know if you have any questions!"

#### Stage 2: Deposit Pending

**When it starts:**
When client signs the contract.

**What happens automatically:**
- Workflow advances to "Deposit Pending"
- Deposit invoice generated based on payment schedule
- Email sent: "Contract Signed! Here's Your Deposit Invoice"
- Task created: "Follow up if deposit not paid within 5 days"

**The deposit invoice email includes:**
- Direct link to pay online
- Amount due and due date
- Accepted payment methods
- Receipt confirmation message

**Workflow logic:**
The booking isn't truly confirmed until you receive the deposit. This stage ensures you get paid before investing time in pre-session planning.

**Payment integration:**
If you've connected Stripe, clients can pay with credit/debit cards directly from the portal. Payments are marked automatically in the system.

**Your action:**
Most clients pay immediately or within 24 hours. If 5 days pass, the workflow task prompts a gentle reminder.

**What if deposit isn't paid?**
After 7-10 days without payment, reach out personally. Sometimes emails get caught in spam, or they forgot. A quick reminder usually solves it!

#### Stage 3: Pre-Session Preparation

**When it starts:**
When deposit payment is received.

**What happens automatically:**
- Workflow advances to "Pre-Session Prep"
- Email sent: "Please Complete Your Questionnaire"
- Task created: "Confirm session date and location"
- Task created: "Send questionnaire reminder if not completed within 7 days"

**The questionnaire email includes:**
- Link to online questionnaire
- Explanation of why it's important
- Deadline for completion
- Your contact info

**Workflow logic:**
This stage prepares both you and the client for a successful session. You confirm logistics, gather important details, and ensure you're aligned on vision.

**7 days before session:**
Automatic reminder email: "Session Coming Up! What to Expect"
- Weather considerations (if outdoor)
- What to bring/wear
- Timeline and location details
- Your contact info for day-of

**Your action:**
Manually confirm details 1-2 weeks before the session:
- Exact location and meeting time
- Backup plan (if weather-dependent)
- Wardrobe suggestions (if applicable)
- Any special requests or concerns

**Best practice:**
Call or text the client 1-2 days before the session for final confirmation. This reduces no-shows and makes them feel cared for!

#### Stage 4: Session Complete

**When it starts:**
You manually mark the session as complete in the app.

**What happens automatically:**
- Workflow advances to "Editing"
- Email sent: "Session Was Wonderful! Photos Coming Soon"
- Task created: "Edit photos (due in [turnaround time])"

**The post-session email includes:**
- Thank you for the session
- Estimated timeline for gallery delivery
- What to expect next
- Sneak peek photo (if you upload one)

**Workflow logic:**
This stage is all about editing. The workflow gives you a deadline based on your configured turnaround time (e.g., 2 weeks for portraits, 6 weeks for weddings).

**Your action:**
Edit the photos! The workflow task appears in your task list with a due date, so you can prioritize your editing queue.

**Turnaround time:**
Configure your default turnaround times in Settings > Workflows. Different job types can have different timelines (weddings take longer than mini sessions).

**Client communication:**
If you'll be late on delivery, send a quick update: "I'm running a few days behind due to a busy month—your gallery will be ready by [new date]. Thanks for your patience!"

#### Stage 5: Gallery Delivered

**When it starts:**
You upload and publish the gallery.

**What happens automatically:**
- Workflow advances to "Gallery Delivered"
- Email sent: "Your Gallery is Ready! 📸"
- Task created: "Follow up if final payment not received within 5 days"
- Gallery download instructions

**The gallery notification email includes:**
- Direct link to view gallery
- Download instructions
- Print ordering options (if applicable)
- Social media sharing guidelines
- Watermark/usage rights reminder

**Workflow logic:**
This is the exciting moment! The client gets their photos, and you move toward wrapping up the job.

**Final payment:**
If there's a balance due, the email includes a reminder and payment link. Most clients pay immediately upon seeing their photos!

**Your action:**
Celebrate this milestone! You've delivered the product. Now just close out any financial loose ends.

**Promotion opportunity:**
This is a great time to ask for a testimonial or referral: "If you loved your photos, I'd be so grateful if you'd leave a review or share with friends!"

#### Stage 6: Final Payment Collected

**When it starts:**
When final payment is received (if balance was due).

**What happens automatically:**
- Workflow advances to "Complete"
- Email sent: "Thank You for Your Business!"
- Task created: "Send thank you card and request review"

**The thank you email includes:**
- Gratitude for their business
- Reminder of gallery link (for their records)
- Invitation to book again in the future
- Request for review or referral

**Workflow logic:**
The job is essentially complete at this point. All deliverables are sent, all payments are collected. The only remaining action is relationship follow-up.

**Your action:**
Send a handwritten thank you card (if that's your style). Ask for a testimonial or Google review. Add them to your past client list for future marketing.

**Best practice:**
Check in with clients 2-4 weeks after delivery to see if they have questions, need additional prints, or want to book another session.

#### Stage 7: Job Complete

**When it starts:**
You manually mark the job as "Complete" after all follow-up is done.

**What happens:**
- Job status changes to "Complete"
- Job moves out of "Production" list
- Workflow ends
- Job preserved in completed jobs archive

**When to mark complete:**
- All deliverables sent
- All payments received
- No outstanding requests
- You're confident the client is satisfied

**Note:**
You can always reopen a completed job if needed (client requests additional edits, orders prints, etc.). Just change the status back to "Production."

### Workflow Transitions Explained

Understanding how and when workflows move from one stage to the next helps you see the full automation in action.

#### Automatic Transitions

**Triggered by client actions:**
- Quote accepted → Lead marked "Won," job created
- Contract signed → Job moves to "Deposit Pending"
- Payment received → Job moves to next stage

**Triggered by your actions:**
- You send quote → Lead moves to "Quoted"
- You upload gallery → Job moves to "Gallery Delivered"
- You mark session complete → Job moves to "Editing"

**Triggered by time:**
- 5 days after quote → Follow-up email sent
- 7 days before session → Reminder email sent
- Turnaround deadline → Task marked overdue

#### Manual Transitions

Some transitions require your input:

**Marking stages complete:**
You manually mark the session as complete when it happens. The workflow doesn't know when you actually did the shoot!

**Marking jobs complete:**
You decide when the entire job is finished and ready to close.

**Skipping stages:**
If a client pays the full amount upfront, you can skip the "Final Payment" stage.

**Why manual?**
Some things require your judgment. The system can't automatically know when you've finished editing or when you're truly done with a client.

### Default Email Templates

The default workflows include email templates for each stage. Here's what they cover:

**Lead Emails:**
- Quote sent confirmation
- Follow-up #1 (5 days)
- Follow-up #2 (10 days)
- Booking confirmation

**Job Emails:**
- Contract signing request
- Deposit invoice
- Questionnaire request
- Pre-session reminder (7 days before)
- Post-session thank you
- Gallery notification
- Final thank you

**Template customization:**
All templates use your business name, logo, and contact info automatically. You can edit the wording to match your voice and brand!

[Learn more about email templates →](../email-templates/)

### Default Workflow Tasks

Tasks keep you on track by reminding you what needs to happen at each stage.

**Lead Tasks:**
- Respond to inquiry within 24 hours
- Follow up if no response within 5 days
- Follow up again if no response within 10 days
- Mark as lost if no response after 14 days

**Job Tasks:**
- Follow up if contract not signed within 3 days
- Follow up if deposit not paid within 5 days
- Confirm session date and location
- Send questionnaire reminder if not completed
- Edit photos (due by [turnaround date])
- Follow up if final payment not received
- Send thank you card and request review

**Task due dates:**
Tasks include realistic due dates based on industry norms. You can always adjust dates for specific jobs if needed.

### Modifying Default Workflows

The defaults work well, but you can customize them to fit your specific process.

#### What You Can Modify

**Email timing:**
Change when follow-up emails send (e.g., 3 days instead of 5 days).

**Email content:**
Rewrite email templates in your voice and tone.

**Tasks:**
Add, remove, or modify tasks for each stage.

**Stages:**
Add custom stages (e.g., "Engagement Session" before main wedding).

**Triggers:**
Change what moves workflows from one stage to another.

#### How to Modify

1. Go to **Settings > Workflows**
2. Select "Lead Workflow" or "Job Workflow"
3. Click "Edit" on any stage
4. Make your changes
5. Save and test with a new job

:::warning Test Before Rolling Out
Before changing default workflows, test your modifications with a "test job" to ensure emails send correctly and transitions work as expected!
:::

#### Common Modifications

**Faster follow-ups:**
Some photographers prefer 3-day and 7-day follow-ups instead of 5-day and 10-day.

**Additional pre-session communication:**
Add a task to call clients 2 weeks before the session for a consultation.

**Print sales follow-up:**
Add a stage 2-3 weeks after gallery delivery to promote prints and albums.

**Mini session workflows:**
Streamline to skip questionnaires and contracts (signed in person).

**Wedding workflows:**
Add engagement session stage, timeline coordination, and album design stages.

[Learn how to customize workflows →](./customizing-workflows)

### When Default Workflows Work Best

**You're just starting out:**
Don't overthink your process yet. Use the defaults and refine as you gain experience.

**You shoot a variety of job types:**
The defaults are broad enough to work for most photography niches (portraits, events, weddings, commercial).

**You want quick setup:**
No configuration needed—just start booking clients and let the workflows guide you.

**You're focusing on other aspects:**
If you're busy marketing, shooting, or building your portfolio, let the defaults handle the admin side.

### When to Create Custom Workflows

**You have a very specific process:**
If your workflow is significantly different from the defaults (e.g., you require a consultation call before quoting), custom workflows make sense.

**Different job types need different processes:**
Weddings and mini sessions have very different workflows. Create separate workflows for each type.

**You're scaling and need automation:**
Custom workflows can automate more of your unique process, saving even more time as you grow.

**You've been using defaults for a while:**
After 2-3 months, you'll know exactly what to tweak based on real experience.

[Learn how to create custom workflows →](./customizing-workflows)

### Tips for Using Default Workflows

**Don't fight the workflow:**
If the workflow feels like it's working against you, modify it. Workflows should help, not hinder!

**Personalize automated emails:**
Even though emails are automated, you can add personal touches when you send them manually (override the automation).

**Complete tasks promptly:**
Workflows work best when you stay on top of tasks. Check your task list daily!

**Review after each job:**
After your first few jobs, review the workflow. What worked? What didn't? Adjust accordingly.

**Use notes liberally:**
Add notes to jobs about anything unusual. This helps you understand why certain workflow steps didn't apply.

### Common Questions

**Can I turn off email automation?**
Yes! In Settings > Workflows, you can disable specific automated emails while keeping the rest of the workflow active.

**Can I use different workflows for different job types?**
Absolutely! Create custom workflows for weddings, portraits, events, etc., and assign them when creating jobs.

**What if a client skips a step?**
You can manually advance the workflow even if triggers haven't fired. You're always in control!

**Can I revert to defaults after customizing?**
Yes! ShootPath keeps a copy of the default workflows. You can duplicate them anytime.

**Do workflows work with manual jobs?**
Yes! Workflows activate for jobs created manually (not just quote-accepted jobs).

### What's Next?

Now that you understand default workflows, explore these resources:

**[Customizing Workflows](./customizing-workflows)** - Learn to create workflows that match your exact process

**[Workflow Tasks](./workflow-tasks)** - Master task management and automatic task generation

**[Email Automation](./email-automation)** - Deep dive into automated email sequences

**[Email Templates](../email-templates/)** - Customize the email templates used in workflows

---

**Questions?** Look for the help links throughout ShootPath, or use the support widget if you need assistance!
