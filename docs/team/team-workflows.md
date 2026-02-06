---
sidebar_position: 4
---

# Team Workflows

## Quick Reference

When working with a team, **collaborative workflows** ensure everyone knows what to do, when to do it, and who's responsible. ShootPath's team workflow features help coordinate multiple people working on the same jobs without confusion or dropped tasks.

**What Team Workflows Enable:**
- **Task assignments** - Delegate specific tasks to specific team members
- **Visibility** - Everyone sees job progress in real time
- **Coordination** - Handoffs between team members happen smoothly
- **Accountability** - Clear ownership of each task
- **Consistency** - Every team member follows the same process

**Key Features:**
- Assign workflow tasks to team members
- Automatic task notifications
- Task comments for coordination
- Progress tracking by team member
- Team calendar view

**Common Team Workflows:**
- Wedding with second shooter
- Studio with multiple photographers
- Owner + assistant collaboration
- Multi-person production process

**Articles Referenced:**
- [Workflows Overview](../workflows/) - Understanding ShootPath's workflow system
- [Jobs Overview](../jobs/) - How job assignments work
- [Team Members](./team-members) - Adding and managing team members

---

## Detailed Guide

### What Are Team Workflows?

A **team workflow** is a series of tasks distributed across multiple people to complete a job. Instead of one person doing everything, each team member handles their specialty or assigned responsibilities.

**Example: Solo workflow (you do everything):**
1. Send quote → You
2. Send contract → You
3. Collect deposit → You
4. Confirm session details → You
5. Shoot session → You
6. Edit photos → You
7. Upload gallery → You
8. Send gallery link → You

**Example: Team workflow (distributed):**
1. Send quote → Assistant (Emma)
2. Send contract → Assistant (Emma)
3. Collect deposit → Owner (You) reviews, Emma sends invoice
4. Confirm session details → Assistant (Emma)
5. Shoot session → Photographer (Alex) + You (second shooter)
6. Edit photos → Editor (Sam)
7. Upload gallery → Assistant (Emma)
8. Send gallery link → Automatic (system sends after Emma uploads)

**Benefits:**
- **Faster turnaround** - Multiple people working in parallel
- **Specialization** - Each person does what they do best
- **Scalability** - Serve more clients without working more hours
- **Redundancy** - If someone is unavailable, someone else can step in

### How Team Workflows Work in ShootPath

ShootPath's workflow system integrates with team features:

**1. Workflows define the process:**
- Stages (Contract Pending, Editing, etc.)
- Tasks (Send contract, Edit photos, Upload gallery)
- Triggers (automatic transitions when conditions are met)

**2. Tasks are assigned to team members:**
- Default assignments based on role or job type
- Manual assignments for specific jobs
- Automatic notifications when tasks are assigned

**3. Team members see their tasks:**
- Dashboard shows "My Tasks" for each team member
- Job detail page shows all tasks and who's responsible
- Calendar shows upcoming tasks and deadlines

**4. Progress is tracked:**
- Task status (pending, in progress, complete)
- Who completed each task and when
- Bottlenecks or delays are visible to admins

### Setting Up Team Workflows

Let's walk through creating a collaborative workflow.

#### Step 1: Define Your Process

Before configuring anything in ShootPath, map out your actual process:

**Example: Wedding workflow with team**

**Pre-wedding (Admin/Assistant):**
- Send booking confirmation
- Send contract for signature
- Send deposit invoice
- Send questionnaire
- Confirm timeline and location

**Wedding day (Photographers):**
- Primary photographer shoots ceremony and portraits
- Second shooter captures details and candids

**Post-wedding (Editor + Assistant):**
- Editor edits photos
- Assistant uploads gallery
- Assistant sends gallery link

**Completion (Admin/Owner):**
- Collect final payment
- Send thank you
- Request review

**Team roles:**
- **Owner (You)** - Primary photographer, oversees everything
- **Admin (Rachel)** - Assigns jobs, handles escalations
- **Photographer (Alex)** - Second shooter
- **Assistant (Emma)** - Admin tasks, gallery uploads
- **Editor (Sam)** - Post-production (may be Assistant or Photographer role)

