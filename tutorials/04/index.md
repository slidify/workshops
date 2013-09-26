---
title       : How Slidify Works?
subtitle    : Slidify Workshop
author      : Ramnath Vaidyanathan
hitheme     : solarized_light 
mode        : selfcontained # {standalone, draft}
assets:
  js:
    - "http://ajax.googleapis.com/ajax/libs/jqueryui/1.10.3/jquery-ui.min.js"
    - "http://bartaz.github.io/sandbox.js/jquery.highlight.js"
  css: "http://fonts.googleapis.com/css?family=Crimson+Text"
---




--- .segue .dark .nobackground

## Deck


--- &callout #step3a .centrepre


	---
	title: Slidify
	author: Ramnath Vaidyanathan
	framework: io2012
	---
	## Get Started
	
	Slidify is easy to use, only three rules!
	
	1. Write content using R Markdown
	3. Add properties using YAML
	4. Separate slides using `---`
	
	---
	## Example Slide
	
	Let us create a __scatterplot__
	
	```{r}
	require(ggplot2)
	qplot(wt, mpg, data = mtcars)
	```


*** #draggable5 .left

Properties

--- &callout #step3b .centrepre


	---
	title: Slidify
	author: Ramnath Vaidyanathan
	framework: io2012
	---
	## Get Started
	
	Slidify is easy to use, only three rules!
	
	1. Write content using R Markdown
	3. Add properties using YAML
	4. Separate slides using `---`
	
	---
	## Example Slide
	
	Let us create a __scatterplot__
	
	```{r}
	require(ggplot2)
	qplot(wt, mpg, data = mtcars)
	```


*** #draggable6 .left

Slide

--- &callout #step3c .centrepre


	---
	title: Slidify
	author: Ramnath Vaidyanathan
	framework: io2012
	---
	## Get Started
	
	Slidify is easy to use, only three rules!
	
	1. Write content using R Markdown
	3. Add properties using YAML
	4. Separate slides using `---`
	
	---
	## Example Slide
	
	Let us create a __scatterplot__
	
	```{r}
	require(ggplot2)
	qplot(wt, mpg, data = mtcars)
	```


*** #draggable7 .left

Separator

--- &callout #step3d .centrepre


	---
	title: Slidify
	author: Ramnath Vaidyanathan
	framework: io2012
	---
	## Get Started
	
	Slidify is easy to use, only three rules!
	
	1. Write content using R Markdown
	3. Add properties using YAML
	4. Separate slides using `---`
	
	---
	## Example Slide
	
	Let us create a __scatterplot__
	
	```{r}
	require(ggplot2)
	qplot(wt, mpg, data = mtcars)
	```


*** #draggable8 .right

Markdown


--- &callout #step3e .centrepre


	---
	title: Slidify
	author: Ramnath Vaidyanathan
	framework: io2012
	---
	## Get Started
	
	Slidify is easy to use, only three rules!
	
	1. Write content using R Markdown
	3. Add properties using YAML
	4. Separate slides using `---`
	
	---
	## Example Slide
	
	Let us create a __scatterplot__
	
	```{r}
	require(ggplot2)
	qplot(wt, mpg, data = mtcars)
	```


*** #draggable9 .right

Code Chunk

--- .segue .dark .nobackground

## Slide

--- .centrepre



	--- {class: [class1, class2], id: id}
	
	## Title
	
	Some content
	
	*** {name: block1, class: class3}
	
	## Block1 Title
	
	Some contents of block 1
	
	*** {bg: green}
	
	## Block2 Title
	
	Some contents of block 2



--- {id: step1a, tpl: callout, class: 'centrepre'}

```no-highlight

 --- {class: [class1, class2], id: id}
 
 ## Title
 
 Some content
 
 *** {name: block1, class: class3}
 
 ## Block1 Title
 
 Some contents of block 1
 
 *** {bg: green}
 
 ## Block2 Title
 
 Some contents of block 2


```

*** .right

Properties

*** =pnotes

### Properties

Slide properties are key-value pairs that are passed to the layout. You can specify class, id and bg and style the slide, either by using built in classes, or specifying additional css.

    --- {class: [class1, class2], id: id}

You can also use symbolic css style prefixes for frequently used properties. For instance, a dot indicates class, a hash refers to id and an ampersand identifies a layout.

    --- .class1 .class2 #id


--- .centrepre #step1b &callout

```no-highlight

 --- {class: [class1, class2], id: id}
 
 ## Title
 
 Some content
 
 *** {name: block1, class: class3}
 
 ## Block1 Title
 
 Some contents of block 1
 
 *** {bg: green}
 
 ## Block2 Title
 
 Some contents of block 2


```

*** .left

Title

--- .centrepre #step1c &callout

```no-highlight

 --- {class: [class1, class2], id: id}
 
 ## Title
 
 Some content
 
 *** {name: block1, class: class3}
 
 ## Block1 Title
 
 Some contents of block 1
 
 *** {bg: green}
 
 ## Block2 Title
 
 Some contents of block 2


```

*** .left

Content

--- .centrepre #step1d &callout

```no-highlight

 --- {class: [class1, class2], id: id}
 
 ## Title
 
 Some content
 
 *** {name: block1, class: class3}
 
 ## Block1 Title
 
 Some contents of block 1
 
 *** {bg: green}
 
 ## Block2 Title
 
 Some contents of block 2


```

*** .left

Blocks

*** =pnotes

## Blocks

Blocks are slides nested within a slide, identified by three stars. Just like a slide, they can contain  properties, title and content. 

There are two types of blocks - named and unnamed. A block can be named by specifying the property `{name: block1}` (or using the symbolic shortcut `{=block1}`). 

A block with the name `block1` can be accessed in a slide layout as `slide.block1`. The title and content of this block can be accessed as `slide.block1.title` and `slide.block1.content`. Unnamed blocks are aggregated into the namespace `slide.blocks`. 


--- .dark .nobackground .segue

## Code Chunks

--- .centrepre &callout #chunk1

    ```{r example, fig.width = 6, comment = NA}
    x <- 1+1
    rnorm(5)
    ```
    
*** .left #markup build:true

Markup

*** .top #label build:true

Label


*** .top #options build:true

Options

*** .bottom #code1 build:true

Code

--- .centrepre &callout #chunk2



	```{r example, fig.width = 6, comment = NA}
	x <- 1+1
	rnorm(5)
	```



    
*** .left #markup

Markup

--- .dark .quote .nobackground

<q>The overriding design goal for Markdown’s formatting syntax is to make it as readable as possible. The idea is that a Markdown-formatted document should be publishable as-is, as plain text, without looking like it’s been marked up with tags or formatting instructions.</q>

--- .segue .dark .nobackground

## Frameworks

--- .centrepre &callout #impress-example .wrap

	---
	title: Testing ImpressJS
	author: Ramnath Vaidyanathan
	mode  : selfcontained
	framework: impressjs
	github: {user: ramnathv, repo: slidify}
	twitter: {text: "Slidify with impress.js!"}
	--- .slide x:-1000 y:-1500
	
	<q>Aren't you just **bored** with all those slides-based presentations?</q>
	
	--- .slide x:0 y:-1500
	
	<q>Don't you think that presentations given **in modern browsers** shouldn't **copy the limits** of 'classic' slide decks?</q>
	
	--- .slide x:1000 y:-1500
	
	<q>Would you like to **impress your audience** with **stunning visualization** of your talk?</q>


<style>#impress-example pre{width: 95%}</style>






