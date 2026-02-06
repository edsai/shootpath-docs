---
sidebar_position: 3
---

# Roles and Permissions

## Quick Reference

ShootPath uses **role-based access control** to determine what each team member can see and do. Understanding roles and permissions ensures team members have the access they need without compromising security or overwhelming them with irrelevant features.

**Four User Roles:**
- **Owner** - Full access to everything (you, the account creator)
- **Admin** - Manage operations and team, but not billing
- **Photographer** - Manage assigned jobs only
- **Assistant** - Support tasks with read-mostly access

**Key Principles:**
- **Least privilege** - Give minimum access needed for the job
- **Role-based** - Permissions tied to roles, not individuals
- **Customizable** - Can override defaults for specific needs
- **Auditable** - Track who did what and when

**Access Settings:** Go to **Settings > Team Members** > click a team member > **Permissions** tab

---

## Detailed Guide

### Understanding Access Control

Access control answers three questions for every action in ShootPath:
1. **Who** is trying to do this? (user authentication)
2. **What** are they trying to do? (action)
3. **Are they allowed** to do it? (authorization)

ShootPath handles this through **roles**:
- Each user has one role
- Each role has a default set of permissions
- Permissions can be customized per user if needed
- System checks permissions before allowing any action

### The Four Roles Explained

Let's deep dive into each role, when to use it, and what it can do.

---

## Owner Role

### Overview

The **Owner** is the person who created the ShootPath account. There's only one owner per account, and they have unlimited access to everything.

**Who should be Owner:**
- You (the business owner)
- The person who pays for the subscription
- The person with ultimate decision-making authority

**Key characteristics:**
- Full access to all features, data, and settings
- Access to billing and subscription management
- Can add/remove any team member (including Admins)
- Cannot be removed by anyone else
- Can transfer ownership (via support)

### Full Permissions List

The Owner can do everything:

#### Jobs & Clients
- ✅ View all jobs (including those assigned to others)
- ✅ Create, edit, and delete jobs
- ✅ Assign jobs to team members
- ✅ View and edit all client information
- ✅ Delete clients (if no associated jobs)

#### Financial
- ✅ View all invoices and payments
- ✅ Create and edit quotes
- ✅ Modify pricing and payment schedules
- ✅ Process refunds
- ✅ View financial reports and analytics
- ✅ Access billing and subscription settings
- ✅ Update payment methods
- ✅ View and export financial data

#### Contracts & Legal
- ✅ Create and edit contract templates
- ✅ Send contracts to clients
- ✅ View signed contracts
- ✅ Modify contract terms (before signing)

#### Galleries & Deliverables
- ✅ Upload, edit, and delete galleries
- ✅ Set gallery permissions and expiration
- ✅ View gallery analytics (client downloads, views)
- ✅ Configure watermarks and branding

#### Workflows & Automation
- ✅ Create and edit workflows
- ✅ Modify workflow stages and triggers
- ✅ Assign workflow tasks to team members
- ✅ Delete or skip workflow tasks

#### Team Management
- ✅ Add and remove team members
- ✅ Change team member roles and permissions
- ✅ View team member activity logs
- ✅ Deactivate or reactivate accounts

#### Settings & Integrations
- ✅ Modify all business settings (name, logo, contact info)
- ✅ Configure integrations (Stripe, email, etc.)
- ✅ Edit email templates
- ✅ Customize branding and styling
- ✅ Configure API access
- ✅ Manage two-factor authentication requirements

#### Reports & Analytics
- ✅ View all reports (financial, operational, team activity)
- ✅ Export data to CSV or PDF
- ✅ Access API for custom integrations

#### System Administration
- ✅ Transfer ownership (via support request)
- ✅ Close or delete the account
- ✅ View audit logs for security and compliance

### Responsibilities

With great power comes great responsibility:

**Security:**
- Protect your password carefully
- Enable two-factor authentication
- Review team member access regularly
- Monitor audit logs for suspicious activity