#### Step 2: Configure Default Task Assignments

Go to **Settings > Workflows > [Your Workflow] > Tasks**

For each task, set default assignee:

**Booking phase tasks:**
- "Send booking confirmation" → Assistant (Emma)
- "Send contract" → Assistant (Emma)
- "Follow up on unsigned contract" → Admin (Rachel)

**Pre-session tasks:**
- "Send questionnaire" → Assistant (Emma)
- "Confirm session details" → Admin (Rachel) or Owner (You)

**Session tasks:**
- "Conduct session" → Owner (You) + Photographer (Alex)

**Editing tasks:**
- "Edit photos" → Editor (Sam)
- "Upload gallery" → Assistant (Emma)

**Completion tasks:**
- "Send final payment reminder" → Assistant (Emma)
- "Request review" → Assistant (Emma)

#### Step 3: Customize Per-Job (Optional)

For specific jobs, you can override defaults:

**Example: VIP wedding**
- "Conduct session" → Owner (You) only (no second shooter)
- "Edit photos" → Owner (You) personally (not delegated to editor)

**How to customize:**
1. Open the job detail page
2. Go to Workflow tab
3. Click on a task
4. Change assignee
5. Save

#### Step 4: Enable Notifications

Ensure team members receive notifications when tasks are assigned:

**Settings > Notifications > Team Task Assignments**
- ✅ Email notification when task assigned
- ✅ In-app notification
- ⚠️ SMS notification (optional, for urgent tasks)

**Per-team member settings:**
Each team member can customize their notification preferences in their profile.

### Common Team Workflow Patterns

Here are proven team workflow patterns for different photography businesses.

---

## Pattern 1: Solo + Assistant

**Team structure:**
- You (Owner) - Photographer
- Emma (Assistant) - Admin support

**Responsibilities:**

**You:**
- Shoot all sessions
- Edit photos (or oversee editing)
- Handle complex client issues
- Make all business decisions

**Emma:**
- Send quotes and follow up on leads
- Send contracts and invoices
- Manage client communication (scheduling, reminders)
- Upload galleries
- Send automated emails

**Workflow task assignments:**

| Task | Assignee |
|------|----------|
| Send quote | Emma |
| Follow up on quote | Emma |
| Send contract | Emma |
| Follow up on contract | Emma |
| Send deposit invoice | Emma |
| Send questionnaire | Emma |
| Confirm session details | You |
| Conduct session | You |
| Edit photos | You |
| Upload gallery | Emma |
| Send gallery link | Automatic (after Emma uploads) |
| Send final payment reminder | Emma |
| Request review | Emma |

**Handoffs:**
- Emma → You: "Client signed contract, confirmed session details"
- You → Emma: "Shoot complete, edited photos ready for upload"
- Emma → You: "Gallery uploaded, client notified"

**Communication:**
- Emma adds notes to job: "Client prefers natural light"
- You add notes: "Bring extra flash, venue is dark"
- Use task comments for questions

**Benefits:**
- You focus on creative work
- Emma handles all admin (20+ hours/week saved)
- Clients get fast responses even when you're shooting

---

## Pattern 2: Wedding with Second Shooter

**Team structure:**
- You (Owner) - Primary photographer
- Alex (Photographer) - Second shooter
- Emma (Assistant) - Admin support

**Responsibilities:**

**You:**
- Primary photographer for wedding
- Direct the timeline and poses
- Edit photos
- Oversee the entire job

**Alex:**
- Second shooter for ceremony, reception, details
- Capture candids and alternative angles
- Deliver raw files to you for editing
- Does NOT communicate with client directly (unless needed)

**Emma:**
- Same as Pattern 1 (all admin tasks)

**Workflow task assignments:**

| Task | Assignee |
|------|----------|
| Send booking confirmation | Emma |
| Conduct session | You + Alex |
| Edit photos | You |
| Upload gallery | Emma |
| All other tasks | Same as Pattern 1 |

