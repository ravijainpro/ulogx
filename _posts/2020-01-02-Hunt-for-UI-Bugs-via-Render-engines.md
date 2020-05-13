---
date: 2020-01-02 12:26:40
layout: post
title: Hunt for UI bugs due to WebRender
subtitle: Hunt from Home, Mozilla karnataka! UI Bug Hunting
description: WebRenders vary due to which graphical bugs arise. Here we'd cover about method to hunt these bugs and contribute to mozilla
image: https://raw.githubusercontent.com/ujwalpro/ujwalpro.github.io/master/assets/img/blog/webrender.png
optimized_image: https://raw.githubusercontent.com/ujwalpro/ujwalpro.github.io/master/assets/img/blog/webrender.png
category: Non-Security
tags:
  - Non-security
  - UI-Bugs
  - Rendering
author: Ujwal kumar
---

Every developer would agree to the fact that, your code is Incomplete if you never encountered bugs. Irrespective of when it would've arised, the satisfaction you get after resolving them is unbeatable, as it helps you move towards "Perfection" or atleast help you get better and design an experience for your user.

It's important that we celebrate these bugs and embrace the positive change they bring in us eventually. In this work, we would focus on UI bugs and the methodology which you could use to do your part of contribution.
Before we go ahead, you'd require to understand what is [Rendering Engine](https://www.pathinteractive.com/blog/design-development/rendering-a-webpage-with-google-webmaster-tools/).

## What is rendering engine?

It takes HTML code and interprets it into what you see visually. For instance, a tag would be interpreted by the rendering engine as a set of instructions to make the text inside of the element <b>bold</b>

The rendering engine has a very important job as it displays what you see on your screen. It communicates with the networking layer of the browser to grab HTML code and other items passed from a remote server.

While Google, Opera and their variants use <b>blink</b> as their rendering engine which accounts 43% of usage, whilst Internet explorer uses <b>Trident</b>(25.8%>, Firefox and it's variants uses <b>Gecko</b>(18.22%), whereas Safari uses <b>Webkit</b>. [source](https://en.wikipedia.org/wiki/Browser_engine)










