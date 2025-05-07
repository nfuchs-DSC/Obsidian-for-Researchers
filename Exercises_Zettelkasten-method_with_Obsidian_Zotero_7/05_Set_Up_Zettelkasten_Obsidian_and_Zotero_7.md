
*This manual is written for **Zotero 7.0***

*The following plugins are used:*
- *Zotero: Better BibTex*
- *Obsidian: Zotero Integration*

*Following workflow is possible with this set up:*
- *Read and annotate your texts in Zotero.*
- *Import tags, bibliographic data, abstract, link to the Zotero file, annotations and comments in the annotations in Obsidian.*
- *Set up for Zettelkasten-Method (Niklas Luhmann)*

*The naming convention is based on the exercises 1-4 in this GitHub Repo and also the settings in this exercises might be important for this exercise. Feel free to adapt this to your needs.*

## Step 1: Settings in Zotero

*With the Zotero plugin Better BibTex you can manage your bibliographic data more easily if you use a Markdown editor. The plugin automatically generates a citation key that follows a form you have selected. In Obsidian our literature note will automatically named with this citation key.*

1. **Download the .xpi file from the GitHub repository** [Better BibTeX for Zotero](https://github.com/retorquere/zotero-better-bibtex/releases/tag/v7.0.17)

	[Click here for the documentation of Better BibTex](https://retorque.re/zotero-better-bibtex/index.html)

2. Install Better BibTex:
**Tools → Plugins → Settings → Install Plugin from file → select .xpi file → click open → restart zotero**

3. Customize Better BibTex:
**Edit → Settings → Better BibTex → Citation key → insert:**
	
	```
	"z." + authEtal2(creator = "*", initials = false, sep = ".").fold + year
	```
	**Output:** z.Author.etal.year
	
	*I use the prefix “z.” so that I can easily distinguish between source notes from Zotero and source notes that I have only created in Obsidian.*
	
	*Please visit the plugin documentation if you would like to create a different cite key.*

4. **Display citation key in Zotero's Literatur List:**
**Right-click on bar "Titel | Creator | Attachment" → select citation key** <br>
	*Now you can see the citation key for each of your reference.*

5. **Document all settings in your CHANGELOG**

## Step 2: Settings in Obsidian

1. **Create a folder** named "ZEKA" → **Create inside the folder "ZEKA" the folders** "SOURCE_NOTES" and "ZETTEL"
2. **Community plugins → Browse → Zotero Integration by mgmeyers → Install → Enable**
3. **Open Zotero Integration Settings → Enable "Open the created note after import"**
4. **Open Zotero Integration Settings → set the "Note Import Location" to "ZEKA/SOURCE_NOTES"**

*This part is important for the Zettelkasten (see next exercise):*



4. **Document all settings in your CHANGELOG**

## Step 3: Set Up Templates for Zettel and Source Notes

**Source Note Template:**

1. *In Obsidian:* <br>
	**Add in Folder BACKEND/TEMPLATES** new note "Zotero_Template" and copy the following template in it (or use/build your own):

```
---
tags: {% if allTags %}{{allTags}}{% endif %}
created: {{importDate|format("YYYY-MM-DD")}}
---


### Titel: {{title}}

**Authors:** {{authors}}

**Reference:** {{bibliography}}
**Zotero Link:** {{pdfZoteroLink}}

> [!NOTE]- Abstract
> {{abstractNote}}


{% for annotation in annotations -%} 
{%- if annotation.annotatedText -%}*{{annotation.annotatedText}}*([p.{{annotation.pageLabel}}](zotero://open-pdf/library/items/{{annotation.attachment.itemKey}}?page={{annotation.pageLabel}}&annotation={{annotation.id}}))
{% endif %}{% if annotation.imageRelativePath %}![[{{annotation.imageRelativePath}}]]{% endif %}
{% if annotation.comment %}{{annotation.comment}}{%- endif %} 
{% if annotation.hashTags %}{{annotation.hashTags}}{%- endif %} 

{% endfor %}
```

**The template generates this output:**
![7_screenshot_zotero_template](https://github.com/user-attachments/assets/2cfabc3e-0f57-4626-8091-70c1d1e7a70e)


2. **Document all settings in your CHANGELOG**


**Zettel Template:**

1. *In Obsidian:*<br>
	**Add in Folder BACKEND/TEMPLATES** new note "Zettel_Template" and copy the following template in it (or use/build your own):

```
---
Created: <% tp.file.creation_date() %>
tags:
---
### Input

### Reference

### Output

### Link

```

## Step 4: Settings in Obsidian and Zotero for Literature Import

*Synchronize the citation format*

1. *Zotero:* <br>
	**Edit → Settings → Cite → Select your Citation Format and remember it (e.g. American Political Science Association)**

2. *Obsidian:* <br>
	**Settings → Zotero Integration → Citation Format → Add Citation Format → Select the same as in Zotero**

	**Import Formats → Add Import Format** <br>
		**Name:** Add Source Notes <br>
		**Output Path:** ZEKA/SOURCE_NOTES/{{citekey}}.md <br>
		**Image Output Path:** BACKEND/ATTACHMENT/{{citekey}}/ <br>
		**Template File:** BACKEND/TEMPLATES/Zotero_Template.md <br>
		**Bibliography Style:** Select the same citation format like before <br>

3. **Document all settings in your CHANGELOG**