**Wedding day coordination:**
- Both you and Alex see the job on your calendars
- Job detail page shows timeline, location, client preferences
- Alex logs in to ShootPath mobile app, sees all details
- After shoot, Alex uploads raw files or delivers via Dropbox (outside ShootPath)

**Benefits:**
- Cover more ground at weddings
- Accept bookings that require two photographers
- Alex sees only this job (privacy for your other clients)

---

## Pattern 3: Multi-Photographer Studio

**Team structure:**
- You (Owner) - Business owner, occasional photographer
- Rachel (Admin) - Studio manager
- Jordan (Photographer) - Associate photographer
- Alex (Photographer) - Associate photographer
- Sam (Photographer) - Associate photographer
- Emma (Assistant) - Admin support

**Responsibilities:**

**You:**
- Oversee business strategy
- Shoot VIP clients
- Handle escalations
- Manage billing

**Rachel:**
- Assign incoming jobs to photographers
- Monitor all job progress
- Handle client escalations
- Manage team schedules

**Jordan, Alex, Sam:**
- Manage their assigned jobs independently
- Shoot sessions
- Edit photos (or coordinate with external editor)
- Upload galleries
- Communicate with assigned clients

**Emma:**
- Send quotes to leads (before jobs are assigned)
- Upload galleries for any photographer who prefers support
- General admin tasks

**Workflow task assignments:**

**Lead phase (before job created):**
- Rachel assigns lead to a photographer based on availability and specialty
- Photographer sends quote

**After quote accepted:**
- Job created and assigned to photographer
- Photographer manages entire job (contract, deposit, session, editing, delivery)

**Handoffs:**
- Rachel → Photographer: "You're assigned to this new booking"
- Photographer → Rachel: "Gallery delivered, job complete"

**Benefits:**
- Studio can handle 20+ simultaneous jobs
- Each photographer runs their jobs independently
- Rachel keeps everyone aligned
- You focus on growth, not daily operations

---

## Pattern 4: Owner + Editor + Assistant

**Team structure:**
- You (Owner) - Photographer
- Sam (Editor) - Post-production specialist
- Emma (Assistant) - Admin support

**Responsibilities:**

**You:**
- Shoot all sessions
- Select/cull photos
- Final review of edited photos
- Client relationships

**Sam:**
- Edit photos (color correction, retouching, etc.)
- Create gallery-ready JPEGs
- Deliver edited files for upload

**Emma:**
- All admin tasks (booking, scheduling, invoicing)
- Upload galleries
- Client communication

**Workflow task assignments:**

| Task | Assignee |
|------|----------|
| Pre-session tasks | Emma |
| Conduct session | You |
| Cull photos | You |
| Edit photos | Sam |
| Review edited photos | You |
| Upload gallery | Emma |
| Post-delivery tasks | Emma |

**Handoffs:**
- You → Sam: "Raw files ready for editing" (via Dropbox or ShootPath file sharing)
- Sam → You: "Edited photos ready for review"
- You → Emma: "Approved, ready to upload"
- Emma → Client: "Gallery ready!" (automatic email)

**Communication:**
- You add notes: "Client wants natural tones, minimal retouching"
- Sam adds notes: "Edited 250 photos, flagged 10 for additional retouching"
- Emma adds notes: "Client loved the gallery, requested 5 additional prints"

**Benefits:**
- You focus on shooting and client relationships
- Sam specializes in editing (faster and higher quality)
- Emma handles all non-creative tasks
- End-to-end process is seamless for clients

---

## Task Assignment Best Practices

### Assign Tasks to the Right Person

**Match tasks to skills and permissions:**

**Owner/Admin tasks:**
- Strategic decisions (pricing, workflows, policies)
- Financial oversight (review payments, process refunds)
- Team management (hiring, performance reviews)

**Photographer tasks:**
- Shooting sessions
- Editing (if they have editing skills)
- Client communication for their assigned jobs

**Assistant tasks:**
- Repetitive admin (send emails, upload galleries)
- Scheduling and coordination
- Data entry

### Use Default Assignments