**Billing:**
- Ensure subscription stays active
- Update payment method before it expires
- Review monthly invoices
- Manage team member costs

**Oversight:**
- Set business strategy and workflows
- Handle escalations and complex problems
- Make final decisions on major changes
- Ensure client satisfaction and quality control

**Compliance:**
- Ensure business follows legal requirements
- Manage contracts and terms of service
- Protect client data and privacy

### Use Cases

**Scenario 1: Solo photographer**
You're the only user. You're the Owner by default and have full access.

**Scenario 2: Small studio**
You're the Owner, and you hire an Admin (studio manager) to run operations. You focus on strategy and VIP clients. Admin handles day-to-day, but you retain billing control.

**Scenario 3: Partnership**
You and a partner co-own the business. One of you is the Owner, the other is an Admin. You make major decisions together, but Owner handles billing.

---

## Admin Role

### Overview

**Admin** is for trusted team members who manage operations but shouldn't access billing. Think studio managers, operations leads, or business partners.

**Who should be Admin:**
- Studio managers who oversee photographers and jobs
- Business partners who co-manage the studio
- Operations leads who handle day-to-day workflow
- Office managers who coordinate the entire business

**Key characteristics:**
- Can manage all jobs, clients, and leads
- Can add/remove team members and change their roles
- Can edit workflows, settings, and integrations
- **Cannot** access billing or subscription settings
- **Cannot** remove the Owner

### Full Permissions List

Admins have almost everything Owners have, minus billing:

#### Jobs & Clients
- ✅ View all jobs (including those assigned to other team members)
- ✅ Create, edit, and delete jobs
- ✅ Assign jobs to team members
- ✅ View and edit all client information
- ✅ Delete clients (if no associated jobs)

#### Financial
- ✅ View all invoices and payments
- ✅ Create and edit quotes
- ✅ Modify pricing and payment schedules
- ⚠️ Process refunds (may require Owner approval, depending on settings)
- ✅ View financial reports
- ❌ Access billing and subscription settings
- ❌ Update payment methods
- ❌ Change subscription plan

#### Contracts & Legal
- ✅ Create and edit contract templates
- ✅ Send contracts to clients
- ✅ View signed contracts
- ✅ Modify contract terms (before signing)

#### Galleries & Deliverables
- ✅ Upload, edit, and delete galleries
- ✅ Set gallery permissions and expiration
- ✅ View gallery analytics
- ✅ Configure watermarks and branding

#### Workflows & Automation
- ✅ Create and edit workflows
- ✅ Modify workflow stages and triggers
- ✅ Assign workflow tasks to team members
- ✅ Delete or skip workflow tasks

#### Team Management
- ✅ Add team members (Owner approves billing impact)
- ✅ Remove team members (except Owner)
- ✅ Change team member roles and permissions
- ✅ View team member activity logs
- ✅ Deactivate or reactivate accounts

#### Settings & Integrations
- ✅ Modify business settings (name, logo, contact info)
- ✅ Configure integrations (Stripe, email, etc.)
- ✅ Edit email templates
- ✅ Customize branding and styling
- ⚠️ Configure API access (may be restricted)

#### Reports & Analytics
- ✅ View all reports (financial, operational, team activity)
- ✅ Export data to CSV or PDF

#### System Administration
- ❌ Transfer ownership
- ❌ Close or delete the account
- ✅ View audit logs

### Why Restrict Billing?

The Owner retains billing control for several reasons:

**Security:**
- Prevents accidental subscription cancellation
- Protects payment method information
- Reduces risk of unauthorized plan changes

**Financial control:**
- Owner ultimately responsible for business costs
- Prevents disputes if partnership dissolves
- Clear accountability for subscription expenses

**Practical:**
- Admin manages operations, Owner manages finances
- Separation of duties (accounting best practice)

### Use Cases

**Scenario 1: Studio manager**
You own a studio with 4 photographers. You hire Rachel as studio manager (Admin). Rachel assigns jobs, manages photographers, handles client escalations—but you retain billing control.

