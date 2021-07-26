---
title : "Css Inception to Modern Day"
description: "How to Approach Css Development, Understand the many ways to style your html and how to choose the best approach"
date : 2020-05-14T16:49:02Z
draft : false
author : "Calil Drissi"
tags : ["FrontEnd", "Css", "Web Development"]
image: images/feature1/css.svg
authorImage: /images/whoami/author-3.jpg
---


![css ](/images/feature2/css-main.jpeg "San Juan Mountains")


## Let's Begin
![Let's get started](https://media.giphy.com/media/Ln2dAW9oycjgmTpjX9/giphy.gif "start")

CSS short for Cascading Style Sheets, cascading describing the way that one style can cascade from one to another, the technology is one of the three cornerstones that power the world wide web, it's used to describe how HTML elements should be layed out and styled. it's a must know for every web-developer, Luckily it's very accessible to get started and begin writing it, however it can get very complex to master and even harder to maintain. 

In this article we'll go over the history of css, why it came to be, how it evolved and how its ecosystem of libraries, tools and frameworks boommed in the last few years.


## Why was Css invented?
{{< img src="https://media1.tenor.com/images/f4db9e84ef44242c55195a6091616531/tenor.gif" title="" caption="" alt="image alt" width="300px" position="center" >}}
 &nbsp;


**The saga** of CSS starts in `1994`, <mark> Håkon Wium Lie</mark> works at CERN – the cradle of the Web – and the Web is starting to be used as a platform for electronic publishing. One crucial part of a publishing platform is missing, however: There is no way to style documents.Having worked on personalized newspaper presentations at the MIT Media Laboratory, Håkon saw the need for a style sheet language for the Web. 

{{< img src="/images/feature2/hakon-W3C.jpg" title="Håkon Wium Lie" caption="Co-inventor of Css" alt="image alt" width="400px" position="center" >}}



Style sheets in browsers were not an entirely new idea.The separation of document structure from the document's layout had been a goal of HTML from its inception in `1990`. In `1992`, <mark>Pei-Yan Wei</mark> developed a browser called "Viola," which had its own style sheet language. However, the browsers that followed offered their users fewer and fewer options to influence the style. In `1993`, NCSA Mosaic, the browser that made the Web popular, came out. Stylewise, however, it was a backward step because it only allowed its users to change certain colors and fonts.

Meanwhile, writers of Web pages complained that they didn't have enough influence over how their pages looked. One of the first questions from an author new to the Web was how to change fonts and colors of elements. At that time, HTML did not provide this functionality – and rightfully so. 

<mark>Marc Andreessen</mark>, one of the programmers behind NCSA Mosaic. He later became a co-founder of Netscape, a company eager to fulfill the request of authors. On `October 13, 1994`, Marc Andreessen announced to www-talk that the first beta release of Mozilla (which later turned into Netscape Navigator) was available for testing. Among the new tags the new browser supported was center, and more tags were to follow shortly.

{{< boxmd >}}
Three days before Netscape announced the availability of its new browser, `Håkon published the first draft of the Cascading HTML Style Sheets proposal`, Although the first version of the document was immature, it provided a useful basis for discussion.
{{< /boxmd >}}

Among the people who responded to the first draft of CSS was <mark> Bert Bos </mark>. At that time, he was building Argo, a highly customizable browser with style sheets, and he decided to join forces with Håkon. Both of the two proposals look different from present-day CSS, but it is not hard to recognize the original concepts. 
One of the features of the Argo style language was that it was general enough to apply to other markup languages in addition to HTML. This also became a design goal in CSS and "HTML" was soon removed from the title of the specification. Argo also had other advanced features that didn't make it into CSS1, in particular, attribute selectors and generated text. Both features had to wait for CSS2.

{{< img src="/images/feature2/Bert-bos-W3C.jpg" title="Bert Bos" caption="co-Inventor of Css" alt="image alt" width="400px" position="center" >}}


"Cascading Style Sheets" wasn't the only proposed style language at the time. There was Pei Wei's language from the Viola browser, and around 10 other proposals for style sheet languages were sent to the www-talk and www-html mailing lists. Then, there was DSSSL, a complex style and transformation language under development at ISO for printing SGML documents. DSSSL could conceivably be applied to HTML as well. But, CSS had one feature that distinguished it from all the others: It took into account that on the Web, the style of a document couldn't be designed by either the author or the reader on their own, but that their wishes had to be combined, or "cascaded," in some way; and, in fact, not just the reader's and the author's wishes, but also the capabilities of the display device and the browser.

As planned, the initial CSS proposal was presented at the Web conference in `Chicago in November 1994`. The presentation at Developer's Day caused much discussion. First, the concept of a balance between author and user preferences was novel. A fictitious screen shot showed a slider with the label "user" on one side and "author" on the other. By adjusting the slider, the user could change the mix of his own preferences and those of the author. Second, CSS was perceived by some as being too simple for the task it was designed for. They argued that to style documents, the power of a full programming language was needed. CSS went in the exact opposite direction by making a point out of being a simple, declarative format.

At the next WWW conference in `April 1995` CSS was presented again. Both Bert and Håkon were there (in fact, this was the first time they met in person) and this time, they could also show implementations. Bert presented the support for style sheets in Argo, and Håkon showed a version of the Arena browser that had been modified to support CSS. 


In 1995, the World Wide Web Consortium (W3C) also became operational. Companies were joining the Consortium at a high rate and the organization became established. It was therefore decided that another workshop should be organized, this time with style sheets as the topic. The W3C technical staff working on style sheets (namely Håkon and Bert) were now located in Sophia-Antipolis in Southern France where W3C had set up its European site. it was decided to hold the workshop in Paris, which is better served by international flights, Among the participants was Thomas Reardon of Microsoft, who pledged support for CSS in upcoming versions of Internet Explorer. 


At the `end of 1995`, W3C set up the HTML Editorial Review Board (HTML ERB) to ratify future HTML specifications. Because style sheets were within the sphere of interest of the members of the new group, the CSS specification was taken up as a work item with the goal of making it into a W3C Recommendation. Among the members of the HTML ERB was Lou Montulli of Netscape. After Microsoft signaled that it was adding CSS support in its browser, it was also important to get Netscape on board. Otherwise, we could see the Web diverge in different directions with browsers supporting different specifications. The battles within the HTML ERB were long and hard, but <mark> CSS level 1 finally emerged as a W3C Recommendation in 17th December 1996 </mark>.



fast-forward to CSS3 is the latest evolution of the Cascading Style Sheets language that aims at extending CSS2.1. It brings a lot of new features and additions, like rounded corners, shadows, gradients, transitions or animations, as well as new layouts like multi-columns, flexible box or grid layouts.

{{< boxmd >}}
CSS (1996) allows the user to select font style and size and change the colour of the text and background. 
In February 1997, CSS got its own working group inside W3C and the new group set out to work on the features which CSS1 didn't address. 


CSS2 (1998) has capabilities that allows the user to design page layout. 

CSS3 (1999) allows the user to create presentations from documents and to select from a wider range of fonts including those from Google and Typecast. Uniquely, CSS3 allows the user to incorporate rounded borders and use multiple columns. CSS3 is considered to be easier to use (when compared to CSS2) because it has different modules 

{{< /boxmd >}}



## The added value of Css?

Firstly, using CSS ensures that your web pages are consistent. Imagine a website with 100s of pages, now imagine having to input the code to define heading sizes, layout and other display data and mix that all in with the content each time you wanted to produce a new page. Also, imagine having a site with 100s of pages and being able to change just one of them while keeping all the rest the same – CSS also makes that a possibility. Using CSS delivers consistency where it is needed but is flexible enough to enable you to make changes to individual pages or sections. 

### Css allows the developer to specify
* Fonts
* Colour of text and links
* Use colours in the text's background
* Where and how the boxes within the content look and are layed out
* Improve user accessibilty, efficiency, flexiblity and ensures browser compatibility
* Make web content more alive with animations


## How do we use Css today?
![css ](/images/feature2/css.jpeg "State of Css")

Today Css is implement in many different approaches to web development, some even changing day by day. Methodes like BEM (from Yandex),  OOCSS (Nicole Sullivan), SMACSS (Jonathan Snook), Atomic CSS (Yahoo!) and ITCSS (Harry Roberts), the use of   preprocessors such as Less and SCSS; CSS-in-JS libraries, including JSS and styled-components, styling with web components, and lately design systems. You come across all of these in articles and blogs, tutorials, talks and all this sea of information on tools, architectures, frameworks etc... and it can get really messy to navigate and find the right approach to building efficient css for your project... but we should always keep in mind what css is all about in the end, it is just a language to style our html elements.

Here is a quick overview of the different ways, tools and architectures of writing and organizing css style sheets in modern web applications which often have complex interfaces and design patterns: 



### Vanilla Css
If you can, do. No build tooling is refreshing. It will age well. The only thing I really miss without any other tooling is nesting media queries within selector blocks. 


### Pre-processors like SASS
Sass/SCSS has been around the block and is still a hugely popular CSS preprocessor. Sass is built into tons of other tools, so choosing Sass doesn’t always mean the same thing. A simple Sass integration might be as easy as a sass --watch src/style.scss dist/style.css npm script. Then, once you’ve come to terms with the fact that you have a build process, you can start concatenating files, minifying, busting cache, and all this stuff that you’re probably going to end up doing somehow anyway.
you can combine it with BEM and 7-1 file structure

### Css Modules
(Built on PostCSS). If you’re working with components in any technology, CSS modules give you the ability to scope CSS to that component, which is an incredibly great idea. I like this approach wherever I can get it. Your module CSS can be Sass too, so we can get the best of both worlds there.


### Web Components (e.g: stencil.js)
Web components are a set of web platform APIs that allow you to create new custom, reusable, encapsulated HTML tags to use in web pages and web apps. Custom components and widgets build on the Web Component standards, will work across modern browsers, and can be used with any JavaScript library or framework that works with HTML


### CSS-in-JS (e.g: styled-components)
Let’s be real, this means “CSS-in-React.” If you’re writing Vue, you’re writing styles the way Vue helps you do it. Same with Svelte. Same with Angular. React is the un-opinionated one, leaving you to choose between things like styled-components, styled-jsx, Emotion… there are a lot of them. I have projects in React and I just use Sass+CSS Modules and think that’s good but a lot of people like CSS-in-JS approaches too. I get it. You get the scoping automatically and can do fancy stuff like incorporate props into styling decisions. Could be awesome for a design system.

### Classic Frameworks (e.g: bootstrap)
CSS framework is a code library that abstracts common web designs and makes the designs easier for a developer to implement in their web apps. In simple terms, a CSS framework is a collection of CSS style-sheets that are prepped and ready to use. 

### Utility First Frameworks ( e.g: Tailwind)
Utility-first frameworks provide a low-level utility class to build out custom designs within your HTML file. Utility classes are named according to their intended purpose, such that they’re easily understandable to the average person.


### Bem Methodology
BEM is nothing more than a guide: no new framework or language to learn, just CSS with a naming convention to organize things better. Following this methodology, you can implement the patterns you’ve already been using, but in a more structured manner. You can also quite easily do progressive enhancements to your existing codebase as it requires no additional tooling configuration or any other complexities.

### Design Systems

the need for atomic design (basically breaking down UI into basic building blocks), many companies are choosing to create component libraries and design systems. Unlike the technologies or approaches on how to handle styling mentioned above, design systems represent an organizational approach to handling components and consistent design across whole platforms or apps.


### Most Popular Ways

BEM, along with SCSS, could help you organize your style sheets better, take a programming approach to CSS, and create meaningful structured class names for cleaner code with minimal configuration. 

Building over a front-end framework like React or Vue, you might it find it convenient to hand class naming to a CSS-in-JS library if you’re comfortable with a component-based approach, putting an end to all your specificity issues, along with a couple of other benefits. 

For larger applications and multiple platforms, you might even consider building a design system in combination with one of the other methods, to boost development speeds while maintaining consistency.


## Conclusion
Styling applications is a world in itself, one not often given the importance and attention it deserves. With complex modern user interfaces, it’s only matter of time before your app becomes a mess of unordered styles, reducing consistency and making it harder for new code to be added or changes made to the existing codebase.

Essentially, depending on your requirements and the size and scale of your software, it’s important to spend time determining your best approach to styling.