Configure default task assignments in **Settings > Workflows** so every job starts with the right person assigned to each task.

**Benefits:**
- Consistency across all jobs
- Reduces manual assignment work
- New team members know their responsibilities

**Override when needed:**
For specific jobs, you can always reassign tasks manually.

### Notify Team Members

When you assign a task to someone, they should know immediately:

**Enable notifications:**
- **Settings > Notifications > Task Assignments**
- Team members receive email or in-app notification
- Notification includes job name, client, and task description

**Include deadlines:**
- Set due dates for tasks
- Team members see tasks sorted by due date
- Overdue tasks are highlighted

### Use Task Comments

Task comments let team members communicate about specific tasks without cluttering email or texts:

**Example:**
- **Emma (Assistant):** "Sent contract to client, waiting for signature"
- **Rachel (Admin):** "Client called, said they have questions. Can you follow up?"
- **Emma:** "Called client, answered questions, they're signing today"

**Benefits:**
- Context stays with the task
- Everyone assigned to the job sees the conversation
- Historical record for future reference

### Monitor Task Completion

**For Admins and Owners:**

Use the **Tasks Dashboard** to see:
- All open tasks across all jobs
- Who's assigned to each task
- Which tasks are overdue
- Team member workload (how many tasks each person has)

**Identify bottlenecks:**
- If Sam (Editor) has 15 open editing tasks, they're overloaded
- If Emma (Assistant) has no tasks, redistribute work

**Intervene when needed:**
- Reassign tasks if someone is overwhelmed
- Follow up on overdue tasks
- Provide support if someone is stuck

---

## Team Calendar Coordination

Team workflows require coordinating schedules. ShootPath's team calendar helps.

### Shared Calendar View

**Access:** Go to **Calendar**

**What you see:**
- All team members' jobs in one view
- Color-coded by photographer (You = Blue, Alex = Green, etc.)
- Session dates, times, and locations
- Avoid double-booking

**Use cases:**
- "Can Alex shoot a wedding on June 15?" (Check calendar, see if Alex is available)
- "When are we all free for a team meeting?" (Find a gap in the schedule)

### Individual Calendars

Each team member has their own calendar feed (iCal or Google Calendar subscription):

**Access:** Settings > Profile > Calendar Feed

**What they see:**
- Only their assigned jobs
- Session dates, deadlines, and tasks due
- Syncs to their personal calendar

**Benefits:**
- Photographers see their schedule in their phone's calendar app
- No need to log into ShootPath to check what's coming up
- Automatic updates when jobs are assigned/reassigned

### Avoiding Conflicts

**Before assigning a job:**
1. Check team calendar for availability
2. Verify photographer isn't already double-booked
3. Assign job to available photographer

**If conflicts arise:**
- System warns: "Alex is already booked on this date"
- Reassign to someone else or reschedule

---

## Handoffs and Communication

Team workflows require smooth handoffs between team members.

### What is a Handoff?

A **handoff** is when one team member completes their task and the next person takes over.

**Example handoffs:**
- Emma (Assistant) sends contract → Client signs → You (Owner) conducts session
- You shoot session → Sam (Editor) edits photos → Emma uploads gallery
- Emma uploads gallery → System sends notification → Client views gallery

### Making Handoffs Smooth

**1. Clear task completion:**
Mark tasks complete as soon as you finish them. This signals the next person to start.

**2. Add handoff notes:**
When completing a task, add a note for the next person:
- "Contract signed, session confirmed for June 15 at 2pm"
- "Edited 200 photos, uploaded to Dropbox folder 'Johnson Wedding'"
- "Gallery uploaded, client notified via email"

**3. Use task assignments:**
When you complete your task, the next task should automatically be assigned to the right person (via workflow configuration).

**4. Communicate delays:**
If you can't complete your task on time, notify the team:
- Add task comment: "Behind on editing, will deliver by Friday instead of Wednesday"
- Notify admin so they can update client

### Internal vs. Client-Facing Communication

**Internal communication (team members only):**
- Task comments
- Job notes (marked "internal")
- Direct messages (if ShootPath has messaging feature)

