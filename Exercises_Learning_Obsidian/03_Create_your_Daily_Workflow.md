# Your Daily Note
*(Duration approx. 15min)*

*The proposed Daily Note template can enhance your workflow by:*

- **Displaying all to-dos:** *Automatically reminds you of tasks planned for today (or later), regardless of when they were set.*
- **Daily Log section:** *Encourages brief reflections on daily achievements, challenges, and insights. Can be used for end-of-day reviews or setting daily focus.*
- **Promoting regular Obsidian use:** *Provides a clear starting point of each day, increasing the likelihood of long-term Obsidian integration into your work routine.*

*Remember, adapt these features to suit your personal workflow. The key is finding an approach that works best for you.*

**Learning Objectives in this Exercise:**
- *How to use **Community Plugins**.*
	- *Templater by SilentVoid*
	- *Dataview by Michael Brenan*
	- *Tasks by Clare Macrae and Ilyas Landikov*
- *How to use Templates for a Daily Note.*

## 1. Community Plugins

*Community plugins in Obsidian are user-created extensions that expand the app's functionality beyond its core features. Developed by the Obsidian community, these plugins let users customize their note-taking experience to fit their unique needs and workflows.*

<details>
<summary>Potential Risks of Community Plugins</summary>
<br>
While community plugins offer great flexibility and power, they can also pose potential risks:

1. **Security concerns**: As these plugins are not officially vetted by Obsidian, they may contain malicious code.
2. **Stability issues**: Community plugins may introduce bugs or conflicts that could impact Obsidian's performance.
3. **Maintenance uncertainty**: There's no guarantee that a plugin will be supported long-term, potentially leading to compatibility issues down the line.
<br>
</details>

<details>
<summary>How to Check whether a Plugin is Dangerous</summary>
<br>
To assess the safety and reliability of a community plugin, consider the following steps:

1. **Check Plugin Reviews**: Look for user feedback in the community (e.g. on Discord) or on the Obsidian forum. Reviews can highlight issues or security concerns.
2. **Inspect the Source Code**: Open the plugin’s source code (available on GitHub) and check for any suspicious or untrusted code.
3. **Check for Regular Updates**: Ensure the plugin is actively maintained. A lack of updates could indicate potential security risks.
4. **Plugin Permissions**: Be cautious if a plugin asks for excessive permissions that seem unnecessary for its function.
5. **Trusted Developers**: Use plugins from well-known, trusted developers or those with a strong community presence.

Remember, Obsidian keeps community plugins disabled by default ("restricted mode"). You must manually enable them, which serves as a built-in safety measure.
<br>
</details>

## 2. Install Community Plugins for Your Daily Workflow

1. Enable the community plugins: **Settings** → Click **Turn on community plugins**
2. Click **Browse** → search for the plugin **"Dataview by Michael Brenan"** → install the plugin → click **Enable**
3. Repeate this for the community plugins **"Tasks by Clare Macrae and Ilyas Landikov"** and **"Templater by SilentVoid"**

## 3. Create Folder and Notes for Your Daily Workflow

1. **Create a folder named "DAILY NOTES" in the folder "BACKEND"**
2. **Create a folder named "TEMPLATES" in the folder "BACKEND"**

**EITHER**

