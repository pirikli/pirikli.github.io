---
title: How discovering Markdown Transformed My Learning and Note-taking Journey
description: Why I Chose Markdown Over Other Note-Taking Methods?
date: 2024-01-28 08:30:00 +0330
last_modified_at: 2025-02-28 14:00:00 +0000
author: Aboutaleb Nasiri Parouch
layout: post
categories:
  - Note-taking
  - Markdown
  - learning
tags:
  - markdown
  - markup-language
  - writing
comments: true
published: true
permalink: /how-markdown-transformed-my-learning/
toc: true
image: /assets/images/posts/markit/down.jpg
---
![D](https://cdn-icons-png.flaticon.com/128/3570/3570060.png){: w="80" h="auto" .left}uring my **🅿️**ython learning journey, I initially used __Microsoft Word__ for note-taking, but I found it time-consuming and ineffective.

__[Notion](https://www.notion.so/)__{:target="_blank"} seemed promising with its creativity, innovation, and **AI** tools, but I realized I was spending more time on templates and design than on learning **<span style="color: green;">Python</span> 🐍.**

  

![W](https://cdn-icons-png.flaticon.com/128/8112/8112804.png){: w="80" h="auto" .left}hile everyone emphasized the importance of note-taking, my existing methods were wasting precious time. I would watch tutorials, <mark>take notes, and never revisit them</mark>❗Feeling stuck, I shifted to solely watching tutorials, until I encountered a breakthrough.

![R](https://cdn-icons-png.flaticon.com/128/13527/13527880.png){: w="80" h="auto" .left}ecently, during my Git learning on [DataCamp](https://datacamp.com){:target="_blank"}, I faced a dilemma – I wasn't taking notes. <ins>The **README.md** file in my Git repository caught my attention</ins>. __An idea struck:__  *use GitHub as a notebook and Markdown as the note-taking tool.* And so, my first note,**"Introduction to Git"**, was born, accessible HERE.

  
  

![M](https://cdn-icons-png.flaticon.com/128/3570/3570071.png){: w="80" h="auto" .left} [**ARKDOWN⬇️**](https://www.markdowntutorial.com/ "Markdown turorial"){:target="_blank"}has empowered me to create organized notes and actively learn Git. Now, I'm immersed in the practical application of Markdown, <span  style="color:#6495ED;">simultaneously learning and documenting my progress...</span>

  
  

**🚶🏼<span  style="color:#7D6608;">Let's start the journey</span>🧳**

## What is [Markdown](https://daringfireball.net/projects/markdown/){:target="blank"}?

Ⓜ️🅰️RKD🅾️WN is a _sweet_ and _suitable_ way to write content for the web🕸️.   
It is a 🪶lightweight markup language with plain-text formatting syntax.   
It uses symbols like `#`, `*`, `_`, `>`, and `!` to format text, create headings, lists, paragraphs, and more.   
Markdown is ideal for web content, documentation, and note-taking due to its simplicity and readability.

**Table of _Contents:_** {#top}

| [**1. Headers**](#head1)                 | [**9. 📃Lists**](#head9)                 |
| ---------------------------------------- | ---------------------------------------- |
| [**2.Text Formatting**](#head2)<br>      | [**10. Scaping Characters**](#head10)    |
| [**3.Paragraphs & Line Breaks**](#head3) | [**11. Tables**](#head11)                |
| [**4. Blockquote**](#head4)              | [**12. Heading IDs**](#head12)           |
| [**5. Horizontal Lines**](#head5)        | [**13. Footnote**](#head13)              |
| [**6. Code Blocks**](#head6)             | [**14. Best Markdown Editors**](#head14) |
| [**7. 🔗Links**](#head7)                 | [**15. Conclusion**](#head15)            |
| [**8. 🖼️Images**](#head8)               |                                          |


## Ⓜ️arkdown ©️heat Sheet
💡Before starting, open a [**Markdown Editor**](https://stackedit.io/app#); copy or write each syntax there to see the magic 🪄

### 1. <img  src="https://cdn-icons-png.flaticon.com/128/4019/4019787.png"  alt="image"  width="30"  height="auto">eaders {#head1}

```md
	# First Level Header
	## Second Level Header
	### Third Level Header
	#### Fourth Level Header
	##### Fifth Level Header
	###### Sixth Level Header
```

🟰➖Alternate Syntax for **H1** & **H2:**

```md
	First Level Header
	==================

	Second Level Header
	-------------------
```

_**<span style="color:green">Tip:</span>**_
> 
 >- Put blank lines before and after a heading.
>- Add a space between `#` and the heading text.
>- Use headings for hierarchy, not just for styling.



### 2. Text formatting {#head2}

| Format              | Syntax                       | Output                 |
| ------------------- | ---------------------------- | ---------------------- |
| **Bold**            | `**text**` or `__text__`     | **Bold Text**          |
| _Italic_            | `*text*` or `_text_`         | _Italic Text_          |
| _**Bold & Italic**_ | `***text***` or `___text___` | _**Bold and Italic**_  |
| ~~Strikethrough~~   | `~~text~~`                   | ~~Strikethrough~~      |
| Highlighted         | `==Highlight==`              | ==Highlight==          |
| Subscript           | `<sub>text</sub>`            | Sub<sub>script</sub>   |
| Superscript         | `<sup>text</sup>`            | Super<sup>script</sup> |



### 3. <img  src="https://cdn-icons-png.flaticon.com/128/5771/5771269.png"  alt="paragraph"  width="50"  height="autho">Paragraphs & Line Breaks {#head3} 

Use 2️⃣`SPACE`s(☄️☄️) at the end of a line to insert a line break.
Press `ENTER` to start a new paragraph.

```md
This is the first line.☄️☄️ 
This is the second line.☄️☄️

This is a new paragraph.☄️☄️
```

### 4. <img  src="https://cdn-icons-png.flaticon.com/128/852/852907.png"  alt="blocs"  width="50"  height="auto">Blockquote {#head4}

#### ❇️Blockquotes are created using the `>` symbol.

```md
> This is a blockquote.
>
> - You can include multiple lines.
> - Even lists inside!
```

#### ❇️Nested Blockquotes:
```md
> This is an outer blockquote.
>> This is an inner blockquote.
>>> You can go deeper.
```

### 5.Horizontal Lines {#head5}

**Use 3️⃣three or more asterisks `(***)`, dashes`(---)`, or underscores`(___)`:** 

```md
***
---
___
```



### 6.Code Blocks {#head6}

#### 💠Inline code
✅To make codes  visible as they are, we wrap the them in 2️⃣ backticks `` `<br> ` ``

#### 💠Code Blocks

✅To create Code Blocks, use 3️⃣ backticks(```) or tilde(~~~)before and after the code snippet, and provide the language name after initial backtics, in order to _Highlight the code syntax_.

```
   ```html
     Code Block goes here...
     ```
```


### 7.🔗Links: {#head7}
#### 🖇️Inline link:
```md
[MY GitHub](https://github.com "GitHub Homepage")
```
[**My GitHub_](https://github.com/pirikli "Pirikli, a Poet and Programming Pilgrim")

#### 🖇️Reference link:
```md
[My Linkedin] [ refrence-to-link ]

[ refrence-to-link ]: https://www.linkedin.com/in/pirikli/ "Pirikli"
```
➡️[**_My LinkedIn_**][refrence-to-link]

[refrence-to-link]: https://www.linkedin.com/in/pirikli/ "Pirikli"

#### 🖇️Direct Link:
```md
<pirikliartan@gmail.com>{:target="_blank"}
```
➡️ <pirikliartan@gmail.com>{:target="_blank"}
  
**💡Tip**: We add the`{:target="_blank"}`immediately after the link, in order to open the link in new tab.

### 8. 🖼️Images: {#head8}

#### 📷Inline Image:
```md
![Alt text](image-url.jpg "Image Title")
```
![HTML Icon](https://cdn-icons-png.flaticon.com/128/7404/7404512.png "اچ‌تی‌ام‌ال")

#### 📷Reference Image:
```md
![Alt text][image]
    
[image]: image-url.jpg "Image Title"
```



### 9. 📃Lists {#head9}

#### 🔢Ordered list

```md
1. This is the first item of this ordered list.
2. This is the second item.
3. The third item.
```

#### ⏹️Unordered list:

```md
* This is the first item of this unordered list.  
* This is the second one.
* and son on...
```


#### 🪺Nested lists(indentation in lists):
✅Use `TAB` to indent nested lists
```
1. The first item with inner list:
    - first inner
    - second inner
2. The second item with nested list
    * first inner
    * second inner
        - one
        - two
            * A
            * B
```

#### Task Lists:  

```md
- [ ] Wake Up
- [ ] Get Up
- [ ] Wash Up
- [ ] Rush Up
```
  


### 10. Scaping Characters:  {#head10}
To display Markdown symbols as plain text, use a backslash (`\`).

```markdown
\*This text is not italicized\*
```
[**Here**](https://www.markdownguide.org/basic-syntax/#characters-you-can-escape) is the list of other characters to scape.    
 
   

### 11. <img  src="https://cdn-icons-png.flaticon.com/128/4598/4598376.png"  alt="paragraph"  width="50"  height="autho">Tables {#head11}

```md
| Column 1 | Column 2 | Column 3 |
|----------|----------|----------|
| Data 1   | Data 2   | Data 3   |
| Data 4   | Data 5   | Data 6   |
```


### 12. Heading IDs {#head12}

 I think of it as "Inner Link" or "IN Page Link".  
 I usually use it to create "Content Table" and "🦘Jump Up High".   
  
```md
[Here is the Link to that Heading](#headid5)   

      
##### This is a heading we want to refer or link to {#headid5}
```
 

### 13. Footnotes {#head13}
```md
This is a sentence with a footnote.[^1]

[^1]: This is the footnote text.
```

### 14. Best Markdown Editors: Why **Obsidian** Stands Out {#head14}

Markdown editors enhance note-taking, documentation, and web writing by providing a distraction-free environment with instant formatting. Here are some top choices:

✅ **Obsidian** – A powerful, local-first Markdown editor with backlinks, graph views, and plugins for knowledge management. Ideal for writers, researchers, and programmers.  
✅ **VS Code** – A robust code editor with Markdown preview and extensions.  
✅ **Typora** – A clean, minimalist editor with real-time rendering.  
✅ **StackEdit** – A browser-based Markdown editor with cloud sync.

🔹 **Why Choose Obsidian?**  
Obsidian isn't just a Markdown editor—it’s a **second brain** for creatives. With its **bi-directional linking, tags, and plugins**, it transforms raw notes into a structured knowledge hub.

[➡️ Download Obsidian](https://obsidian.md/) 🚀

### 15. Conclusion {#head15}

Switching to Markdown has revolutionized my learning experience. It allows me to take structured notes, integrate them with GitHub, and focus on learning instead of formatting. Whether you’re documenting your programming journey or writing blog posts, Markdown is a game-changer!

🔗 **Start your [Markdown](https://www.markdownguide.org/) journey today!**   
**➕Share your experience below in comments:**   
➖Which Markdown Editor do you use and why?   
➖Do you prefer other writing tools over Markdown? why?      
➖🟣🟣🟣   

[**<span style="background-color: black; color: orange; border-radius: 25px;">🦘Jump Up High</span>**](#top)

{% raw %}{% include disqus_comments.html %}{% endraw %}
