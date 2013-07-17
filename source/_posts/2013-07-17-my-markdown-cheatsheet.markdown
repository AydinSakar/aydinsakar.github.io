---
layout: post
title: "My Markdown Cheatsheet"
date: 2013-07-17 15:49
comments: true
categories: 
- Markdown
---

Since this blog will also serve as my cheatsheets repository for everything I want to remember, here is my [markdown][] cheatsheet:

+ Whenever an indentation is needed it is allways **1 tab** or **4 spaces** in markdown.

##### Headers:
```
# h1 Header 
## h2 Header 
### h3 Header 
#### h4 Header 
##### h5 Header 
###### h6 Header 
```
# h1 Header 
## h2 Header 
### h3 Header 
#### h4 Header 
##### h5 Header 
###### h6 Header 

#### Lists:
```
* first item
* second item
* third item
or
- first item
- second item
- third item
or
+ first item
+ second item
+ third item
```
* first item
* second item
* third item

#### Numbered Lists
```
1. first item
2. second item
3. third item
```
1. first item
2. second item
3. third item

#### Mix Lists
```
1. first item
    + first item
    + second item
    + third item
2. second item
3. third item
```
1. first item
    + first item
    + second item
    + third item
2. second item
3. third item

#### Emphasis/Strong
```
*emphasized*
_emphasized_
**strong**
__strong__
***strong emphasized***
___strong emphasized___
```
*emphasized*  
**strong**  
***strong emphasized***

#### Code Blocks:
```
    This is a code block indented by 4 spaces
```
    This is a code block indented by 4 spaces and the spaces removed

#### Blockquotes:
```
> This is a blockquote with two paragraphs. Lorem ipsum dolor sit amet,
consectetuer adipiscing elit. Aliquam hendrerit mi posuere lectus.
Vestibulum enim wisi, viverra nec, fringilla in, laoreet vitae, risus.

> Donec sit amet nisl. Aliquam semper ipsum sit amet velit. Suspendisse
id sem consectetuer libero luctus adipiscing.
```
> This is a blockquote with two paragraphs. Lorem ipsum dolor sit amet,
consectetuer adipiscing elit. Aliquam hendrerit mi posuere lectus.
Vestibulum enim wisi, viverra nec, fringilla in, laoreet vitae, risus.

> Donec sit amet nisl. Aliquam semper ipsum sit amet velit. Suspendisse
id sem consectetuer libero luctus adipiscing.

#### Markdown in Blockquotes:
```
> ## This is a header.
> 
> 1.   This is the first list item.
> 2.   This is the second list item.
> 
> Here's some example code:
> 
>     return shell_exec("echo $input | $markdown_script");
```
> ## This is a header.
> 
> 1.   This is the first list item.
> 2.   This is the second list item.
> 
> Here's some example code:
> 
>     return shell_exec("echo $input | $markdown_script");

#### Blockquote in blockquote:
```
> This is the first level of quoting.
>
> > This is nested blockquote.
>
> Back to the first level.
```

> This is the first level of quoting.
>
> > This is nested blockquote.
>
> Back to the first level.


[markdown]: http://daringfireball.net/projects/markdown/syntax  "Markdown"