**Scenario 2: Business partner**
You co-own the business with Jordan. You're the Owner (you started the account), Jordan is an Admin. You both manage operations equally, but you handle the subscription billing.

**Scenario 3: Senior team member**
Alex started as a Photographer but proved trustworthy and capable. You promote Alex to Admin so they can help manage the team and workflows while you focus on growth.

---

## Photographer Role

### Overview

**Photographer** is for team members who shoot jobs but shouldn't see the entire business. They manage their assigned jobs independently.

**Who should be Photographer:**
- Second shooters who handle overflow bookings
- Associate photographers in multi-photographer studios
- Freelance photographers contracted for specific jobs
- External editors who need job context

**Key characteristics:**
- **Only sees jobs assigned to them** (biggest distinction from Admin)
- Full job management for assigned jobs
- Cannot see other photographers' jobs or business-wide data
- Cannot manage team or settings

### Full Permissions List

Photographers have focused, job-specific access:

#### Jobs & Clients
- ✅ View assigned jobs only
- ✅ Edit assigned job details (notes, dates, locations)
- ❌ Create new jobs (Admin/Owner does this)
- ❌ Delete jobs
- ✅ View client information for assigned jobs
- ❌ View clients not associated with assigned jobs
- ❌ Edit client contact information

#### Financial
- ✅ View invoices and payments for assigned jobs
- ❌ Edit pricing or payment schedules
- ❌ Process refunds
- ❌ View business-wide financial reports
- ❌ Access billing settings

#### Contracts & Legal
- ❌ Create or edit contract templates
- ✅ View contracts for assigned jobs
- ✅ Send contracts (if workflow task assigned to them)
- ❌ Modify contract terms

#### Galleries & Deliverables
- ✅ Upload galleries for assigned jobs
- ✅ Edit gallery details (title, description, cover photo)
- ✅ Set gallery permissions (client download settings)
- ❌ Delete galleries (may require Owner/Admin approval)
- ✅ View gallery analytics for assigned jobs

#### Workflows & Automation
- ❌ Create or edit workflows
- ✅ View workflow for assigned jobs
- ✅ Mark workflow tasks complete for assigned jobs
- ✅ Add notes to workflow tasks
- ❌ Delete or skip workflow stages

#### Team Management
- ❌ Add or remove team members
- ❌ View other team members (may see names in job assignments)
- ❌ Change permissions
- ✅ View their own profile and settings

#### Settings & Integrations
- ❌ Modify business settings
- ❌ Configure integrations
- ❌ Edit email templates (use existing templates only)
- ✅ Customize their personal profile (photo, contact info)

#### Reports & Analytics
- ❌ View business-wide reports
- ✅ View their own job history and activity
- ✅ View calendar for assigned jobs only

#### Communication
- ✅ Send emails to clients (for assigned jobs)
- ✅ Use email templates
- ✅ View email history for assigned jobs
- ❌ View emails for other jobs

### Why Limit to Assigned Jobs?

**Privacy:**
Photographers don't need to see clients they're not working with. This protects client privacy and complies with data minimization principles.

**Focus:**
Showing only assigned jobs keeps photographers focused on their work. They're not overwhelmed by the entire business's job list.

**Scalability:**
In large studios, photographers shouldn't see competitors' bookings or pricing. Assigned-jobs-only access enables healthy team dynamics.

**Security:**
Reduces risk if a freelance photographer's account is compromised or if they leave on bad terms.

### Use Cases

**Scenario 1: Second shooter**
You book two weddings on the same day. You assign one to Alex (Photographer role). Alex sees only that wedding's details and manages it independently. Alex doesn't see your other jobs.

**Scenario 2: Associate photographer**
You run a portrait studio with 3 associate photographers. Each photographer has their own clients. Each logs in and sees only their assigned jobs—not each other's bookings or pricing.