3. **Create a note called "Template_Daily_Note" and move it into the "TEMPLATES" folder.**
4. **Select one of the templates from the GitHub folder "Obsidian-for-Researcher/Materials-for-the-Exercises/Templates" and copy the content into the note you have created:**

   [Daily Note Basic](https://github.com/nfuchs-DSC/Obsidian-for-Researchers/blob/7495e7b4582fdaf896b12761988c5e9b1421e2de/Materials-for-the-Exercises/Templates/Template_Daily_Note_basic.md)<br>
	→ This template includes sections for: Daily Thoughts, New Tasks, Tasks Due Today, Upcoming Tasks, Completed Tasks, and Overdue Tasks.

   [Daily Note Recurring Tasks](https://github.com/nfuchs-DSC/Obsidian-for-Researchers/blob/7495e7b4582fdaf896b12761988c5e9b1421e2de/Materials-for-the-Exercises/Templates/Template_Daily_Note_with_Recurring_Tasks.md)<br>
	→ This template includes sections for: Daily Thoughts, New Tasks, Tasks Due Today, Upcoming Tasks, Completed Tasks, Overdue Tasks, **and Recurring Tasks**.
   
   [Daily Note with Scheduled Today](https://github.com/nfuchs-DSC/Obsidian-for-Researchers/blob/7495e7b4582fdaf896b12761988c5e9b1421e2de/Materials-for-the-Exercises/Templates/Template_Daily_Note_with_Scheduled_Today.md)<br>
   	→ This template includes sections for: Daily Thoughts, New Tasks, Tasks Due Today, **Tasks Scheduled for Today**, Upcoming Tasks, Completed Tasks, and Overdue Tasks.
   
   [Daily Note with Recurring Tasks und Scheduled Today](https://github.com/nfuchs-DSC/Obsidian-for-Researchers/blob/7495e7b4582fdaf896b12761988c5e9b1421e2de/Materials-for-the-Exercises/Templates/Daily_Note_with_Recurring_Scheduled_Tasks.md)<br>
   	→ This template includes sections for: Daily Thoughts, New Tasks, Tasks Due Today, **Tasks Scheduled for Today**, Upcoming Tasks, Completed Tasks, Overdue Tasks, **and Recurring Tasks**.
   
   
**OR**

6. **Download the template you want and drag and drop it to your vault.**
7. **Move the template into the "TEMPLATES" folder.**

*Once you are familiar with the template you can delete the instructions within the template. These are your for a first understanding and guidance.*

### Understand the Error Messages in the Template
The message you are seeing (see screenshot below) indicates that the template placeholders (e.g., `<% today %>`) are not being expanded when viewed directly in the template file. This is normal behavior because the placeholders are intended to be replaced when the template is used, not when the template is viewed directly.

![4_error_message_template_daily_note](https://github.com/user-attachments/assets/fd47a260-1310-4a38-894b-db0ce37d464f)


## 4. Settings in the Community and Core Plugins

*To make sure everything works properly, you need to adjust a few settings in the community plugins.*

1. **Settings** → **Templater** → set **Template folder location** to "BACKEND/TEMPLATES" → and turn on **Trigger Templater on new file creation**
2. **Settings** → **Dataview** → enable **Enable JavaScript queries** and **Enable inline JavaScript queries**
3. **Settings** → go to **Daily notes** → set **New file location** to "BACKEND/DAILY NOTES" → set **Template file location** to "BACKEND/TEMPLATES/Template_Daily_Note" (*This is the path to the template you just created in the step before.)*

## 5. Check if everything is working
*Now you finished all settings for your daily workflow. Check if everythings works quite well.* 
1. Go to your vault and click on the left sidebar on the calendar icon ("Open today's daily note").
2. Then a note with the template should open with the today's date.
3. The note sould be stored in BACKEND/DAILY NOTES.

*In the next exercise there are some tips how you can use the daily note in your workflow.*

## 6. Change Log
Insert the following text into your note "CHANGELOG" and enter today's date. Add everything else you changed in the settings.
```markdown
**dd/mm/yyyy**
Installed community plugins Templater, Dataview and Task.
	Templater: Set folder locations.
	Dataview: Enabled JavaScript queries and inline JavaScript queries.
These plugins are used for the daily note.
New Template for daily note.
```

## 7. Customization (optional)
###### Tasks Plugin: Global task filter
*With the current settings every task in your vault which is marked as a task (- [ ]) and has a date is shown in your daily note. You can change this with the global filter within the task plugin. There you can choose a sign or text and filter the tasks. E.g if you set there a "+" as filter just the tasks with a date and the sign "+" will be displayed in the daily note (you can choose any sign you want). You can adjust this in the settings for the task plugin.*
###### Open daily note on startup
1. **Settings** → **Core Plugin: Daily Note** → Enable "Open daily note on startup"

## 8. Tip
There are documentations available for the *Community Plugins* and pre-installed *Core Plugins*. On these pages, you'll find all the features that come with each plugin. To reduce complexity, this guide only describes a small portion of the possibilities you have with the plugins. However, if you want to know more or have specific questions, you can read the documentations.

[Daily notes - Obsidian Help](https://help.obsidian.md/plugins/daily-notes)

[Tasks by Clare Macrae and Ilyas Landikov](https://publish.obsidian.md/tasks/Introduction)

[Templater by SilentVoid](https://silentvoid13.github.io/Templater/introduction.html)

[Dataview by Michael Brenan](https://blacksmithgu.github.io/obsidian-dataview/)
