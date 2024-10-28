## Linking your Knowledge
*(Duration approx. 30min)*

*One of the most powerful features of Obsidian is the ability to link your notes. Obsidian allows users to create bi-directional links between notes, enabling a web of interconnected ideas. This feature facilitates easy navigation and retrieval of related information, making it ideal for building a personal knowledge base.*

### Linking to other notes
*I believe it is important for the note-taking system to be as interoperable as possible. If you ever stop using Obsidian, you can use the .txt files in another app. If the new app also uses Markdown syntax, then your links will not be lost. However, you need to disable the Wikilink format for internal links and set it to Markdown format.*

**Settings** → **Files and links** → disable **Use [[Wikilinks]]** → enable **Automatically update internal links** *(It has nothing to do with interoperability, but since we are already here, we can do that as well.)*

<img src="https://github.com/user-attachments/assets/8346e5ae-310c-4c26-934a-128b97c17b2c" height="300" alt="screenshoot_settings_interoperability">

#### Exercise: Linking to other notes
The following exercise is an example that demonstrates how you can use the internal linking function.
1. You found an important research article about cats, dogs and object recognition models in your previous exercise. It's now afternoon and you have time to read the articles. Write behind the task "- [ ] Check literatur [...]":
```markdown 
[[Object Category Recognition]]
```
  *A link titled "Object Category Recognition" should now appear. You'll notice that its color is lighter compared to the other links. This is because the note for this header hasn't been created yet.*

2. **Click on the link**, and a new tab will open where Obsidian will automatically generate the note.
3. **Expand the right sidebar** → **click on backlinks** *Here, you can view all the backlinks to your note. Currently, you will see the mention in your daily note.*

<img src="https://github.com/user-attachments/assets/9f9e9363-0d2b-483b-b251-e8875a8ece53" height="270" alt="image">


5. You have read the article and found some really interesting facts which might be useful for your publication. Copy the following in the note:
```markdown
Pets in Clothes: The research team found that one of the common issues with the images collected for their dataset was pets wearing clothes. The article mentions that images of pets dressed up were often discarded, which implies that while some owners may enjoy dressing their pets, it complicates the task of accurately identifying their breed. Source: [Cats and dogs | IEEE Conference Publication](https://ieeexplore.ieee.org/abstract/document/6248092) [[Ideas Collection Publication]]
```
6. **Go to the note** "Ideas Collection Publication 3" by clicking the link.
7. Again: **Expand the right sidebar** → **click on backlinks** *Now you can see all the places where you had ideas for your publication.*

### Graph View
*The graph view is a great tool for getting an overview of your linked notes. You can visualize your knowledge with just one click.*

**Left sidebar** → **Click on graph view icon**

<img src="https://github.com/user-attachments/assets/b8e94764-09e7-41ed-82c8-f8b3b56b8ce9" height="200" alt="sidebar_graphview">



### Linking a local file
*It is also possible to write a link in a note in Obsidian that allows you to open a file from your computer. You need to insert the path to the file into the following link. You can find the path by right-clicking on the file and selecting "Copy Path".*

```markdown
[filename](file:///<absolute-path>)
```
### Using Tags
To link your knowledge quickly and easily, you can use tags. To do this, write '#word' in a note. When you click on the tag, all the notes in which you have used the tag will be displayed in the sidebar. 
 - This might be useful if you have fixed topics that recur often in different notes and should be connected with each other. For example, if you are learning a new language, you can use it to tag new words that appear in various notes. You can easily write in your daily note without having to search for the right place for the vocabulary.
 - It is not useful to interconnect all of your thoughts. The number of tags would become too large, and after a while, you would forget which tags you've used.
 - However, with the Dataview plugin, which you installed in [03_Create_your_Daily_Workflow](https://github.com/nfuchs-DSC/Obsidian-for-Researchers/blob/main/Skill-Building-Exercises/03_Create_your_Daily_Workflow.md), you can display tags in a note. This feature is helpful for getting a better overview of your content.
