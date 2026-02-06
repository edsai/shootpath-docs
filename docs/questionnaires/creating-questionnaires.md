---
sidebar_position: 2
---

# Creating Questionnaires

## Quick Reference

Creating a questionnaire in ShootPath is straightforward. Build custom forms to gather exactly the information you need from clients before sessions or events.

**Basic Steps:**
1. Go to **Settings > Questionnaires**
2. Click **New Questionnaire**
3. Add questions using the questionnaire builder
4. Configure field types, options, and requirements
5. Save and assign to workflows or send manually

**Field Types Available:**
- **Short Text** - Single-line text (names, locations)
- **Long Text** - Multi-line text area (descriptions, timelines)
- **Dropdown** - Select one option from a list
- **Checkboxes** - Select multiple options
- **Radio Buttons** - Choose one option (visible)
- **Date Picker** - Calendar date selection
- **Time Picker** - Time selection
- **File Upload** - Photos, PDFs, documents

**Quick Tips:**
- Start with a template and customize
- Group questions into logical sections
- Mark only essential questions as required
- Test before sending to clients
- Use clear, specific question wording

**Next Steps:** Read the detailed guide below or explore [questionnaire examples](./questionnaire-examples).

---

## Detailed Guide

### Accessing the Questionnaire Builder

To create or edit questionnaires:

1. Log into ShootPath admin
2. Go to **Settings** (gear icon in navigation)
3. Select **Questionnaires** from the settings menu
4. Click **New Questionnaire** to create from scratch
5. Or select an existing questionnaire to edit

The questionnaire builder is a visual, drag-and-drop interface that makes creating forms simple.

### Questionnaire Settings

Before adding questions, configure the questionnaire's basic settings:

#### Questionnaire Name

Give your questionnaire a clear, descriptive name that helps you identify it later:
- "Wedding Day Timeline Questionnaire"
- "Portrait Session Prep Form"
- "Newborn Photography Details"
- "Commercial Project Brief"

**Good naming:** Specific to the job type and purpose
**Avoid:** Generic names like "Questionnaire 1" or "Client Form"

This name is for your reference—clients don't see it. It appears in settings, workflow configuration, and when selecting which questionnaire to send.

#### Internal Description (Optional)

Add notes for yourself or team members:
- When to send this questionnaire
- What job types it's designed for
- Any special instructions

Example: "Send 4-6 weeks before wedding date. Covers timeline, family groupings, and vendor contacts."

#### Intro Message

This appears at the top of the questionnaire when clients open it. Set expectations and explain why you're asking these questions.

**Example intro message:**
> "Thanks for booking your wedding photography with us! This questionnaire helps me prepare for your big day. Your answers ensure I capture all the important moments and people. It takes about 10-15 minutes to complete. You can save your progress and come back later if needed!"

**What to include:**
- Friendly greeting
- Purpose of the questionnaire
- Estimated time to complete
- Any special instructions
- Reassurance about privacy

#### Completion Message

This appears after the client submits the questionnaire. Thank them and set next-step expectations.

**Example completion message:**
> "Thank you! I've received your responses and will review them carefully. I'll reach out within 48 hours if I have any follow-up questions. Looking forward to your session!"

**What to include:**
- Thank you
- What happens next
- Timeline for your response
- Reassurance

### Adding Questions

Now for the fun part—building your question list!

#### Creating a New Question

1. Click **Add Question** in the builder
2. Select the field type (text, dropdown, checkbox, etc.)
3. Enter your question text
4. Configure field-specific options
5. Set whether it's required or optional
6. Add help text or examples if needed

#### Question Text Best Practices

Write clear, specific questions that clients can answer without confusion:

**Too vague:** "Tell me about your wedding"
**Better:** "What time does your ceremony begin, and approximately how long will it last?"

**Too complex:** "Please list all family members, their relationships, and desired groupings for formal photographs"
**Better:** "Who are the key family members you'd like in formal photos?" (with examples)

