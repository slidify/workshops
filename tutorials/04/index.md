---
title    : Widgets
subtitle : Slidify Workshop
author   : Ramnath Vaidyanathan
mode     : selfcontained # {standalone, draft}
url      : {lib: "../../libraries"}
hitheme  : solarized_light
editlink : "tutorials/02"
assets:
  js:
    - "http://ajax.googleapis.com/ajax/libs/jqueryui/1.10.3/jquery-ui.min.js"
    - "http://bartaz.github.io/sandbox.js/jquery.highlight.js"
  css: "../02/assets/css/app.css"
--- .segue .dark .nobackground

<q>A widget is a collection of stylesheets, javascripts and layouts that add additional functionality to a slide deck.</q>




--- .segue .dark .nobackground

## MathJax

--- .wrappre .centrepre

 	---
 	title: MathJax
 	widgets: [mathjax]
 	mode: draft
 	---
 	
 	## Mathjax ##
 	
 	$$
 	\begin{aligned}
 	\nabla \times \vec{\mathbf{B}} -\, \frac1c\, \frac{\partial\vec{\mathbf{E}}}{\partial t} & = \frac{4\pi}{c}\vec{\mathbf{j}} \\   \nabla \cdot \vec{\mathbf{E}} & = 4 \pi \rho \\
 	\nabla \times \vec{\mathbf{E}}\, +\, \frac1c\, \frac{\partial\vec{\mathbf{B}}}{\partial t} & = \vec{\mathbf{0}} \\
 	\nabla \cdot \vec{\mathbf{B}} & = 0 \end{aligned}
 	$$


--- bg:lightgoldenrodyellow

## Try It

<a class='example'>Your Turn</a>

1. Open `demos/widgets/mathjax/index.Rmd`
2. Slidify and Open `index.html`

You can experiment by adding other equations.

--- .segue .dark .nobackground

## Quiz

--- .wrappre .centrepre

 	---
 	title: Interactive Quiz
 	widgets: [bootstrap, quiz]
 	mode: draft
 	--- &radio
 	
 	## Question 1
 	
 	What is 1 + 1?
 	
 	1. 1 
 	2. _2_
 	3. 3
 	
 	*** .hint
 	
 	This is a hint
 	
 	*** .explanation
 	
 	This is an explanation


--- bg:lightgoldenrodyellow

## Try It

<a class='example'>Your Turn</a>

### Basic

1. Open `demos/widgets/quiz/index.Rmd`
2. Slidify and Open `index.html`

### Intermediate

You can find more question types [here](http://slidify.github.io/iquiz). Press `p` on any slide to get the Rmd source, paste it in your `index.Rmd` file and see how it works.