**Client-facing communication:**
- Automated emails (triggered by workflow)
- Manual emails sent via ShootPath
- Portal messages

**Keep internal communication internal:**
- Don't add sensitive notes where clients can see them
- Use "internal notes" for candid team discussion
- Send formal emails to clients via ShootPath (use templates for consistency)

---

## Second Shooter Workflows

Second shooter scenarios require special coordination.

### Assigning a Second Shooter to a Job

**Option 1: Assign to the job**
1. Open job detail page
2. Click "Assign Team Member"
3. Select Alex (Photographer)
4. Save

Alex now sees the job and all its details.

**Option 2: Assign to specific tasks**
1. Open job detail page
2. Go to Workflow tab
3. Click "Conduct session" task
4. Assign to both You and Alex
5. Save

Both you and Alex see the task.

### What the Second Shooter Sees

**If Alex is assigned to the job:**
- Full job details (client name, timeline, location)
- Contract (if they need to review it)
- Notes and preferences
- Workflow tasks
- Calendar event

**If Alex is only assigned to "Conduct session" task:**
- Task details (date, time, location)
- Limited job context
- Cannot see contract, pricing, or other tasks

**Choose based on trust and need:**
- Full job access: For trusted associate photographers
- Task-only access: For contracted second shooters who don't need full details

### Day-of Coordination

**Before the shoot:**
- Both photographers sync calendars (automatic via ShootPath)
- Primary photographer (you) shares timeline and shot list
- Confirm equipment, roles, and responsibilities

**During the shoot:**
- Primary photographer directs
- Second shooter captures complementary angles
- No direct client communication unless necessary (primary photographer leads)

**After the shoot:**
- Second shooter delivers raw files (via Dropbox, ShootPath file sharing, or other method)
- Primary photographer edits (or hands off to editor)
- Second shooter marks "Conduct session" task complete

### Payment for Second Shooters

Second shooters are typically paid per gig (not via ShootPath billing):

**How to handle:**
- Track second shooter jobs manually or via ShootPath notes
- Pay second shooter via your payroll system, Venmo, etc.
- ShootPath doesn't handle contractor payments (use external tools)

**Record keeping:**
- Add job note: "Paid Alex $500 for second shooting on [date]"
- Export jobs by photographer for contractor payment reconciliation

---

## Quality Control and Review

With a team, quality control ensures consistency.

### Review Processes

**Who reviews what:**

**Admin/Owner reviews:**
- Quotes before they're sent (if accuracy is critical)
- Edited photos before delivery (if quality control is needed)
- Client communications (spot-check emails for tone and accuracy)

**Photographer reviews:**
- Their own work before marking tasks complete
- Galleries before upload (catch errors early)

**Assistant reviews:**
- Emails for typos and tone before sending
- Gallery uploads for correct files and settings

### Approval Workflows

**For critical tasks, require approval:**

**Example: Edited photos must be approved before upload**

1. Editor (Sam) edits photos and marks "Edit photos" task complete
2. System creates "Review edited photos" task assigned to Owner (You)
3. You review, approve (or request changes)
4. Once approved, "Upload gallery" task assigned to Assistant (Emma)

**How to configure:**
- **Settings > Workflows > [Workflow] > Tasks**
- Add "Approval required" step between editing and uploading
- Assign approval task to Owner or Admin

### Feedback and Iteration

**Give constructive feedback:**
- If a team member's work needs improvement, provide specific feedback
- Use task comments or direct communication (not public notes)
- Focus on what can improve, not blame

**Celebrate great work:**
- When someone nails a task, acknowledge it publicly
- Positive reinforcement builds morale and consistency

---

## Measuring Team Performance

Track how your team is performing to identify strengths and bottlenecks.

### Key Metrics

**1. Task completion time**
- How long does each team member take to complete tasks?
- Are tasks completed on time or overdue?

**2. Job throughput**
- How many jobs is each photographer handling simultaneously?
- Is anyone overloaded or underutilized?

