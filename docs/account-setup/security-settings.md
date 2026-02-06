---
sidebar_position: 4
---

# Security Settings

## Quick Reference

Security settings protect your ShootPath account, business data, and client information from unauthorized access. Strong security practices are essential for running a professional photography business.

**Key Security Areas:**
- **Password Management** - Strong passwords and password changes
- **Two-Factor Authentication (2FA)** - Extra login protection layer
- **Login Sessions** - Manage devices logged into your account
- **API Keys** - Access tokens for integrations and automation
- **Audit Log** - Track who did what and when
- **Account Recovery** - Options for regaining access if locked out

**Access Security Settings:** Settings → **Security Settings**

**Quick Security Checklist:**
- ✅ Use a strong, unique password (12+ characters, mixed case, numbers, symbols)
- ✅ Enable two-factor authentication (2FA)
- ✅ Review active login sessions monthly
- ✅ Never share your password or 2FA codes
- ✅ Use a password manager (1Password, LastPass, Bitwarden)

---

## Detailed Guide

Your ShootPath account contains sensitive business and client data - financial records, personal information, contracts, and private galleries. Protecting this data is your responsibility. This guide walks through every security setting and best practice.

### Accessing Security Settings

1. Click your **profile photo** or initials (top-right corner)
2. Select **Settings**
3. In the left sidebar, click **Security Settings**

You'll see all security configuration options.

### Password Management

Your password is the primary key to your account. A weak password puts your entire business at risk.

#### Password Requirements

ShootPath enforces strong password requirements:

