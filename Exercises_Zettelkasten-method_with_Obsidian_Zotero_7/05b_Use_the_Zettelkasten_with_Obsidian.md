
**Learning Objectives in this Exercise:**

- Create and Link "Zettel" in Obsidian
- Using the Zettel Template, includes explanation of the template

## Step 1: Your first "Zettel": Lunch with Colleagues

*After lunch your back in your office. At lunch colleague told you about his cat and suddenly you got an idea for your article.*

1. **Create a note in the folder ZEKA/ZETTEL** → **press alt + e** (on Windows; or open command palette with `Ctrl+P` and type `Templater: Open insert template modal`) → **select** "Zettel_Template" → name the "Zettel" "cats_in_space"  

**Note:** In most cases, the Windows hotkeys cannot be used for MacOS. You can set these up manually: Settings → Hotkeys → search for “Insert Template” → press alt + e (or Option + e on Mac)

*Now you see the Zettel Template in your note and you can fill it like this:*

```
---
Created: 2025-04-09 18:41
tags: p1/lit_review

---
### Input
Colleagues story about his cat. 
### Reference
My idea based on his story.
### Output
Idea for introduction: Cats in space are funny.
### Link
[[Link_to_related_Zettel]]
```

**Tip:** To change between preview mode and source mode press **strg + p**  → "Toggle Live Preview/Source mode"

*It should look like this:* <br>
![8_screenshot_zettel_template](https://github.com/user-attachments/assets/576e9902-ad45-4d90-b190-7c572018d59c)


**Explanation of the Zettel structure**
*This is a structure of a Zettel I like. It is not the way Luhmann did it. He had less structure in his notes, which is perfectly fine. Please choose the way it suits for you.*

1: *The name of the file is important because you connect the Zettel with each other. Choose a name which reflect the overall topic of the note.*

2: *I use the [Properties](https://help.obsidian.md/properties) for the tags. With the Dataview plugin (you already installed it in the previous exercises) it is possible to query your database via tags (see exercise 05d). I use my tags to sort the Zettel into my projects.*

3: *In the input section I add the quote, situation, picture, thought etc. on which my insight was based.*

4: *Here, I add the source or reference of the input. It can be a bibliography reference, or a link to a website, or yourself.*

5: *Here, I add what output I have based on the input. It is one of the most important section for your Zettelkasten. Based on what is written here you can write paper easily by copy and paste your written text. In this section you have to think about your topic/insight which is the most important difference between an archive (where you store data) and your Zettelkasten (where you think).*

6: *In this section you link your "Zettel" to another "Zettel". Make sure that the "Zettel" is connected to your knowledge base. Otherwise you will lose the "Zettel" between the others. Choose one or two links which relates to the topic of your note. Don't use more links, it will clutter your Graphview (see exercise 05d). By typing `[[]]` into the note, you can search through your notes to find a fitting one. For demonstration purposes, I’ve added a placeholder here.* 

## Step 2: Your second "Zettel": An Idea Based on the First "Zettel"

*While creating your first "Zettel" an idea comes into your mind: You want to generate a picture for your publication. With the help of AI you generate a picture with cats in space and connect it to your first "Zettel".*

1. **Generate a picture with the help of AI or download one from this GitHub Repo** → "Materials-for-the-Exercises" → "For_Exercise_05b_ChatGPT Image 9. Apr. 2025, 19_24_48.png"

2. **Change the link in your first "Zettel"** (Link_to_related_Zettel) into "picture_cats_in_space" → **create a new note** by clicking on the link → **press alt + e** → **select** "Zettel_Template"

*Now you see the Zettel Template in your note and you can fill it like this:*

```
---
Created: 2025-04-10 10:51
tags: p1/lit_review

---
### Input
Prompt: Cats in space are funny.
### Reference
ChatGPT Image 9. Apr. 2025, 19_24_48
### Output

### Link

```

*Use drag-and-drop to insert the cat image from your local device under the “Output” header.*

*It should look like this:* <br>
![9_screenshot_zettel_cats_in_space](https://github.com/user-attachments/assets/74a12a9e-deb7-4c6c-af52-b9cea2e2eee5)


*I did not fill in the section "Link", because the "Zettel" is already linked to a "Zettel" via the backlink function.*

**Important: Move both Zettel into the "ZETTEL" folder.**
**Tip: Enable Backlink View:**

*I recommend to enable the feature so you can see the backlinks of your notes permanently in your note.*

3. **Settings** → **Core Plugin** → **Backlinks** → **Enable** "Show Backlinks at the bottom of your notes"

4. To activate it, **close and reopen the note.** You can now collapse the right sidebar, as the backlinks are no longer needed here.