**Scenario 3: External editor**
You outsource editing to a specialist. You add them as a Photographer so they can access job files, see deadlines, and upload galleries—but they can't see your other clients or business details.

---

## Assistant Role

### Overview

**Assistant** is for administrative support staff who help with tasks but don't manage jobs or clients directly. They have broad visibility but limited editing permissions.

**Who should be Assistant:**
- Virtual assistants who handle emails and scheduling
- Office coordinators who support all photographers
- Gallery uploaders who post photos but don't need full access
- Customer service reps who answer client questions

**Key characteristics:**
- Can view most jobs and clients (read-only)
- Can perform specific tasks (send quotes, upload galleries)
- **Cannot** edit job details, pricing, or financial data
- **Cannot** delete anything important

### Full Permissions List

Assistants have task-specific access:

#### Jobs & Clients
- ✅ View all jobs (read-only)
- ❌ Create or edit job details (can't change pricing, dates, etc.)
- ❌ Delete jobs
- ✅ View client information (read-only)
- ❌ Edit client contact information
- ✅ Add notes to jobs (if Owner/Admin allows)

#### Financial
- ⚠️ View invoices (may be restricted depending on settings)
- ❌ Edit pricing or payment schedules
- ❌ Process payments or refunds
- ❌ View financial reports

#### Contracts & Legal
- ❌ Create or edit contract templates
- ✅ View contracts (if needed for client support)
- ⚠️ Send contracts (if assigned this workflow task)
- ❌ Modify contract terms

#### Galleries & Deliverables
- ✅ Upload galleries
- ⚠️ Edit gallery details (may be restricted to upload-only)
- ❌ Delete galleries
- ✅ View gallery analytics (who downloaded what)

#### Workflows & Automation
- ❌ Create or edit workflows
- ✅ View workflow for all jobs
- ⚠️ Mark workflow tasks complete (only tasks assigned to them)
- ✅ Add notes to tasks

#### Team Management
- ❌ Add or remove team members
- ❌ View team member details
- ❌ Change permissions

#### Settings & Integrations
- ❌ Modify business settings
- ❌ Configure integrations
- ❌ Edit email templates
- ✅ Customize their personal profile

#### Reports & Analytics
- ❌ View business-wide reports
- ✅ View their own activity log

#### Communication
- ✅ Send emails to clients (using templates)
- ✅ Use email templates
- ✅ View email history for all jobs
- ⚠️ Send quotes (if allowed in settings)

### Why So Limited?

**Assistants execute, they don't decide:**

Assistants support the business but shouldn't change pricing, delete data, or make strategic decisions. They're given specific tasks:
- "Send this quote to this lead"
- "Upload this gallery for this job"
- "Respond to this client email using the template"

Limiting permissions ensures they can't accidentally (or intentionally) change critical data.

**Assistants are often contractors or part-time:**

If you hire a VA or part-time coordinator, you don't want them having access to financials or settings. Assistant role provides the right balance.

### Use Cases

**Scenario 1: Virtual assistant**
You hire Emma (VA) to handle client emails, send quotes, and upload galleries. Emma has Assistant access. She can see all jobs (to answer client questions) but can't edit pricing or delete anything.

**Scenario 2: Gallery uploader**
You hate uploading galleries. You hire a part-time assistant just to upload edited photos. They have Assistant role, can upload galleries, but can't see financials or edit job details.

**Scenario 3: Customer service**
You have a customer service rep who answers client inquiries. They need to see job details and contracts to answer questions, but shouldn't edit anything. Assistant role is perfect.

---

## Comparing Roles Side-by-Side

Here's a detailed comparison table:

| Permission | Owner | Admin | Photographer | Assistant |
|------------|-------|-------|--------------|-----------|
| **Jobs & Clients** |
| View all jobs | ✅ | ✅ | ❌ (assigned only) | ✅ (read-only) |
| Create/edit/delete jobs | ✅ | ✅ | ⚠️ (edit assigned) | ❌ |
| View all clients | ✅ | ✅ | ❌ (assigned only) | ✅ (read-only) |
| Edit client details | ✅ | ✅ | ❌ | ❌ |
| **Financial** |
| View invoices/payments | ✅ All | ✅ All | ✅ Assigned | ⚠️ Limited |
| Edit pricing | ✅ | ✅ | ❌ | ❌ |
| Process refunds | ✅ | ⚠️ | ❌ | ❌ |
| View financial reports | ✅ | ✅ | ❌ | ❌ |
| Access billing/subscription | ✅ | ❌ | ❌ | ❌ |
| **Contracts** |
| Create/edit templates | ✅ | ✅ | ❌ | ❌ |
| Send contracts | ✅ | ✅ | ✅ (assigned) | ⚠️ (if allowed) |
| View contracts | ✅ All | ✅ All | ✅ Assigned | ⚠️ (if allowed) |
| **Galleries** |
| Upload galleries | ✅ All | ✅ All | ✅ Assigned | ✅ All |
| Edit gallery settings | ✅ | ✅ | ✅ (assigned) | ⚠️ Limited |
| Delete galleries | ✅ | ✅ | ⚠️ (may need approval) | ❌ |
| **Workflows** |
| Create/edit workflows | ✅ | ✅ | ❌ | ❌ |
| View workflow progress | ✅ All | ✅ All | ✅ Assigned | ✅ All |
| Complete tasks | ✅ | ✅ | ✅ (assigned) | ⚠️ (assigned to them) |
| **Team Management** |
| Add/remove team members | ✅ | ✅ (not Owner) | ❌ | ❌ |
| Change roles/permissions | ✅ | ✅ | ❌ | ❌ |
| View team activity | ✅ | ✅ | ❌ | ❌ |
| **Settings** |
| Modify business settings | ✅ | ✅ | ❌ | ❌ |
| Configure integrations | ✅ | ✅ | ❌ | ❌ |
| Edit email templates | ✅ | ✅ | ❌ | ❌ |
| **Reports** |
| View business reports | ✅ | ✅ | ❌ | ❌ |
| Export data | ✅ | ✅ | ⚠️ (assigned jobs) | ❌ |
| **System** |
| Transfer ownership | ✅ | ❌ | ❌ | ❌ |
| Close account | ✅ | ❌ | ❌ | ❌ |
| View audit logs | ✅ | ✅ | ❌ | ❌ |

**Legend:**
- ✅ Full access
- ⚠️ Limited or conditional access
- ❌ No access

---

## Custom Permissions

While roles provide sensible defaults, you can customize permissions for specific users.

### When to Customize

**Use cases for custom permissions:**

**1. Hybrid roles**
- A Photographer who also needs to see reports
- An Assistant who needs to edit job details for their assigned jobs

**2. Training periods**
- New Admin who temporarily has read-only access while learning
- Intern with limited Assistant access for security

**3. Specialized responsibilities**
- Bookkeeper who's an Admin but only needs financial access
- Marketing team member who needs gallery access but not job details

**4. Contractual requirements**
- Freelancer who needs Photographer access but can't see payments
- External agency with Assistant access plus specific job editing

### How to Customize

1. Go to **Settings > Team Members**
2. Click on the team member
3. Navigate to **Permissions** tab
4. Toggle specific permissions on/off
5. Save changes

**Permission categories:**
- Jobs & Clients
- Financial
- Contracts & Galleries
- Workflows & Tasks
- Team Management
- Settings & Integrations
- Reports & Analytics

Each category has granular toggles (view, create, edit, delete).

### Best Practices for Custom Permissions

**Document why:**
Add a note explaining why you customized permissions. Future-you will thank you.

**Start restrictive:**
Start with the default role and add permissions as needed. Don't start with full access and remove things.

**Review regularly:**
Custom permissions can get messy over time. Review every quarter and simplify where possible.

**Prefer role changes:**
If someone's responsibilities change significantly, change their role instead of heavily customizing permissions.

---

## Security Best Practices

Roles and permissions are only effective if you follow security best practices.

### Principle of Least Privilege

Give team members the **minimum access** required to do their job.

**Examples:**
- Assistant who uploads galleries doesn't need financial access
- Photographer who shoots weddings doesn't need to see portrait jobs
- Admin who manages operations doesn't need billing access

**Why it matters:**
- Reduces risk if account is compromised
- Prevents accidental changes or deletions
- Protects client privacy
- Simplifies offboarding

### Strong Authentication

**Require strong passwords:**
- Minimum 12 characters
- Mix of upper/lowercase, numbers, symbols
- No common words or patterns

**Enable two-factor authentication (2FA):**
- Required for Owner and Admin
- Strongly recommended for Photographers and Assistants
- Use authenticator app (not SMS, if possible)

**Avoid shared logins:**
- Each team member gets their own account
- Never share the Owner password
- Don't create generic "info@" or "admin@" accounts

### Access Reviews

**Monthly:**
- Check who's logged in recently
- Verify active team members still need access

**Quarterly:**
- Review all team member roles and permissions
- Adjust based on changed responsibilities
- Remove inactive accounts

**After changes:**
- When someone leaves, disable their account immediately
- When someone's role changes, update permissions same day
- When a project ends, remove contractor access

### Audit Logging

ShootPath tracks who does what:

**View audit logs:**
1. Go to **Settings > Security > Audit Logs**
2. Filter by team member, action type, or date range
3. Export for compliance or investigation

**What's logged:**
- Logins and logouts
- Job creations and edits
- Gallery uploads and deletions
- Settings changes
- Team member additions/removals
- Financial transactions

**Why it matters:**
- Accountability (who did this?)
- Troubleshooting (what changed?)
- Security (detect suspicious activity)
- Compliance (record keeping)

---

## Common Permission Scenarios

Let's walk through typical permission questions.

### "Can a Photographer see other Photographers' jobs?"

**No.** Photographers only see jobs assigned to them. This is intentional:
- Protects client privacy
- Prevents pricing visibility (if photographers have different rates)
- Keeps focus on their work
- Avoids confusion ("Is this my job?")

**If you want photographers to see all jobs,** promote them to Admin.

### "Can an Assistant edit job pricing?"

**No.** Assistants have read-only access to most job details. They can upload galleries and send emails, but can't change pricing, dates, or critical details.

**If you need an assistant to edit jobs,** consider:
- Giving them Photographer role (if they manage specific jobs)
- Customizing their permissions to allow job editing
- Promoting them to Admin (if they're truly managing operations)

### "Can an Admin see billing and subscription details?"

**No.** Admins intentionally cannot access:
- Subscription plan and pricing
- Payment method
- Billing history
- Ability to change subscription

**Why?** Prevents accidental subscription changes and keeps financial control with the Owner.

**If an Admin needs billing visibility** (e.g., they're your accountant):
- Owner can download invoices and share manually
- Consider using ShootPath API to sync billing data externally
- Or make them an authorized contact on your subscription (contact support)

### "Can a Photographer reassign their own jobs to someone else?"

**No.** Only Admins and Owners can reassign jobs. Photographers manage jobs assigned to them but can't reassign.

**Why?** Prevents photographers from shifting work without oversight.

**If a Photographer can't handle a job:**
They should notify Admin/Owner, who reassigns it.

### "Can an Assistant delete galleries?"

**No.** Assistants can upload galleries but typically can't delete them (to prevent accidental data loss).

**If you need an Assistant to delete galleries:**
Customize their permissions to allow gallery deletion (Settings > Team Members > select member > Permissions).

---

## Role Change Scenarios

What happens when you change someone's role?

### Promoting Assistant to Photographer

**Before (Assistant):**
- Views all jobs (read-only)
- Uploads galleries for any job
- Can't edit job details

**After (Photographer):**
- Views only assigned jobs
- Can edit assigned job details
- Manages assigned jobs independently

**Impact:**
- They lose visibility into jobs not assigned to them
- They gain editing permissions for assigned jobs
- Reassure them this is intentional (more responsibility, more focus)

### Promoting Photographer to Admin

**Before (Photographer):**
- Sees only assigned jobs
- Manages assigned jobs
- Can't see business-wide data

**After (Admin):**
- Sees all jobs, clients, leads
- Can assign jobs to other photographers
- Can edit workflows and settings
- Still can't access billing

**Impact:**
- Huge increase in visibility and responsibility
- Provide training on new features
- Set expectations about their new responsibilities

### Demoting Admin to Photographer

**Before (Admin):**
- Full visibility and control
- Manages team and settings

**After (Photographer):**
- Only sees assigned jobs
- Can't manage team or settings
- Limited to job-specific tasks

**Impact:**
- Significant reduction in access (communicate clearly why)
- May need to reassign their oversight responsibilities
- Consider if this is the right move or if removal is more appropriate

### Demoting Photographer to Assistant

**Before (Photographer):**
- Manages assigned jobs
- Edits job details and pricing

**After (Assistant):**
- Views all jobs (read-only)
- Can't edit job details
- Limited to support tasks

**Impact:**
- Loss of job management authority
- Often used when transitioning someone from shooting to admin support
- Communicate clearly about changed role and expectations

---

## Troubleshooting Permissions

Common permission issues and how to fix them.

### "I can't see a feature I used to access"

**Possible causes:**
- Role changed
- Custom permissions revoked
- Feature disabled for your plan tier

**Solutions:**
1. Check your current role (Settings > Profile)
2. Contact Owner/Admin to verify permissions
3. Check if feature is available in your subscription plan

### "I see jobs I shouldn't see"

**Possible causes:**
- Role is more permissive than expected (e.g., Admin instead of Photographer)
- Jobs were assigned to you accidentally

**Solutions:**
1. Verify your role
2. If you're Admin, that's expected (you see all jobs)
3. If you're Photographer, check job assignments (you may have been assigned unexpectedly)
4. Contact Owner to adjust role or assignments

### "I can't complete a task I'm assigned"

**Possible causes:**
- Task requires permissions you don't have
- Task is for a job you can't access (Photographer not assigned)

**Solutions:**
1. Verify you're assigned to the job
2. Check if your role allows this action
3. Contact Admin/Owner to complete the task or adjust permissions

### "Changes I made disappeared"

**Possible causes:**
- You don't have edit permissions (only view)
- Changes conflicted with another user's edit
- Bug or browser issue

**Solutions:**
1. Verify your role allows editing
2. Check audit log to see what happened
3. Try again, refresh browser
4. Contact support if problem persists

---

## Best Practices Summary

**Choose roles carefully:**
- Start with the most restrictive role that fits
- Customize only when truly necessary
- Document custom permissions

**Review regularly:**
- Monthly check of active team members
- Quarterly permissions audit
- Adjust as responsibilities change

**Secure accounts:**
- Strong passwords for everyone
- Two-factor authentication enabled
- Individual logins (no sharing)

**Communicate expectations:**
- Explain what each role can and can't do
- Set clear responsibilities
- Provide training on relevant features

**Monitor activity:**
- Check audit logs for suspicious behavior
- Verify team members are logging in and working
- Address permission issues promptly

---

## What's Next?

Now that you understand roles and permissions in depth, explore these related articles:

**[Team Members](./team-members)** - Learn how to add, manage, and remove team members

**[Team Workflows](./team-workflows)** - Discover collaborative workflows and task delegation strategies

**[Team Management Overview](./index)** - Understand the bigger picture of team features

Or explore related topics:

**[Workflows](../workflows/)** - See how workflows integrate with role-based task assignments

**[Jobs](../jobs/)** - Learn how job visibility differs by role

**[Settings](../account-setup/)** - Configure team-wide settings and integrations

---

**Questions?** Look for the help links throughout ShootPath, or use the support widget if you need assistance!
