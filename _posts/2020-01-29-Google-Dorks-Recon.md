---
date: 2020-01-29 12:30:49
layout: post
title: Google Dorks, Recon & OSINT
description: Complete Hands on, recon using Google dorks and other OSINT tricks for Critical info extraction for Bug Bounty.
image: https://res.cloudinary.com/dm7h7e8xj/image/upload/v1559824021/theme12_e0vxlr.jpg
optimized_image: https://res.cloudinary.com/dm7h7e8xj/image/upload/c_scale,w_380/v1559824021/theme12_e0vxlr.jpg
subtitle: Google dorks Usage - Basics to Advanced For Bug Bounty.
category: 'Recon'
tags:
  - Google 
  - OSINT
  - Recon
  - Bug Bounty
author: Ujwal kumar
---

Google hacking, also named Google dorking, is a computer hacking technique that uses Google Search and other Google applications to find security holes in the configuration and computer code that websites use. 
These techniques are excellent in manual recon methodology to find crucial information about any organization, which might have been left out due to certain consequences.

> This method may be time consuming, but it has it's own set of results which might be extremely crucial to model threat vectors against any target being tested against.

Before I list out structural methodology for greater usage of **Google Dorking**, Here's a list of resources which you'd like to go through for greater clarity. Credits to the creators.

- [Google Hacking for Penetration Testing - Elaborate video](https://www.youtube.com/watch?v=cFOBUYaxdWI)

Here's the official link of Google Hacking Database (GHDB)
- [GHDB](https://www.exploit-db.com/google-hacking-database)

If you find a new unique way to Dork searches, you could get your own Dork published as well. Adds to your work and benifits the overall database.

# Formula of Google Dorks

Dorks : They are like search criteria in which a search engine returns results related to your dork.
The process can be a little time consuming, but the outcome will be worth it after learning on how to use dorks.

## Basic Formula of dork

"inurl:."domain"/"dorks" "

So you would normally understand it like this:
"inurl" = input URL

"domain" = your desired domain. For eg, .gov, or .edu or so on, Based On target specification.

"dorks" = The dork of your choice

Here is another example of that

You can use following words instead of inurl :

-intitle:
-inurl:
-intext:
-define:
-site:
-phonebook:
-maps:
-book:
-froogle:
-info:
-movie:
-weather:
-related:
-link:


The above list is just one of few examples of usage, You could deep dive into DB and use any dork of your choice and yield results accordingly.

# Mandatory List to check

It is important to understand that Google dorks aren't just limited to google for that matter, Dorks works on large variety of search engines such as Bing, Duck Duck Go, AOL and Yahoo.

One of main reasons, BB Hunters use Dorks is to locate third party vendors. Organizations and companies use sites such as Pastebin, Jira, Github, Trello, Coggle and more in their daily operations. There would be several instances where hard-coded credentials would be typically stored on a public platform as such.

A dork looking for a third party vendor may look like:

#### site:<third party vendor> <Organization name>

## Code

Cum sociis natoque penatibus et magnis dis `code element` montes, nascetur ridiculus mus.

```js
// Example can be run directly in your JavaScript console

// Create a function that takes two arguments and returns the sum of those arguments
var adder = new Function("a", "b", "return a + b");

// Call the function
adder(2, 6);
// > 8
```

Aenean lacinia bibendum nulla sed consectetur. Etiam porta sem malesuada magna mollis euismod. Fusce dapibus, tellus ac cursus commodo, tortor mauris condimentum nibh, ut fermentum massa.

## Lists

Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Aenean lacinia bibendum nulla sed consectetur. Etiam porta sem malesuada magna mollis euismod. Fusce dapibus, tellus ac cursus commodo, tortor mauris condimentum nibh, ut fermentum massa justo sit amet risus.

* Praesent commodo cursus magna, vel scelerisque nisl consectetur et.
* Donec id elit non mi porta gravida at eget metus.
* Nulla vitae elit libero, a pharetra augue.

Donec ullamcorper nulla non metus auctor fringilla. Nulla vitae elit libero, a pharetra augue.

1. Vestibulum id ligula porta felis euismod semper.
2. Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus.
3. Maecenas sed diam eget risus varius blandit sit amet non magna.

Cras mattis consectetur purus sit amet fermentum. Sed posuere consectetur est at lobortis.

Integer posuere erat a ante venenatis dapibus posuere velit aliquet. Morbi leo risus, porta ac consectetur ac, vestibulum at eros. Nullam quis risus eget urna mollis ornare vel eu leo.

## Images

Quisque consequat sapien eget quam rhoncus, sit amet laoreet diam tempus. Aliquam aliquam metus erat, a pulvinar turpis suscipit at.

![placeholder](https://placehold.it/800x400 "Large example image")
![placeholder](https://placehold.it/400x200 "Medium example image")
![placeholder](https://placehold.it/200x200 "Small example image")

## Tables

Aenean lacinia bibendum nulla sed consectetur. Lorem ipsum dolor sit amet, consectetur adipiscing elit.

<table>
  <thead>
    <tr>
      <th>Name</th>
      <th>Upvotes</th>
      <th>Downvotes</th>
    </tr>
  </thead>
  <tfoot>
    <tr>
      <td>Totals</td>
      <td>21</td>
      <td>23</td>
    </tr>
  </tfoot>
  <tbody>
    <tr>
      <td>Alice</td>
      <td>10</td>
      <td>11</td>
    </tr>
    <tr>
      <td>Bob</td>
      <td>4</td>
      <td>3</td>
    </tr>
    <tr>
      <td>Charlie</td>
      <td>7</td>
      <td>9</td>
    </tr>
  </tbody>
</table>

Nullam id dolor id nibh ultricies vehicula ut id elit. Sed posuere consectetur est at lobortis. Nullam quis risus eget urna mollis ornare vel eu leo.