**3. Client satisfaction**
- Are clients happy with response times and quality?
- Any complaints about specific team members?

**4. Revenue per photographer**
- How much revenue does each photographer generate?
- Are associate photographers profitable after their costs?

**5. Team collaboration**
- Are handoffs smooth or full of delays?
- Are team members communicating effectively?

### Using ShootPath Reports

**Access:** Go to **Reports > Team Performance**

**Available reports:**
- Tasks completed by team member
- Average task completion time
- Jobs per photographer
- Revenue by photographer
- Overdue tasks by team member

**Export data:**
- Download CSV for deeper analysis in Excel or Google Sheets

### Regular Team Check-Ins

**Weekly or biweekly team meetings:**
- Review active jobs and upcoming deadlines
- Address bottlenecks or delays
- Celebrate wins and completed projects
- Adjust workflows based on feedback

**Monthly performance reviews:**
- Review metrics with each team member
- Discuss what's working and what's not
- Set goals for the next month

---

## Troubleshooting Team Workflows

Common team workflow issues and solutions.

### "Tasks aren't getting done on time"

**Possible causes:**
- Team member is overloaded
- Task deadlines are unrealistic
- Team member doesn't understand the task
- Notifications aren't working

**Solutions:**
1. Check workload: How many tasks does this person have?
2. Reassign tasks if they're overloaded
3. Adjust deadlines if they're too aggressive
4. Provide training or clarification
5. Verify notification settings

### "Team members aren't communicating"

**Possible causes:**
- No clear expectations about communication
- Task comments aren't being used
- Team members prefer other tools (text, Slack)

**Solutions:**
1. Set clear communication expectations
2. Train team on task comments and job notes
3. Encourage commenting when marking tasks complete
4. Consider integrating with Slack or other tools (if ShootPath supports it)

### "Handoffs are getting dropped"

**Possible causes:**
- Next person doesn't know they're up
- Task assignments aren't clear
- Notifications aren't working

**Solutions:**
1. Configure automatic task assignments in workflow
2. Enable notifications for task assignments
3. Use handoff notes (mark task complete + add note for next person)
4. Admin monitors tasks to catch dropped handoffs

### "Quality is inconsistent across team members"

**Possible causes:**
- Lack of training or clear standards
- No review/approval process
- Team members have different interpretations of quality

**Solutions:**
1. Create quality standards document (what's acceptable)
2. Implement approval workflows for critical tasks
3. Provide training and examples
4. Review work samples regularly and give feedback

---

## Best Practices Summary

**Clear task assignments:**
- Every task has one owner (no ambiguity)
- Use default assignments for consistency
- Override when needed for specific jobs

**Enable notifications:**
- Team members know immediately when tasks are assigned
- Overdue tasks are highlighted

**Use task comments:**
- Keep communication contextual (attached to the task)
- Everyone assigned to the job sees the conversation

**Monitor progress:**
- Admins and Owners track task completion
- Identify bottlenecks early
- Redistribute work if needed

**Smooth handoffs:**
- Mark tasks complete as soon as finished
- Add handoff notes for the next person
- Next task should auto-assign to the right person

**Quality control:**
- Review critical work before delivery
- Provide feedback and training
- Celebrate great work

**Regular check-ins:**
- Weekly team meetings to review progress
- Monthly performance reviews
- Adjust workflows based on feedback

---

## What's Next?

Ready to optimize your team workflows? Explore these related articles:

**[Team Members](./team-members)** - Learn how to add and manage team members

**[Roles and Permissions](./roles-and-permissions)** - Understand what each role can do

**[Team Management Overview](./index)** - See the bigger picture of team features

Or explore workflow and job management:

**[Workflows Overview](../workflows/)** - Deep dive into ShootPath's workflow system

**[Job Workflows](../jobs/job-workflows)** - Understand how workflows integrate with jobs

**[Managing Jobs](../jobs/managing-jobs)** - Learn job management best practices

**[Calendar](../calendar/)** - Master team calendar coordination

---

**Questions?** Look for the help links throughout ShootPath, or use the support widget if you need assistance!
