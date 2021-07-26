---
title: Types of Front-End Websites
date: 2021-07-26T12:00:06+09:00
description: Frontend web development is one of the domains that's changing rapidly in this article we are going the explore the three main methods web front-ends are built today
draft: false
hideToc: false
enableToc: true
enableTocContent: false
authorImage: /images/whoami/author-3.jpg
author : "Calil Drissi"
tags:
- html
categories:
- Web Development
image: images/feature1/website.svg
---


Technology has evolved in different ways and in the same way the concepts of building products or tools. Frontend web development is one of the domains which is changing rapidly with the growing community and requirements of faster development. Many libraries and frameworks have been introduced to the developers starting from jquery to react, angular etc. Every technology, concept, library and framework have its own pros and cons but they know how to stand out as per the requirement.

In this article, I am going to discuss different methods of creating frontend sites.
Topics

- Vanilla HTML Websites
- Client-Side Rendering
- Server-Side Rendering
- Static-Site Generator

## Vanilla HTML Websites

Vanilla HTML or Static Websites are the raw form of websites that we build using HTML, CSS, JavaScript. They are directly served from a web host or CDN.

![static-website](https://cdn.hashnode.com/res/hashnode/image/upload/v1621176481419/sVusuh4Lb.jpeg?auto=compress,format&format=webp "static-web")

Pros

* It is easy to get started with.
* Generally, not so complex.
* SEO optimization can be done.

Cons

* Less modularity; Hard to update/maintain pages as we need to rewrite a lot of the same code for every page.
* New request to the server for every page.
* Generally, do not contain dynamic data.


## Client-Side Rendering

You may have heard this term many times, it is also known as CSR in short. So what happens in Client-Side Rendering?

When we build a site with React, Angular or Vue, it creates a SPA (Single Page Application) that doesn't have any pre-rendered HTML pages. When the browser requests the server for the site, the initial request is for a blank HTML page and then it fetches the JS scripts that manipulate the DOM and render the pages. Routing, data handling etc., are also done within the browser itself.


![client-rendering](https://cdn.hashnode.com/res/hashnode/image/upload/v1621177704707/CzL1inkZ7.png?auto=compress,format&format=webp "spa")


Pros

* Easy to maintain codebase.
* Modular approach.
* It's fast except for the initial request.

Cons

* It is not SEO friendly.
* It can become complex.
<br>
> React.js, Angular, Vue can be used to build SPAs.

We can optimize these kinds of sites with Server-Side Rendering.

## Server-side Rendering

In Server-Side Rendering, the pages are rendered on the server on every request for it. The server aggregates the data from its source like a database and fed it to the templates to render the requested HTML pages. And rendered pages are then sent back to the browser, to display to the user.

![ssr](https://cdn.hashnode.com/res/hashnode/image/upload/v1621178361766/o92jvSxda.png?auto=compress,format&format=webp "ssr")

Pros

* Easy to maintain codebase.
* Modular approach.
* SEO friendly.

Cons

* Network latency can impact.
* Request for every page.
> Next.js for React and Nuxt.js for Vue can be used for Server-Side Rendering.

There is a hybrid approach to get benefits of both CSR and SSR which we will be discussing next.

## Static-Site Generator
In Static-Site Generator, the static pages are compiled at the build-time i.e, before deployment with some initial data. The static pages are then deployed to a web server. After the initial request, the site behaves more like a Single-Page Application.

![ssc](https://cdn.hashnode.com/res/hashnode/image/upload/v1621179375849/uDbKkaMo5.png?auto=compress,format&format=webp "ssc")


Pros

* Easy to maintain codebase.
* Modular approach.
* SEO friendly.

Cons

* It can become complex.

* Gatsby.js with React can be used for Static-Site Generator.

## Conclusion

There is no hard and fast rule on which one you should use. It depends on your application and its usage.

In my opinion, Client-Side Rendering is suited for applications where users will stay for a longer time and will interact often and want a user experience similar to a desktop application. For example, a trading platform. While Server-side Rendering is good for applicationslike blogging platform that need to be optimized for SEO such as Wordpress or Ghost Systems.



