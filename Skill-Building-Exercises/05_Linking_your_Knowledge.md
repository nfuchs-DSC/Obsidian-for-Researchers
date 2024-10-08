## Linking your Knowledge
*(Duration approx. 30min)*

*One of the most powerful features of Obsidian is the ability to link your notes. Obsidian allows users to create bi-directional links between notes, enabling a web of interconnected ideas. This feature facilitates easy navigation and retrieval of related information, making it ideal for building a personal knowledge base.*

### Linking to other notes
*I believe it is important for the note-taking system to be as interoperable as possible. If you ever stop using Obsidian, you can use the .txt files in another app. If the new app also uses Markdown syntax, then your links will not be lost. However, you need to disable the Wikilink format for internal links and set it to Markdown format.*

**Settings** → **Files and links** → disable **Use [[Wikilinks]]** → enable **Automatically update internal links** *(It has nothing to do with interoperability, but since we are already here, we can do that as well.)*

![Interoperability](https://github.com/user-attachments/assets/d98f61f6-54db-4a01-a764-bddacbdba7e2)



#### Exercise: Linking to other notes
The following exercise is an example that demonstrates how you can use the internal linking function.
1. You found an important research article about cats, dogs and object recognition models in your previous exercise. It's now afternoon and you have time to read research articles. You should add a note to the task you created earlier called "Check literature..." to remind yourself to read this specific article. Write behind the task:
```markdown 
[[Object Category Recognition]]
```
  *A link titled "Object Category Recognition" should now appear. You'll notice that its color is lighter compared to the other links. This is because the note for this header hasn't been created yet.*

2. **Click on the link**, and a new tab will open where Obsidian will automatically generate the note.
3. **Expand the right sidebar** → **click on backlinks** *Here, you can view all the backlinks to your note. Currently, you will see the mention in your daily note.*
4. You have read the article and found some really interesting facts which might be useful for your publication. Copy the following in the note:
```markdown
Pets in Clothes: The research team found that one of the common issues with the images collected for their dataset was pets wearing clothes. The article mentions that images of pets dressed up were often discarded, which implies that while some owners may enjoy dressing their pets, it complicates the task of accurately identifying their breed. Source: [Cats and dogs | IEEE Conference Publication](https://ieeexplore.ieee.org/abstract/document/6248092) [[Ideas Collection Publication 3]]
```
6. **Create the note** "Ideas Collection Publication 3" by clicking the link.
7. Again: **Expand the right sidebar** → **click on backlinks** *Now you can see all the places where you had ideas for your publication.*