**Minimum requirements:**
- **12 characters minimum** (16+ recommended)
- **Mixed case** - At least one uppercase and one lowercase letter
- **Numbers** - At least one digit (0-9)
- **Special characters** - At least one symbol (!@#$%^&*)
- **No common passwords** - Not in the top 10,000 most common passwords list
- **No personal info** - Can't contain your name, email, or business name

**Examples of strong passwords:**
- `Cr@sh1ng-Elegance-2024!` (25 characters, memorable phrase)
- `7hX#9mK$pL2wQ@vR` (16 characters, random)
- `PhotographyStudio!2024#Seattle` (31 characters, memorable)

**Examples of weak passwords (never use these):**
- `password123` - Too common, in breach databases
- `Photography` - No numbers or symbols
- `Emma1234` - Uses your name, predictable pattern
- `qwerty` - Keyboard pattern, easily guessed

:::tip Use a Password Manager
Password managers (1Password, LastPass, Bitwarden) generate and store strong passwords securely. You only need to remember one master password. This is the #1 security recommendation for photographers.
:::

#### Changing Your Password

**When to change your password:**
- Every 6-12 months (routine security practice)
- If you suspect your password was compromised
- After using ShootPath on a public/shared computer
- If a team member who knew your password leaves
- If your password appears in a data breach (check haveibeenpwned.com)

**How to change your password:**
1. Go to **Security Settings > Password**
2. Enter your **current password**
3. Enter your **new password** (must meet requirements)
4. Confirm new password
5. Click **Update Password**

**What happens after changing:**
- You remain logged in on your current device
- All other devices/browsers are logged out automatically (security measure)
- You'll need to log in again on those devices with the new password

:::warning Security Note
Never reuse passwords across different services. If one service gets breached, attackers will try that password on other sites (including ShootPath). Use unique passwords everywhere!
:::

#### Forgot Password / Account Recovery

If you forget your password:

1. Go to the ShootPath login page
2. Click **"Forgot password?"**
3. Enter your email address
4. Check your email for a password reset link (arrives within 5 minutes)
5. Click the link (valid for 1 hour)
6. Enter a new password
7. Log in with your new password

**If you don't receive the email:**
- Check spam/junk folder
- Verify you entered the correct email address
- Wait 10 minutes (email delivery can be delayed)
- Try the reset process again

**If your email is not verified:**
You cannot reset your password via email. Contact support@shootpath.com with:
- Your account email address
- Business name
- Last known login date
- Proof of identity (business registration, website, etc.)

**Security of reset links:**
Password reset links expire after 1 hour and can only be used once. They cannot be reused or intercepted after use.

### Two-Factor Authentication (2FA)

Two-factor authentication (2FA) adds an extra security layer: even if someone steals your password, they can't access your account without the second factor (a code from your phone).

#### Why Enable 2FA?

**Protection against:**
- **Stolen passwords** - Password leaks from other sites
- **Phishing attacks** - Someone tricks you into revealing your password
- **Brute force** - Automated password guessing
- **Shoulder surfing** - Someone sees you type your password

**Real-world scenario:**
Your password appears in a data breach from another service where you used the same password. Attackers try that password on thousands of sites, including ShootPath. With 2FA enabled, they can't get in - they'd need the 6-digit code from your phone, which they don't have.

#### How 2FA Works

**Two factors:**
1. **Something you know** - Your password
2. **Something you have** - Your phone (generates time-based codes)

**Login flow with 2FA:**
1. Enter your email and password
2. ShootPath prompts for 6-digit code
3. Open your authenticator app (Google Authenticator, Authy, 1Password, etc.)
4. Enter the current code
5. You're logged in

**Codes change every 30 seconds**, so even if someone sees a code, it expires quickly.

#### Enabling Two-Factor Authentication

**Prerequisites:**
- An authenticator app installed on your phone:
  - **Google Authenticator** (iOS, Android) - Simple, reliable
  - **Authy** (iOS, Android) - Multi-device sync
  - **1Password** (iOS, Android, desktop) - If you use 1Password already
  - **Microsoft Authenticator** (iOS, Android)
  - **Any TOTP-compatible app**

**Setup steps:**
1. Go to **Security Settings > Two-Factor Authentication**
2. Click **Enable 2FA**
3. ShootPath displays a QR code
4. Open your authenticator app
5. Tap "Add account" or "Scan QR code"
6. Scan the QR code with your phone's camera
7. The app shows "ShootPath - your@email.com" with a 6-digit code
8. Enter the code in ShootPath to verify
9. Click **Confirm and Enable**

**Backup codes:**
After enabling 2FA, ShootPath shows **10 backup codes** (8-digit codes). Save these immediately!

**How to save backup codes:**
- **Download as text file** and store in a password manager
- **Print and store** in a secure physical location
- **Never** share backup codes with anyone

**What backup codes are for:**
If you lose your phone or can't access your authenticator app, you can use a backup code instead of the 6-digit code to log in. Each backup code works once.

:::danger Save Backup Codes!
If you enable 2FA and lose your phone WITHOUT saving backup codes, you will be locked out of your account. You'll need to contact support and verify your identity (a slow process). Save your backup codes!
:::

#### Using 2FA to Log In

**Normal login (with phone):**
1. Enter email and password
2. Open authenticator app
3. Find ShootPath
4. Enter the 6-digit code
5. Click **Verify**

**Login without phone (using backup code):**
1. Enter email and password
2. Click **"Use a backup code instead"**
3. Enter one of your saved 8-digit backup codes
4. Click **Verify**
5. That backup code is now used (can't reuse it)

**"Remember this device" option:**
When logging in with 2FA, you can check **"Trust this device for 30 days"**. For the next 30 days, you won't need to enter 2FA codes on this device. Only use this on personal devices you control!

#### Disabling or Resetting 2FA

**To disable 2FA:**
1. Go to **Security Settings > Two-Factor Authentication**
2. Click **Disable 2FA**
3. Enter your password to confirm
4. 2FA is now disabled (not recommended!)

**To reset 2FA (if you lost your phone):**
1. Log in using a backup code
2. Go to **Security Settings > Two-Factor Authentication**
3. Click **Reset 2FA**
4. Set up 2FA again with a new device
5. Save new backup codes

**If you lost your phone AND backup codes:**
You'll need to contact support. This process takes 1-3 business days and requires identity verification.

#### 2FA Best Practices

**Do:**
- ✅ Use 2FA on all critical accounts (email, banking, ShootPath)
- ✅ Save backup codes securely
- ✅ Use a password manager to store backup codes
- ✅ Enable 2FA for all team members

**Don't:**
- ❌ Share backup codes with anyone (not even team members)
- ❌ Store backup codes in an unencrypted note on your phone
- ❌ Use SMS-based 2FA (less secure than authenticator apps)
- ❌ Take screenshots of QR codes and leave them in your photo library

### Login Sessions and Device Management

Every time you log into ShootPath from a browser or device, a session is created. You can view and manage all active sessions.

#### Viewing Active Sessions

See all devices currently logged into your account:

1. Go to **Security Settings > Active Sessions**
2. You'll see a list of sessions with:
   - **Device/Browser** (e.g., "Chrome on Windows", "Safari on iPhone")
   - **Location** (approximate, based on IP address)
   - **Last activity** (when this session was last used)
   - **IP address**
   - **Session created** (when you logged in)

**Current session indicator:**
The device you're currently using shows "This device" or "Current session" (you can't log out this session from here).

#### Why Monitor Sessions?

**Security reasons:**
- Detect unauthorized access (someone logged in without permission)
- Check if you left yourself logged in on a public computer
- Verify team members aren't sharing login credentials

**Example of suspicious activity:**
You're in Seattle, but you see an active session from New York that you don't recognize. This could indicate:
- Someone has your password
- You accidentally left yourself logged in on a client's computer
- Your account was compromised

**What to do if you see suspicious sessions:**
1. **Immediately** log out all other sessions (see below)
2. Change your password
3. Enable 2FA if not already enabled
4. Contact support to review account activity

#### Logging Out Other Sessions

**To log out a specific session:**
1. Go to **Security Settings > Active Sessions**
2. Find the session you want to log out
3. Click **"Log out"** next to that session
4. That device/browser is logged out immediately

**To log out ALL other sessions:**
1. Go to **Security Settings > Active Sessions**
2. Click **"Log out all other sessions"** (top-right)
3. Confirm
4. All devices except your current one are logged out
5. You'll need to log in again on those devices

**When to log out all sessions:**
- You changed your password
- You left yourself logged in on a public computer
- A team member with account access left your company
- You suspect unauthorized access

#### Session Timeout and Auto-Logout

**Session timeout:**
After a period of inactivity (no mouse/keyboard activity), ShootPath automatically logs you out.

**Timeout options:**
- **15 minutes** (high security)
- **1 hour** (moderate)
- **4 hours** (default, relaxed)
- **Never** (stay logged in indefinitely)

**How to set:**
1. Go to **Security Settings > Session Timeout**
2. Select timeout duration
3. Click **Save Changes**

**What counts as "activity":**
- Clicking anywhere in ShootPath
- Typing in a field
- Scrolling (on some browsers)

**What doesn't count as activity:**
- Having the ShootPath tab open in the background
- Reading content without interacting

**Recommendation:**
Use 4-hour timeout for personal devices. Use 15-minute timeout if you ever log in on public/shared computers.

### API Key Management

API keys are access tokens that allow third-party apps or automation scripts to access your ShootPath data without using your password.

#### What Are API Keys?

**API key = alternate login method:**
Instead of username + password, an app uses an API key to authenticate.

**Example use cases:**
- **Zapier integration** - Automatically create jobs from form submissions
- **Custom scripts** - Export client data for accounting
- **Third-party tools** - Portfolio sites that pull data from ShootPath
- **Mobile apps** - iOS/Android apps use API keys for requests

**API key format:**
`sk_live_abc123def456ghi789` (starts with `sk_live_` or `sk_test_`)

#### Creating API Keys

**Who can create API keys:**
- **Owner** - Can create keys with full permissions
- **Admin** - Can create keys with limited permissions

**How to create:**
1. Go to **Security Settings > API Keys**
2. Click **Create API Key**
3. Enter a **name** (e.g., "Zapier Integration", "Accounting Export Script")
4. Select **permissions**:
   - Read-only (can view data, cannot modify)
   - Read + Write (can create/edit leads, jobs, etc.)
   - Full access (can do anything, including deleting data)
5. Click **Create Key**
6. **Copy the key immediately** - it's only shown once!

**After creation:**
ShootPath displays the full API key. Copy it and store it securely (password manager, environment variables, etc.). You cannot view the full key again - only the last 4 characters.

:::danger API Keys Are Like Passwords
Treat API keys as sensitive as passwords. Anyone with your API key can access your ShootPath data (within the key's permissions). Never share keys publicly, commit them to git repos, or send them via email.
:::

#### Managing Existing API Keys

**View keys:**
Go to **Security Settings > API Keys** to see all your keys:
- **Name** (what you named it)
- **Permissions** (read-only, read-write, full)
- **Last used** (when the key was last used to make an API request)
- **Created** (when you created the key)
- **Key preview** (last 4 characters, e.g., `...j789`)

**Revoke a key:**
1. Find the key in the list
2. Click **"Revoke"**
3. Confirm
4. The key is immediately invalid - apps using it will get "Unauthorized" errors

**When to revoke API keys:**
- You no longer use the integration/script
- The key was exposed or leaked
- A team member who had access to the key left the company
- You're rotating keys for security (good practice every 6-12 months)

**Regenerate a key (rotate):**
1. Create a new API key with the same permissions
2. Update your app/script to use the new key
3. Test that the new key works
4. Revoke the old key

#### API Key Best Practices

**Do:**
- ✅ Use descriptive names ("Zapier - Lead Import", not "Key 1")
- ✅ Use read-only permissions when possible (principle of least privilege)
- ✅ Store keys in environment variables or password managers (not in code)
- ✅ Rotate keys periodically (every 6-12 months)
- ✅ Revoke unused keys immediately

**Don't:**
- ❌ Commit API keys to git repositories
- ❌ Share keys via email, Slack, or unencrypted channels
- ❌ Give full permissions when read-only would suffice
- ❌ Reuse the same key for multiple integrations
- ❌ Store keys in plaintext files on your computer

### Audit Log and Activity Tracking

The audit log records every action taken in your ShootPath account - who did what, when, and from where.

#### What's Tracked

**User actions:**
- Login attempts (successful and failed)
- Password changes
- 2FA enabled/disabled
- Team member added/removed
- Role changes
- API key created/revoked

**Business data changes:**
- Client created/edited/deleted
- Lead status changed
- Job created/moved to different status
- Quote sent/accepted/declined
- Contract sent/signed
- Invoice created/paid
- Gallery uploaded/shared

**Security events:**
- Login from new device/location
- Failed login attempts (multiple in short time)
- Password reset requested
- Session expired
- API request made

**Metadata captured:**
- **Who** - User who performed the action (or "System" for automated actions)
- **What** - Action performed (e.g., "Job status changed to In Production")
- **When** - Exact timestamp
- **Where** - IP address and approximate location
- **How** - Web browser, mobile app, or API

#### Viewing the Audit Log

**Access:**
1. Go to **Security Settings > Audit Log**
2. You'll see a chronological list of actions

**Filters:**
- **Date range** (last 7 days, 30 days, custom range)
- **User** (all users, specific team member)
- **Action type** (logins, data changes, security events)
- **Resource** (all, specific client, job, etc.)

**Search:**
Type keywords to find specific actions (e.g., "invoice 12345" to see all actions on that invoice).

**Example log entries:**

```
[2024-02-06 14:32:18] Emma Chen (emma@example.com)
  → Job #456 status changed from "Editing" to "Delivered"
  → IP: 192.168.1.100 (Seattle, WA)
  → Browser: Chrome 120

[2024-02-06 14:15:03] System
  → Automated email sent: Gallery ready notification to Sarah Thompson
  → Job: #456

[2024-02-06 09:22:45] John Doe (john@example.com)
  → Login successful
  → IP: 203.0.113.45 (Los Angeles, CA)
  → Browser: Safari on iPhone
  → New device detected

[2024-02-05 16:44:12] Emma Chen (emma@example.com)
  → API Key created: "Zapier Integration"
  → Permissions: Read-only
  → IP: 192.168.1.100 (Seattle, WA)
```

#### Why Audit Logs Matter

**Security monitoring:**
Detect unauthorized access or suspicious activity. If you see login attempts from unfamiliar locations, investigate immediately.

**Team accountability:**
Know which team member performed specific actions. Useful if something was changed accidentally or incorrectly.

**Compliance:**
Some industries (legal, healthcare) require audit trails. Even for general photography, it's good practice.

**Troubleshooting:**
If something broke or changed unexpectedly, the audit log helps you understand what happened and when.

**Dispute resolution:**
If a client claims you didn't send a contract or invoice, the audit log proves you did (with timestamp).

#### Audit Log Retention

**Retention period:**
- **Solo plan:** 90 days
- **Studio plan:** 1 year
- **Studio Pro:** 2 years
- **Self-hosted:** Unlimited (you control the database)

**Exporting audit logs:**
1. Go to **Security Settings > Audit Log**
2. Set filters for the data you want
3. Click **Export to CSV**
4. Download the file

Use this to keep permanent records or analyze data in Excel.

### Account Recovery Options

If you lose access to your account, these recovery options help you regain control.

#### Recovery Email

**What it is:**
An alternate email address (different from your login email) used for account recovery.

**Why add one:**
If your primary email is compromised or you lose access to it, you can still recover your ShootPath account via the recovery email.

**How to add:**
1. Go to **Security Settings > Account Recovery**
2. Click **Add Recovery Email**
3. Enter alternate email address
4. ShootPath sends verification email to that address
5. Click verification link
6. Recovery email is now active

**Using recovery email:**
If you're locked out, click "Forgot password?" and select "Use recovery email" option. Password reset link is sent to the recovery email instead of your primary email.

#### Trusted Phone Number

**What it is:**
A phone number where you can receive SMS codes for account recovery.

**How to add:**
1. Go to **Security Settings > Account Recovery**
2. Click **Add Trusted Phone Number**
3. Enter phone number (include country code)
4. ShootPath sends a verification code via SMS
5. Enter the code
6. Phone number is now trusted

**Using trusted phone:**
If locked out and you have 2FA enabled, you can request an SMS code to the trusted phone as a last-resort recovery method.

:::warning SMS Security Note
SMS is less secure than authenticator apps (can be intercepted via SIM swapping). Only use this as a backup recovery method, not for regular 2FA.
:::

#### Security Questions (Not Recommended)

ShootPath does NOT use security questions (e.g., "What's your mother's maiden name?") because they're insecure - answers are often public information or easy to guess.

**Instead, use:**
- Strong password + 2FA (primary security)
- Recovery email (backup access)
- Backup codes (2FA recovery)
- Support verification (last resort)

### Security Best Practices for Photographers

#### Protecting Client Data

**Your responsibilities:**
As a photographer, you handle sensitive client information:
- Names, emails, phone numbers (PII - personally identifiable information)
- Financial data (credit card transactions, payment records)
- Private photos (weddings, family portraits, boudoir)

**Best practices:**
- ✅ Enable 2FA on your ShootPath account
- ✅ Use strong, unique passwords
- ✅ Never share your login credentials with clients or vendors
- ✅ Log out on shared/public computers
- ✅ Keep your computer/phone secure (screen lock, encryption)
- ✅ Only give team members the minimum access they need

#### Team Access Control

**Principle of least privilege:**
Team members should only have access to what they need to do their job.

**Examples:**
- **Associate photographer** - Only see their assigned jobs (Photographer role)
- **VA/Admin assistant** - Read-only access to help with scheduling (Assistant role)
- **Business partner** - Full operational access but not billing (Admin role)

**Review team access regularly:**
- Every 3-6 months, audit your team list
- Remove former employees immediately
- Downgrade permissions if roles change

#### Secure Devices

**Your computer/phone is the gateway to ShootPath:**
- ✅ Use a password/PIN/biometric lock
- ✅ Enable FileVault (Mac) or BitLocker (Windows) full-disk encryption
- ✅ Keep OS and browser updated
- ✅ Use antivirus software
- ✅ Be cautious with public WiFi (use VPN if possible)

#### Phishing Awareness

**Phishing = fake emails/messages trying to steal your password**

**Red flags:**
- Email says "Your account will be suspended, click here to verify"
- Sender address looks close but wrong (e.g., `support@sho0tpath.com` - note the zero)
- Email asks for your password or 2FA code
- Link doesn't go to `shootpath.com`

**What to do:**
- ❌ Never click suspicious links
- ❌ Never enter your password on a site you didn't navigate to directly
- ✅ Type `shootpath.com` in browser manually
- ✅ Check URL bar shows `https://app.shootpath.com`
- ✅ Report phishing emails to support@shootpath.com

**ShootPath will NEVER:**
- Ask for your password via email
- Ask for your 2FA code
- Threaten immediate account suspension
- Send password reset links you didn't request

### What's Next?

Now that your security is locked down, explore other account settings:

**[Business Profile](./business-profile)** - Set up your business name, logo, and contact info

**[User Preferences](./user-preferences)** - Customize notifications, timezone, and display settings

**[Account Setup Overview](./index)** - Return to the account setup checklist

Or configure business features:

**[Team Management](../team/)** - Add team members with appropriate permissions

**[Integrations](../integrations/)** - Securely connect Stripe, Gmail, and other services

---

**Questions?** Look for the help links throughout ShootPath, or reach out to support if you need assistance!
