---
sidebar_position: 2
---

# Login Issues

## Quick Reference

Having trouble logging in to ShootPath? This guide covers the most common login problems and how to resolve them, from forgotten passwords to account lockouts.

**Common Login Problems:**
- Forgot password → Use password reset
- Email not recognized → Check spelling or try alternate email
- Account locked → Wait 30 minutes or contact support
- Two-factor authentication not working → Use backup code
- Password reset email not received → Check spam folder

**Quick Fixes:**
- **Clear browser cookies:** Settings → Privacy → Clear cookies
- **Try incognito mode:** Ctrl+Shift+N (Windows) or Cmd+Shift+N (Mac)
- **Check Caps Lock:** Password is case-sensitive
- **Use correct email:** The one you signed up with

:::tip Most Common Issue
90% of login problems are caused by:
1. Using wrong email address (try all your email addresses)
2. Caps Lock accidentally on (passwords are case-sensitive)
3. Browser remembering old password (clear saved passwords)
:::

---

## Detailed Guide

### Can't Log In - General Troubleshooting

If you see "Invalid email or password" when trying to log in:

**Step 1: Verify Your Email**
- Make sure you're using the email address you signed up with
- Check for typos (common: .com vs .net, gmail vs yahoo)
- Try all email addresses you might have used

**Step 2: Check Your Password**
- Is Caps Lock on? Passwords are case-sensitive
- Are you typing it correctly? Reveal the password (click the eye icon) to check
- Is your browser auto-filling an old password? Clear saved passwords and type manually

**Step 3: Clear Browser Cookies**
Old session cookies can interfere:

**Chrome:**
1. Click three dots → Settings
2. Privacy and security → Cookies and other site data
3. See all site data and permissions
4. Search for "shootpath.com"
5. Click trash icon to remove
6. Refresh the login page

**Safari:**
1. Safari → Settings → Privacy
2. Manage Website Data
3. Search for "shootpath"
4. Remove → Done
5. Refresh the login page

**Firefox:**
1. Menu → Settings → Privacy & Security
2. Cookies and Site Data → Manage Data
3. Search for "shootpath"
4. Remove Selected → Save Changes
5. Refresh the login page

**Step 4: Try Incognito/Private Mode**
This tests if browser extensions or cache are the problem:
1. Open an incognito/private window (Ctrl+Shift+N or Cmd+Shift+N)
2. Go to shootpath.com/login
3. Try logging in

If it works in incognito:
- Clear your normal browser cache and cookies
- Disable browser extensions one-by-one to find the culprit
- Update your browser to the latest version

**Step 5: Reset Your Password**
If you still can't log in, your password might be wrong. See [Password Reset](#password-reset) below.

### Password Reset

If you've forgotten your password or suspect it's incorrect:

