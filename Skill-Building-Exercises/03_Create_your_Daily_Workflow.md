# Your Daily Workflow
*(Duration approx. 15min)*

*The "Daily Note" is your hub where everything that happens in your day will be in one place and connected to your whole knowledge base. Here you can take notes, add new To-Dos, and automatically display To-Dos that you want or need to complete today. There are many ways to design the Daily Note. For guidance, I have created a minimalist template that primarily organizes To-Dos and can interconnect your knowledge. With a bit of programming experience or patience, you can customize the template to your liking.*

*You can access the Daily Note either by clicking on the calendar button in the left taskbar, or you can set it up in the settings so that the Daily Note automatically opens when you open your Obsidian vault.*

*For our daily workflow, we need to add a few functions to our Obsidian Vault. We do this with plugins created by the Obsidian Community: The so-called community plugins.*

## Communitiy Plugin
*Community plugins in Obsidian are user-created extensions that enhance the functionality of the app beyond its core features. These plugins are developed by members of the Obsidian community, allowing users to customize and expand their note-taking experience to suit individual needs and workflows.*

<details>
<summary>Potential Risks of Community Plugins</summary>
<br>
While community plugins offer great flexibility and power, they can also pose potential risks:

1. **Security concerns**: Since these plugins are not officially vetted by Obsidian, they could potentially contain malicious code.
   
2. **Stability issues**: Community plugins may introduce bugs or conflicts that could affect the performance of Obsidian.
   
3. **Maintenance uncertainty**: There's no guarantee that a plugin will be maintained long-term, which could lead to compatibility issues in the future.
<br>
</details>

<details>
<summary>How to Check whether a Plugin is Dangerous</summary>
<br>
To assess the safety and reliability of a community plugin, consider the following steps:

1. **Check update frequency**: Look at when the plugin was last updated. Regularly maintained plugins are generally more reliable.
   
2. **Review download count**: A higher number of downloads often indicates a more trusted and widely-used plugin.
   
3. **Examine the GitHub repository**: Visit the plugin's GitHub page to review the code, issues, and overall project activity.
   
4. **Read user reviews**: Look for feedback from other users in the Obsidian community forums or Discord.
   
5. **Start with essential plugins**: Begin with well-established, popular plugins that are more likely to be secure and maintained.

Remember, Obsidian keeps community plugins disabled by default ("restricted mode"). You must manually enable them, which serves as a built-in safety measure.
<br>
</details>

## Install Community Plugins for your Daily Workflow

1. Enable the community plugins: **Settings** → Click **Turn on community plugins**
2. Click **Browse** → search for the plugin **"Dataview by Michael Brenan"** → install the plugin
3. Enable the dataview plugin: go back to **settings** menu item **community plugin** → activate it by clicking on the slider in the line of the newly installed plugin
4. Repeate this for the community plugins **"Tasks by Clare Macrae and Ilyas Landikov"** and **"Templater by SilentVoid"**

## Create folder and notes for your Daily Workflow

*Of course, you can also use other names and terms for the folders and notes. The important thing is that you don't change the names anymore.*

1. Create a folder "DAILY NOTES".
2. Create a folder "TEMPLATE".
3. Create a note "Template_Daily_Note" and drag and drop it into the TEMPLATE folder.
4. Copy and paste the following in the "Template_Daily_Note". It saves automaticaly.

         #### Date: <% tp.date.now("dddd Do MMMM YYYY") %>
         
         
         # Daily Log
         
         *Documentation of Activities, focus for today, accomplishments or important insights etc.*
         
         # Tasks
         
         #### New
         *Note here the tasks which will meet you on this day and tag it with a date*
         
         #### Done Today
         *Here will every tasks listed which are done today.*
         ```tasks
         # done today, from filename
         done on <% tp.date.now("YYYY-MM-DD", 0, tp.file.title, "YYYY MM DD") %>
         ```
         
         #### Due Today 
         *The due date is the specific date by which a task must be completed. It signifies a deadline for the task.* 
         ```tasks
         not done
         is not recurring
         # due today, from filename
         due on <% tp.date.now("YYYY-MM-DD", 0, tp.file.title, "YYYY MM DD") %>
         hide due date
         ```
         
         #### Scheduled Today
         *The schedule date refers to when a task is planned to be worked on or started. This date does not necessarily indicate a deadline but rather a target date for when the task should be tackled.* 
         ```tasks
         not done
         is not recurring
         # scheduled today, from filename
         scheduled on <% tp.date.now("YYYY-MM-DD", 0, tp.file.title, "YYYY MM DD") %>
         hide scheduled date
         ```
         
         #### Recurring today
         *A recurring task is a task that is automatically generated to repeat at regular intervals, such as daily, weekly, monthly, or yearly.* 
         ```tasks
         not done
         is recurring
         # happens today, from filename
         happens on <% tp.date.now("YYYY-MM-DD", 0, tp.file.title, "YYYY MM DD") %>
         ```
         
         #### Overdue tasks
         *Tasks that have a due date in the past but are still incomplete could be considered overdue. This term emphasizes that the task should have been completed by the specified date.*
         
         ```tasks
         not done
         # happens before today, from filename
         happens before <% tp.date.now("YYYY-MM-DD", 0, tp.file.title, "YYYY MM DD") %>
         hide edit button
         ```
         
         #### Backlogged tasks
         *These tasks are waiting to be adressed, their important enough so you don't want to forget them. But not that time spcific, that you have to do it until a specific time. Here I am also collection ideas which are waiting for the right timing.*
         ```tasks
         not done
         no due date
         no scheduled date
         no start date
         ```
             
## Settings in the community plugins
   
1. **Settings** → **Templater** → set **Template folder location** to "TEMPLATES" → and turn on **Trigger Templater on new file creation**
3. **Settings** → **Dataview** → enable **Enable JavaScript queries** and **Enable inline JavaScript queries**
4. **Settings** → go to **Daily notes** → set **New file location** to "DAILY NOTE" → set **Template file location** to "TEMPLATES/Template_Daily Note" (*This is the path to the template you just created.*)

## Check that everything is working
*Now you finished all settings for your daily workflow. Check if everythings works quite well.* **Go to your vault and click on the left sidebar on the calendar icon (daily note). Then a note with the template should open with the today date.** *In the next manual there are some tips how you can use the daily note in your workflow.*

## Note
There are documentations available for the *Community Plugins* and pre-installed *Core Plugins*. On these pages, you'll find all the features that come with each plugin. To reduce complexity, this guide only describes a small portion of the possibilities you have with the plugins. However, if you want to know more or have specific questions, you can read the documentations.

[Tasks by Clare Macrae and Ilyas Landikov](https://publish.obsidian.md/tasks/Introduction)

[Templater by SilentVoid](https://silentvoid13.github.io/Templater/introduction.html)

[Dataview by Michael Brenan](https://blacksmithgu.github.io/obsidian-dataview/)