**Tips:**
- Ask one thing per question (don't combine multiple questions)
- Use plain language, avoid jargon
- Be specific about format (dates, times, names)
- Provide context when necessary

#### Help Text and Examples

Most field types let you add optional help text that appears below the question. Use this to:
- Clarify what you're asking
- Provide examples
- Explain why you need this information

**Question:** "What's your vision for this session?"
**Help text:** "Example: Natural, candid moments in golden hour light with soft, warm tones. Or: Moody, editorial-style portraits with dramatic lighting."

Help text makes the difference between vague, one-word answers and detailed, useful responses!

### Field Types Explained

Choose the right field type for each question:

#### Short Text Field

Single-line text input for brief answers.

**Best for:**
- Names
- Locations
- Phone numbers
- Email addresses
- Short descriptive answers

**Configuration options:**
- Required or optional
- Character limit (optional)
- Placeholder text

**Example questions:**
- "What's the venue name and address?"
- "Who is your main contact for day-of coordination?"
- "What's your fiancé's full name?"

#### Long Text Field (Text Area)

Multi-line text box for longer responses.

**Best for:**
- Detailed timelines
- Special requests
- Background stories
- Open-ended questions
- Lists

**Configuration options:**
- Required or optional
- Rows (how tall the box appears)
- Character limit (optional)

**Example questions:**
- "Please describe your wedding day timeline from start to finish"
- "Are there any special moments, traditions, or surprises we should be aware of?"
- "What's most important to you about your session?"

:::tip When to Use Text Areas
Use text areas for questions where you want detailed, thoughtful responses. Don't use them for simple answers that fit in one line!
:::

#### Dropdown (Select)

Menu where clients select one option from a list.

**Best for:**
- Predefined choices
- Time ranges
- Style preferences
- Package add-ons

**Configuration options:**
- Required or optional
- List of options (add as many as needed)
- Default selection (optional)

**Example questions:**
- "What time of day works best for your session?"
  - Morning (before 10am)
  - Midday (10am-2pm)
  - Afternoon (2pm-5pm)
  - Evening/Sunset (after 5pm)
- "What's your photography style preference?"
  - Light and Airy
  - Moody and Dramatic
  - True to Color
  - Black and White

**When to use dropdowns vs radio buttons:**
- Dropdown: More than 5 options (saves space)
- Radio buttons: 5 or fewer options (easier to scan)

#### Radio Buttons

Visible options where clients select one.

**Best for:**
- Yes/No questions
- Few options (2-5)
- Important choices you want clearly visible

**Configuration options:**
- Required or optional
- List of options
- Vertical or horizontal layout

**Example questions:**
- "Do you want an engagement session?"
  - Yes, please!
  - No, thanks
  - Maybe - let's discuss
- "Indoor or outdoor session?"
  - Indoor
  - Outdoor
  - Both

Radio buttons make options obvious at a glance, while dropdowns hide options until clicked.

#### Checkboxes

Multiple selection—clients can choose as many as apply.

**Best for:**
- Must-have shots
- Family groupings
- Features to include
- Style preferences

**Configuration options:**
- Required or optional
- Minimum/maximum selections
- List of options

**Example questions:**
- "Which family combinations would you like photos of?"
  - Bride with parents
  - Groom with parents
  - Bride with siblings
  - Groom with siblings
  - Both sets of parents together
  - Full extended family
- "What are your must-have shots?"
  - First look
  - Ceremony exit
  - First dance
  - Cake cutting
  - Bouquet toss
  - Grand exit

**Pro tip:** Add "Other (please specify)" with a text field for anything you didn't list.

#### Date Picker

Calendar widget for selecting dates.

**Best for:**
- Session dates
- Preferred dates
- Deadlines
- Important milestones

**Configuration options:**
- Required or optional
- Allow past dates
- Allow future dates only
- Date range restrictions

**Example questions:**
- "What's your preferred session date?"
- "When is your baby due?"
- "What's your event date?"

Date pickers prevent formatting errors (no more "12/5" when you need "December 5, 2024").

#### Time Picker

Time selection widget.

**Best for:**
- Session start times
- Event schedule
- Availability windows

**Configuration options:**
- Required or optional
- 12-hour or 24-hour format
- Minute intervals (15-min, 30-min, etc.)

**Example questions:**
- "What time does your ceremony start?"
- "What time should we arrive?"
- "What time would you like to begin the session?"

#### File Upload

Allows clients to attach files.

**Best for:**
- Inspiration photos
- Venue maps
- Shot list documents
- Reference images
- Mood boards

**Configuration options:**
- Required or optional
- Accepted file types (jpg, png, pdf, etc.)
- File size limit
- Maximum number of files

**Example questions:**
- "Upload any inspiration photos that represent your vision"
- "Attach your venue map or layout diagram (PDF)"
- "Share photos of your nursery or props you'd like to include"

**Important:** Be clear about file format and size. Clients uploading from phones may have large image files.

### Organizing Questions with Sections

For longer questionnaires (10+ questions), group related questions into sections:

#### Creating Sections

1. Click **Add Section** in the builder
2. Give the section a name
3. Optionally add section description
4. Drag questions into the section

#### Section Examples

**Wedding questionnaire sections:**
- Basic Information (names, date, venue)
- Timeline & Schedule (ceremony, reception, events)
- People & Groupings (wedding party, family formals)
- Preferences & Details (style, must-haves, special requests)

**Portrait session sections:**
- Session Logistics (date, location, time)
- Who's Involved (names, ages, relationships)
- Style & Preferences (wardrobe, vibe, must-haves)
- Special Considerations (mobility, shyness, surprises)

Sections make long forms feel manageable. Clients think "Just two more sections!" instead of "20 more questions?!"

### Required vs Optional Fields

Mark fields as required only when you truly need the answer to proceed.

#### When to Require a Field

Make fields required when:
- You can't prepare without this information (session date, location)
- It affects pricing or deliverables (number of people, add-ons)
- It's critical for safety or logistics (allergies, mobility concerns)
- You need it for legal or business purposes (names for contracts)

#### When to Make Fields Optional

Make fields optional when:
- It's a nice-to-have but not essential
- Not all clients will have an answer (some families don't want formal groupings)
- It's exploratory ("Any special requests?" is fine to leave blank)
- You're gathering ideas rather than requirements

**Rule of thumb:** If you'd still do the session without this answer, make it optional.

:::caution Required Fields
Every required field is a potential barrier to completion. If a client doesn't know an answer, they might abandon the form. Only require essentials!
:::

### Conditional Logic

Advanced feature: Show or hide questions based on previous answers.

#### How Conditional Logic Works

1. Create a question that determines what shows next
2. Add conditional questions
3. Set rules: "Show this question if previous answer is X"

#### Conditional Logic Examples

**Example 1: Engagement session**
- Question: "Do you want to include an engagement session?"
  - Yes
  - No
- If "Yes" → Show: "When would you like to schedule your engagement session?"
- If "No" → Skip that question

**Example 2: Indoor/outdoor**
- Question: "Will your session be indoors or outdoors?"
  - Indoor
  - Outdoor
  - Both
- If "Outdoor" or "Both" → Show: "What's your backup plan if weather doesn't cooperate?"
- If "Indoor" → Skip weather question

**Benefits:**
- Clients only see relevant questions
- Shorter, more focused forms
- Better user experience

**When to use conditional logic:**
- You have branching scenarios
- Some questions only apply to certain clients
- You want to keep forms short and relevant

**When NOT to use conditional logic:**
- Simple, short questionnaires (adds unnecessary complexity)
- Questions that apply to everyone
- You're just starting with questionnaires (keep it simple first!)

### Default Questionnaires vs Custom

ShootPath includes default questionnaires for common photography types. You can:
1. Use defaults as-is
2. Duplicate and customize defaults
3. Create completely custom questionnaires

#### Using Default Questionnaires

Default questionnaires cover:
- Wedding photography
- Portrait sessions
- Newborn photography
- Event photography
- Family sessions

These are based on best practices and common needs. They're great starting points!

**To use a default:**
1. Go to Settings > Questionnaires
2. Find the default template you want
3. Assign it to workflows or send it manually
4. No configuration needed!

#### Customizing Default Questionnaires

To adapt a default to your style:

1. Find the default questionnaire
2. Click **Duplicate**
3. Rename it (e.g., "My Custom Wedding Questionnaire")
4. Edit questions to match your process
5. Add/remove questions as needed
6. Save your custom version

Now you have the convenience of a template with your unique touches!

#### Creating Fully Custom Questionnaires

For unique needs:

1. Click **New Questionnaire**
2. Build from scratch using the field types
3. Organize with sections
4. Configure settings
5. Test thoroughly
6. Assign to workflows

### Testing Your Questionnaire

Before sending to clients, always test!

#### How to Test

1. In the questionnaire editor, click **Preview**
2. Fill out the form as a client would
3. Try different answer combinations
4. Submit the form
5. Check how responses appear in admin view

#### What to Test

**Question clarity:** Can you understand what's being asked?

**Field validation:** Do required fields block submission if empty?

**Conditional logic:** Do questions show/hide correctly based on answers?

**Mobile experience:** Does it work well on a phone screen?

**Completion time:** How long does it take to fill out?

**Completion message:** Does the thank-you message display properly?

#### Common Issues to Catch

- Questions are ambiguous or confusing
- Too many required fields (frustrating for clients)
- Text areas too small for expected answers
- Dropdown options missing common choices
- Help text that doesn't actually help
- Typos or grammatical errors

Fix these before sending to real clients!

### Sending Questionnaires

Once created, you can send questionnaires in two ways:

#### Automatic via Workflows

Integrate questionnaires into your workflows for automatic sending:

1. Go to **Settings > Workflows**
2. Edit the workflow you want to use
3. Add a task: "Send Questionnaire"
4. Select which questionnaire to send
5. Set the trigger (e.g., "3 weeks before session date" or "After contract signed")
6. Save workflow

Now every job using that workflow will automatically send the questionnaire at the right time!

[Learn more about workflow automation →](../workflows/email-automation)

#### Manual Sending

To send a questionnaire manually:

1. Open the job
2. Go to **Actions** or **Workflow** tab
3. Click **Send Questionnaire**
4. Select which questionnaire
5. Optionally customize the email message
6. Click **Send**

Client receives an email with a link to complete the questionnaire.

### Managing Responses

After clients submit questionnaires:

#### Viewing Responses

1. Open the job
2. Go to **Questionnaire** tab
3. View all submitted responses

Responses are organized by section (if you used sections) and displayed clearly.

#### Downloading Responses

You can download responses as:
- **PDF** - Print or save for offline reference
- **CSV** - Import into spreadsheets
- **Plain Text** - Copy/paste into other systems

#### Editing Responses

If a client made a mistake or needs to update an answer:

1. Open the questionnaire responses
2. Click **Edit Response** (if enabled)
3. Make changes
4. Save

Or send them a new link to re-submit (previous submission is replaced).

#### Responding to Clients

If responses need follow-up:
- Note unclear or incomplete answers
- Send email or text asking for clarification
- Reference specific questions: "On the questionnaire, you mentioned..."
- Follow up before the session, not during!

### Questionnaire Settings and Permissions

#### Client-Facing Settings

**Allow clients to save and return later:** For long questionnaires, let clients save progress without submitting. They receive a link to return and finish later.

**Allow clients to edit after submission:** Clients can update their responses after submitting (useful if details change).

**Require submission before session:** Block other workflow tasks until questionnaire is complete (ensures you always have the info you need).

#### Admin Settings

**Notification preferences:** Get notified when questionnaires are submitted.

**Auto-reminders:** Send reminder emails if not completed within X days.

**Deadline enforcement:** Set a deadline for completion (e.g., "Complete 1 week before session").

### Tips for Better Questionnaires

**Start Simple**

Your first questionnaire doesn't need to be perfect. Start with 10-12 essential questions and refine over time based on what you actually use.

**Get Feedback from Clients**

After a few sessions, ask clients: "Was the questionnaire helpful? Were any questions confusing?" Adjust based on their input.

**Update Seasonally**

Review questionnaires every few months:
- Remove questions you never reference
- Add questions based on things clients always ask
- Update examples to stay current

**Use Plain Language**

Write for real humans, not robots:
- "Who will be in your photos?" not "Participant enumeration"
- "What time should we arrive?" not "Commencement temporal parameters"

**Provide Context**

Tell clients why you're asking:
- "This helps me pack the right gear"
- "Knowing this ensures we capture all the key moments"
- "Your answer helps me plan the perfect session for you"

**Respect Their Time**

Every question should have a purpose. If you won't use the answer, don't ask the question!

### Troubleshooting Common Issues

**Clients aren't filling out questionnaires:**
- Make them shorter (remove non-essential questions)
- Send reminders (workflow automation helps)
- Explain the benefit ("This ensures I'm fully prepared!")
- Set a friendly deadline

**Clients give one-word answers to open-ended questions:**
- Provide better examples in help text
- Ask more specific questions
- Break complex questions into smaller ones
- Use field types that guide responses (checkboxes, dropdowns)

**Responses are incomplete or unclear:**
- Mark essential questions as required
- Add help text with examples
- Follow up with clients before the session
- Refine questions based on patterns

**Questionnaires feel too long:**
- Use sections to break them up
- Enable "save and return later" feature
- Remove questions that aren't actionable
- Use conditional logic to hide irrelevant questions

**Mobile experience is poor:**
- Test on an actual phone before sending
- Avoid complex layouts
- Use mobile-friendly field types
- Keep section names short

### Advanced Techniques

Once you're comfortable with basics, try these:

#### Question Templates

Create reusable question snippets you can insert into any questionnaire:
- "Family formal groupings" question with standard options
- "Timeline section" with standard scheduling questions
- "Style preferences" with your standard options

Save time by reusing well-crafted questions across multiple questionnaires.

#### Job Type-Specific Questionnaires

Create specialized versions for different photography types:
- **Wedding (full day)** - Comprehensive timeline, 25+ questions
- **Wedding (elopement)** - Simplified, 10-12 questions
- **Portrait (extended)** - Detailed style/location questions
- **Portrait (mini)** - Essential logistics only, 5-7 questions

Assign the right questionnaire to the right job type automatically via workflows.

#### Multi-Language Questionnaires

If you serve clients who speak different languages:
- Create duplicate questionnaires in each language
- Name them clearly ("Wedding Questionnaire - Spanish")
- Send the appropriate version based on client preference

#### Integration with Other Tools

Export questionnaire responses to:
- **Google Sheets** - Analyze trends across clients
- **Notion/Airtable** - Build custom dashboards
- **Timeline tools** - Import wedding timelines
- **Shot list apps** - Generate shot lists from responses

### Examples of Great Questions

**Logistics:**
- "What's the full address where we should meet you?"
- "Where can we park? Do we need any special access codes or permissions?"
- "What time should we arrive, and when do you want us to wrap up?"

**Style & Vision:**
- "If your session was a mood board, what words would describe it?" (Examples: Romantic, playful, elegant, adventurous, intimate)
- "Show me 3-5 photos you love (from any photographer) and tell me what you like about them"
- "What do you want to feel when you look at these photos in 10 years?"

**People & Relationships:**
- "Tell me about each person who will be in the photos—names, ages, personalities, any special considerations"
- "Are there any relationship dynamics I should know about?" (Example: Recently blended family, shy teenager, someone with mobility concerns)
- "Who are the VIPs we absolutely must capture?"

**Practical Considerations:**
- "Is there anything that would make this session more comfortable for you?" (Mobility concerns, sensory sensitivities, preferred pronouns, etc.)
- "What's your plan B if weather doesn't cooperate?"
- "Is there anything you're worried about, or any questions you have for me?"

### What's Next?

Now that you know how to create questionnaires, explore:

**[Client Experience](./client-experience)** - See what clients experience when filling out questionnaires

**[Questionnaire Examples](./questionnaire-examples)** - Copy-paste templates for different photography types

**[Workflows](../workflows/)** - Automate questionnaire sending

---

**Questions?** Look for the help links throughout ShootPath, or use the support widget if you need assistance!