**How to Reset:**
1. Go to [shootpath.com/login](https://shootpath.com/login)
2. Click **Forgot Password?**
3. Enter your email address (the one you used to sign up)
4. Click **Send Reset Link**
5. Check your email for a password reset message

**Email Not Received?**
See [Email Not Received](#email-not-received) section below.

**Clicking the Reset Link:**
1. Check your email (including spam folder)
2. Look for subject: "Reset your ShootPath password"
3. Click the **Reset Password** button in the email
4. You'll be taken to a page where you can enter a new password

**Creating a Strong Password:**
Your new password must be:
- At least 8 characters long
- Include at least one uppercase letter (A-Z)
- Include at least one lowercase letter (a-z)
- Include at least one number (0-9)
- Include at least one special character (!@#$%^&*)

**Recommended:**
- 12+ characters
- Mix of random words (e.g., "Blue$Sky42Running!")
- Use a password manager to generate and store it
- Don't reuse passwords from other sites

**After Resetting:**
1. Enter your new password twice
2. Click **Reset Password**
3. You'll be automatically logged in
4. Update your password manager if you use one

### Email Not Received

If you're not receiving password reset emails (or any emails from ShootPath):

**Step 1: Check Spam/Junk Folder**
- Open your email client
- Go to Spam, Junk, or Promotions folder
- Search for "shootpath" or "noreply@shootpath.com"
- If found, mark as "Not Spam" and move to inbox

**Step 2: Check Email Address**
- Did you enter the correct email when requesting reset?
- Try all email addresses you might have used to sign up
- Common mistakes:
  - Swapping .com with .net
  - Forgetting a number or underscore
  - Using an old work email vs personal email

**Step 3: Whitelist ShootPath**
Add our email address to your contacts or safe sender list:
- noreply@shootpath.com
- support@shootpath.com
- *@shootpath.com (to whitelist all ShootPath emails)

**Gmail:**
1. Open Gmail → Settings → Filters and Blocked Addresses
2. Create a new filter
3. From: noreply@shootpath.com
4. Never send it to Spam
5. Create filter

**Outlook:**
1. Settings → Mail → Junk email
2. Safe senders and domains → Add
3. noreply@shootpath.com
4. Save

**Yahoo:**
1. Settings → More Settings → Filters
2. Add new filter
3. From contains: shootpath.com
4. Move to folder: Inbox
5. Save

**Step 4: Check Email Service Issues**
Some corporate or school email systems block external emails:
- Ask your IT department if they block emails from shootpath.com
- Try using a personal email (Gmail, Yahoo, etc.) for your ShootPath account

**Step 5: Wait and Retry**
Sometimes email delivery is delayed:
- Wait 15 minutes
- Check spam again
- Try requesting the reset email again
- Still nothing? Contact support (see Step 6)

**Step 6: Contact Support**
If you still haven't received the email after 30 minutes:
1. Email [support@shootpath.com](mailto:support@shootpath.com)
2. Subject: "Password reset email not received"
3. Include:
   - The email address you're trying to reset
   - When you requested the reset (date and time)
   - Confirmation that you checked spam
4. We'll manually send a reset link or help you regain access

### Two-Factor Authentication Problems

If you enabled two-factor authentication (2FA) and can't complete login:

**Problem: Don't Have My Phone**

**Solution: Use Backup Code**
1. When prompted for 2FA code, click **Use a backup code**
2. Enter one of the backup codes you saved when setting up 2FA
3. You'll be logged in
4. Each backup code can only be used once
5. Go to **Settings → Security** to generate new backup codes

**If You Lost Your Backup Codes:**
- Contact [support@shootpath.com](mailto:support@shootpath.com)
- Subject: "Lost 2FA device and backup codes"
- We'll verify your identity and disable 2FA so you can log in

**Problem: 2FA Code Not Working**

**Solution 1: Check Time Sync**
Authenticator apps rely on accurate device time:

**iPhone:**
1. Settings → General → Date & Time
2. Enable "Set Automatically"
3. Close and reopen your authenticator app
4. Try the new code

**Android:**
1. Settings → System → Date & time
2. Enable "Automatic date & time"
3. Enable "Automatic time zone"
4. Force close authenticator app and reopen
5. Try the new code

**Solution 2: Wait for New Code**
- Codes change every 30 seconds
- Wait for the next code to generate
- Enter it immediately (don't wait too long)

**Solution 3: Type Code Manually**
- Don't copy-paste (sometimes adds spaces)
- Type the 6-digit code manually
- No spaces, no dashes, just numbers

**Problem: Lost Access to Authenticator App**

**If You Have Backup Codes:**
Use them to log in (see above), then disable 2FA and set up new authenticator.

**If You Don't Have Backup Codes:**
1. Email [support@shootpath.com](mailto:support@shootpath.com)
2. Subject: "Lost access to 2FA authenticator"
3. Include:
   - Your account email
   - Last successful login date (if you remember)
   - Description of what happened
4. We'll verify your identity through:
   - Secret question you set up
   - Payment method on file (last 4 digits)
   - Recent activity in your account
5. Once verified, we'll disable 2FA so you can log in

**Preventing This in the Future:**
- Save backup codes in a secure place (password manager, safe)
- Set up 2FA on multiple devices
- Use an authenticator app that syncs (like Authy)

### Account Locked

If you see "Your account has been locked," it means there were too many failed login attempts.

**Why Accounts Get Locked:**
- 5 failed login attempts in 15 minutes
- Protects your account from brute force attacks
- Automatic security measure

**How to Unlock:**

**Option 1: Wait 30 Minutes**
- Accounts auto-unlock after 30 minutes
- The timer starts from the last failed attempt
- Don't try logging in during this time (it resets the timer)

**Option 2: Use Password Reset**
- Click **Forgot Password?** on the login page
- Follow the password reset process
- This unlocks your account immediately
- You'll be able to log in with your new password

**Option 3: Contact Support**
For urgent access:
1. Email [support@shootpath.com](mailto:support@shootpath.com)
2. Subject: "Account locked - urgent"
3. Include your account email
4. We can manually unlock your account during business hours

**Preventing Lockouts:**
- Use a password manager to avoid typos
- Reset your password if you're not sure what it is
- Don't let browsers auto-fill old passwords

### Browser Cookie/Cache Issues

Sometimes login problems are caused by corrupted cookies or cache:

**Full Browser Reset (All Browsers):**

**Step 1: Clear ShootPath Cookies**
(See instructions in [Can't Log In](#cant-log-in-general-troubleshooting) above)

**Step 2: Clear ShootPath Cache**

**Chrome:**
1. Click three dots → More tools → Clear browsing data
2. Time range: All time
3. Check: Cookies and Cached images
4. Click **Clear data**

**Safari:**
1. Safari → Settings → Advanced
2. Check "Show Develop menu in menu bar"
3. Develop → Empty Caches
4. Safari → Settings → Privacy → Manage Website Data → Remove All

**Firefox:**
1. Menu → Settings → Privacy & Security
2. Cookies and Site Data → Clear Data
3. Check both boxes → Clear

**Step 3: Disable Browser Extensions**
Extensions can interfere with login:
1. Open incognito/private window (Ctrl+Shift+N or Cmd+Shift+N)
2. Try logging in
3. If it works, an extension is causing the issue
4. In regular browser: Disable extensions one-by-one to find the culprit

**Common Problematic Extensions:**
- Ad blockers (uBlock Origin, AdBlock Plus)
- Privacy tools (Privacy Badger, Ghostery)
- Password managers (if misconfigured)
- VPN extensions

**Step 4: Update Your Browser**
Old browsers have security and compatibility issues:
- Chrome: Menu → Help → About Google Chrome → Update
- Safari: Update via macOS Software Update
- Firefox: Menu → Help → About Firefox → Update
- Edge: Menu → Help → About Microsoft Edge → Update

**Step 5: Try a Different Browser**
If all else fails:
1. Download Chrome (if you don't have it)
2. Try logging in with Chrome
3. If it works, the issue is with your original browser
4. Consider switching browsers or reinstalling your original browser

### Using Wrong Email Address

One of the most common issues: You're trying to log in with the wrong email.

**How to Find Your ShootPath Email:**

**Check Old Emails:**
1. Search your email for "shootpath" or "welcome to shootpath"
2. Your signup confirmation email will show the email address you used
3. Also check for invoices or password reset emails

**Try All Your Email Addresses:**
If you have multiple email addresses:
- Personal Gmail
- Work email
- Old work email (if you changed jobs)
- Alternative spelling (firstname.lastname@ vs firstnamelastname@)

**Contact Support:**
If you can't figure out which email you used:
1. Email [support@shootpath.com](mailto:support@shootpath.com) from ALL your email addresses
2. Subject: "Can't remember my account email"
3. Include:
   - Your name
   - Your business name
   - Approximate signup date
4. We'll search for your account and confirm the email address

### Error Messages and What They Mean

**"Invalid email or password"**
- Most common cause: Wrong password
- Solution: Reset your password or try a different email address

**"Account not found"**
- You're using an email address that's not registered
- Solution: Try another email or sign up for a new account

**"Your account has been locked"**
- Too many failed login attempts
- Solution: Wait 30 minutes or reset your password

**"Session expired"**
- You were logged in but your session timed out (4 hours of inactivity)
- Solution: Just log in again

**"Email already in use"**
- You're trying to sign up with an email that already has an account
- Solution: Use the login page (not signup) or reset your password

**"Two-factor authentication required"**
- Your account has 2FA enabled
- Solution: Enter code from your authenticator app or use a backup code

**"Too many requests, please try again later"**
- You've made too many login attempts too quickly
- Solution: Wait 5-10 minutes and try again

**"This browser is not supported"**
- You're using Internet Explorer or a very old browser
- Solution: Update your browser or use Chrome, Safari, Firefox, or Edge

### Login on Mobile App

Mobile app login works similarly to web login, but with a few differences:

**Can't Log In on Mobile App:**

**Step 1: Check App Version**
- iOS: App Store → Updates → Update ShootPath
- Android: Play Store → My apps → Update ShootPath

**Step 2: Check Internet Connection**
- The app requires internet to log in (no offline mode)
- Try switching between WiFi and cellular
- Try opening a website in your browser to confirm internet works

**Step 3: Use Same Credentials as Web**
- Email and password are the same as web login
- If you can log in on web but not mobile, the app may need updating

**Step 4: Clear App Cache**
- iOS: Delete the app and reinstall from App Store (your data is safe on our servers)
- Android: Settings → Apps → ShootPath → Storage → Clear cache (don't clear data yet)

**Step 5: Reinstall the App**
- Delete ShootPath app
- Restart your phone
- Download and install ShootPath again
- Try logging in

**Mobile 2FA:**
- If 2FA is enabled, you'll be prompted for a code after entering password
- Use your authenticator app on the same device or another device
- Or use a backup code

### Multiple Accounts / Wrong Account

If you accidentally created multiple ShootPath accounts:

**Identifying Which Account:**
1. Check which email address receives ShootPath notifications
2. Log in with each email to see which has your data
3. The account with your clients, jobs, and settings is the one you want

**Consolidating Accounts:**
We can't automatically merge accounts, but you can:
1. Export data from the unwanted account
2. Import it into your main account (manual process)
3. Cancel the unwanted account

Contact [support@shootpath.com](mailto:support@shootpath.com) for help with this process.

**Switching Between Accounts:**
If you legitimately need multiple accounts (e.g., multiple businesses):
1. Log out from one account
2. Log in with the other email
3. Or use different browsers (Chrome for account A, Firefox for account B)
4. Or use incognito for the second account

---

## Common Questions

**How many times can I try logging in before getting locked out?**
5 failed attempts within 15 minutes will lock your account for 30 minutes.

**Can I change my login email address?**
Yes:
1. Log in to ShootPath
2. Go to **Settings → Account → Email Address**
3. Enter your new email and confirm
4. Verify the new email (we'll send a confirmation link)
5. Once verified, log in with the new email

**Why does ShootPath keep logging me out?**
Security timeout after 4 hours of inactivity. Check "Remember Me" when logging in to stay logged in for 30 days (on trusted devices only).

**Can I log in from multiple devices?**
Yes! You can be logged in on multiple devices simultaneously (laptop, phone, tablet, etc.). Your data syncs across all devices.

**Do I need to log in every time I visit ShootPath?**
No, if you check "Remember Me" when logging in, you'll stay logged in for 30 days (or until you log out manually).

**Can I use a password manager?**
Yes! Password managers like 1Password, LastPass, or Bitwarden work great with ShootPath. They can auto-fill your credentials and store strong unique passwords.

**What if someone else has access to my account?**
1. Change your password immediately
2. Check **Settings → Security → Active Sessions** and log out all other sessions
3. Enable two-factor authentication
4. Review recent activity in your account
5. Contact [support@shootpath.com](mailto:support@shootpath.com) if you see suspicious changes

**Can I disable two-factor authentication?**
Yes:
1. Log in to ShootPath
2. Go to **Settings → Security**
3. Click **Disable Two-Factor Authentication**
4. Confirm by entering a 2FA code
5. 2FA is now disabled (not recommended for security)

---

## Still Can't Log In?

If you've tried everything and still can't access your account:

**Contact Support:**
Email [support@shootpath.com](mailto:support@shootpath.com)

**Include:**
- The email address you're trying to use
- Description of what happens when you try to log in
- Screenshots of error messages
- Steps you've already tried
- Your browser and version (find at [whatismybrowser.com](https://whatismybrowser.com))

**Response Time:**
- Starter plan: Within 48 hours
- Professional plan: Within 24 hours
- Studio plan: Within 12 hours

We'll help you regain access as quickly as possible.
