---
title: Why I am learning Markdown?!
date: 2024-01-27 08:30:00 +0330
mermaid: true
toc: true
---
# <img  src="https://cdn-icons-png.flaticon.com/128/1570/1570738.png"  alt="discovery"  width="40"  height="auto"><span  style="color:green;">Discovering</span>[Markdown](https://daringfireball.net/projects/markdown/syntax)<img  src="https://www.markdownguide.org/assets/images/markdown-mark-white.svg"  alt="markdown"  width="35"  height="auto">{: .dark}<span  color="#85C1E9"> has transformed🚇</span><span  color="green">my note-taking📝 journey✈️</span>**

  
  

**<span  style="color:#3498DB"><img  src="https://cdn-icons-png.flaticon.com/128/8133/8133834.png" alt="H"  width="30"  height="auto"><sup>ere's why I chose to embrace it:</sup></span>**

  
  
  

![D](https://cdn-icons-png.flaticon.com/128/3570/3570060.png){: w="80" h="auto" .left}uring my **P**ython learning journey, I initially used __Microsoft Word__ for note-taking, but I found it time-consuming and ineffective.

__[Notion](https://www.notion.so/)__ seemed promising with its creativity, innovation, and **AI** tools, but I realized I was spending more time on templates and design than on learning **<font  color="green">Python</font> 🐍.**

  

![W](https://cdn-icons-png.flaticon.com/128/8112/8112804.png){: w="80" h="auto" .left}hile everyone emphasized the importance of note-taking, my existing methods were wasting precious time. I would watch tutorials, <mark>take notes, and never revisit them</mark>❗Feeling stuck, I shifted to solely watching tutorials, until I encountered a breakthrough.

![R](https://cdn-icons-png.flaticon.com/128/13527/13527880.png){: w="80" h="auto" .left}ecently, during my Git learning on [DataCamp](https://datacamp.com), I faced a dilemma – I wasn't taking notes. <ins>The **README.md** file in my Git repository caught my attention</ins>. __An idea struck:__  *use GitHub as a notebook and Markdown as the note-taking tool.* And so, my first note,**"Introduction to Git"**, was born, accessible HERE.

  
  

![M](https://cdn-icons-png.flaticon.com/128/3570/3570071.png){: w="80" h="auto" .left} arkdown has empowered me to create organized notes and actively learn Git. Now, I'm immersed in the practical application of Markdown, <span  style="color:#6495ED;">simultaneously learning and documenting my progress...</span>

  
  

**🚶🏼<span  style="color:#7D6608;">Let's start the journey</span>🧳**


Markdown is a _sweet_ and _suitable_ way to write content for the web.

It is plain text with simple syntax. it has some symbols(#, * _, >, !) to *control text's appearance and organize it*, such as making them **BOLD**, creating __**HEADER**s__, ordering them in lists, paragraphs...**



## <img  src="https://cdn-icons-png.flaticon.com/128/4019/4019787.png"  alt="image"  width="30"  height="auto">EADER and its 6 different level:

1️⃣ First Level Header  
> ✅**Symbol**(`#`)  
> ✅**Syntax**(`# First Level Header`)
>> ➡️Alternate Syntax(`===`)
```
First Level Header
===
```


2️⃣ Second Level Header    
> ✅**Symbol**(`##`)  
> ✅**Syntax**(`## Second Level Header`)
>> ➡️Alternate Syntax(`---`)
```
Second Level Header
---
```


3️⃣ Third Level Header   
>✅**Symbol**(`###`)  
>✅**Syntax**(`### Third Level Header`)


4️⃣ Fourth Level Header  
>✅**Symbol**(`####`)  
>✅**Syntax**(`#### Forth Level Header`)

  
5️⃣ Fifth Level Header  
>✅**Symbol**(`#####`)  
>✅**Syntax**(`##### Fifth Level Header`)


6️⃣ Fifth Level Header  
>✅**Symbol**(`######`)  
>✅**Syntax**(`###### Sixth Level Header`)  


**Tip**:  
- Put blank lines before and after a Heading.
- Put a space between the hashtag/pound sign(#️⃣) and the heading name.
{: .prompt-tip}
  
 


## Text Styles

**bold:**
>✅**Syntax**➡️(`** ** or __ __`)    
>✅**Example**➡️(`**This is bold** | __This also__`)      
>✅**Output**➡️(**This is bold** | __This also__)     


 _italic_:
>✅**Syntax**➡️(`* * or _ _`)     
>✅**Example**➡️(`*this is italic* | _this also_`)     
>✅**Output**➡️(*this is italic* | _this also_)   


**bold** and _italic_:
>✅**Syntax**➡️(`*** *** or ___ ___`)    
>✅**Example**➡️(`***This is bold and italic*** | ___This also___`)    
>✅**Output**➡️(***This is bold and italic*** | ___This also___)    


Bold and _nested italic_:
>✅**Syntax**➡️(`**_ _**`)  
>✅ **Example**➡️(`**This is _italic_ inside bold**`)   
>✅**Output**➡️(**This is _italic_ inside bold**)   


<sub>Subscript</sub>
>✅**Syntax**➡️(`<sub> </sub>`)    
>✅**Example**➡️(`This is a <sub>SubScript</sub> text`)    
>✅**Output**➡️(This is a <sub>SubScript</sub> text)    


<sup>Superscript</sup>
>✅**Syntax**➡️(`<sup> </sup>`)    
>✅**Example**➡️(`This is a <sup>SuperScript</sup> text`)    
>✅**Output**➡️(This is a <sup>SuperScript</sup> text)



## 3. 🔗Links:

  
### Inline link:

✅**Syntax**  
`[wrap the __link text__ in brackets]( wrap the __link__ in parentheses)`  

✅**Example**  
`[Pirikli's _GitHub_](https://github.com/pirikli)`  

✅**Output**➡️  
[**Pirikli**'s _GitHub_](https://github.com/pirikli)


### Reference link:

✅**Syntax** 
```
[link text][__refrence__ to another place inside doc]

[__refrence__ to another place inside doc]: **_link_**-to-outside-websites
```

✅**Example** 
```
[learn turki] [ refrence-to-link ]

[ refrence-to-link ]: https://mirze.ir
```

✅**Output**➡️  
[**_learn turki_**][refrence-to-link]

[refrence-to-link]: https://mirze.ir

  
  

## 4. 🖼️Images:


### Inline Image link:

✅**Syntax**  
```
❗[Alt text](online or local path to image)
```

✅**Example** 
```
![HTML Icon] (https://cdn-icons-png.flaticon.com/128/7404/7404512.png)
```


✅**Output**➡️

![HTML Icon](https://cdn-icons-png.flaticon.com/128/7404/7404512.png)


### Reference Images:

**Syntax**
```
![Alt text][Image tag]

[Image tag]: link-to-image </blockquote>
```

**Example**
```
![Pretty Python][ prepy ]

[ prepy ]: https://cdn-icons-png.flaticon.com/128/3098/3098090.png </blockquote>
```

**Outpute**


![Pretty Python][prepy]


[prepy]: https://cdn-icons-png.flaticon.com/128/3098/3098090.png



  
   




## 📃Lists

### Ordered list

✅**Syntax**:⬇️  
use numbers with dont (1. 2. 3.)

✅**Example**:⬇️
```
1. This is first item of ordered list
2. This is second item
3. Third item
```

✅**Output**⬇️
1. This is first item of ordered list
2. This is second item
3. Third item
4. 

### Unordered list:

✅**Syntax**:⬇️ 
use asterisk * or dash -


✅**Example**:⬇️
```
* This is first item of this unordered list.  
* This is second one
* and son on...
```

✅**Output**⬇️
* This is first item of this unordered list.  
* This is second one
* and son on...


### Nested lists(indentation in lists):
✅**Syntax**:⬇️
Use `TAB` to indent nested lists

✅**Example**:⬇️
```
1. first item with inner list
    - first inner
    - second inner
2. second item with nested list
    * first inner
    * second inner
        - one
        - two
            * A
            * B
```

✅**Output**⬇️
1. first item with inner list
    - first inner
    - second inner
2. second item with nested list
    * first inner
    * second inner
        - one
        - two
            * A
            * B
  


**Tip**:You can use other markdown syntax inside lists.  
Juat try it. Learn by doing.
{: .prompt-tip}   
  






## <img  src="https://cdn-icons-png.flaticon.com/128/5771/5771269.png"  alt="paragraph"  width="50"  height="autho">Paragraphs


✅**Syntax**  
> To break each line of a paragraph, use 2️⃣`SPACE`s☄️☄️.  
> To separate paragraphs with one or more _blank lines_🛣️, press `ENTER` 


✅**Example** 
> This is first line of first paragraph. ☄️☄️  
this is second line.☄️☄️   
🛣️🛣️🛣️🛣️🛣️🛣️🛣️🛣️  
thi is first line of second paragraph☄️☄️     
> and this is second line.☄️☄️   


>  ✍️Note:
* Keep lines left-aligned. 
* don't use `TAB` to indent paragraph. if you need, use  HTML entity for _non-breaking space_:
```  
   &nbsp;&nbsp;&nbsp;&nbsp;This is an indented Paragraph.   
```
* You can use HTML `<br>` element for line breaking.
{: .prompt-tip} 
  


## Tables





## 2. <img  src="https://cdn-icons-png.flaticon.com/128/852/852907.png"  alt="blocs"  width="50"  height="auto">Blockquote

### ❇️Turn a line or a paragraph to a blockquote.

✅**Syntax**⬇️  
Put a Greater than sign ( > ) at the begining.   

✅**Example**⬇️
``` 
> I am turning this paragraph to a blocquote with just one Greater than sign (>).   
be aware that the lines mustn't have blank lines in between.  
The lines must continuous not separated.
```
✅**Output**⬇️ 
> I am turning this paragraph to a blocquote with just one Greater than sign (>).   
be aware that the lines mustn't have blank lines in between.  
The lines must continuous not separated.



### ❇️Turn separated lines or more than one paragraph to blockquote.

✅**Syntax**:⬇️  
 Put a Greater than sign( > ) at the begining and between each line.

✅**Example**:⬇️
```
> This is the first line of the first paragraph.  
This is second line.
That's enough.
>
> This is Second paragraph.  
lets put them together in one Blocquote.  
```

✅**Output**⬇️
> This is the first line of the first paragraph.  
This is second line.
That's enough.
>
> This is Second paragraph.  
lets put them together in one Blocquote. 


### ❇️Indented or nested blockquotes.

✅**Syntax**:⬇️  
Use Double Greater than sign ( >> )

✅**Example**:⬇️
```
> This is outer blociquoe
>> This is inner blockquote:
> >> This line is the most inner one.
>> >> You can go deeper inside...
> >> >> deeper and deeper!
>> >> >> again
>> >> >>> agian and again
```

✅**Output**⬇️

> This is outer blociquoe
>> This is inner blockquote:
> >> This line is the most inner one.
>> >> You can go deeper inside...
> >> >> deeper and deeper!
>> >> >> again
>> >> >>> agian and again


### Inline Blockquote:
 ✅**Syntax**:⬇️  
 `<blockquote></blockquote>`

 ✅**Example**:⬇️
```
You can also use this <blockquote>inline syntax</blockquote>
```

 ✅**Output**⬇️   

You can also use this <blockquote>inline syntax for blockquote.</blockquote>