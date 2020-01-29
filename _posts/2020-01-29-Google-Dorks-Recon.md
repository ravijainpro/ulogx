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

- intitle:
- inurl:
- intext:
- define:
- site:
- phonebook:
- maps:
- book:
- froogle:
- info:
- movie:
- weather:
- related:
- link:


The above list is just one of few examples of usage, You could deep dive into DB and use any dork of your choice and yield results accordingly.

# Mandatory List to check

It is important to understand that Google dorks aren't just limited to google for that matter, Dorks works on large variety of search engines such as Bing, Duck Duck Go, AOL and Yahoo.

One of main reasons, BB Hunters use Dorks is to locate third party vendors. Organizations and companies use sites such as Pastebin, Jira, Github, Trello, Coggle and more in their daily operations. There would be several instances where hard-coded credentials would be typically stored on a public platform as such.

A dork looking for a third party vendor may look like:

> site: <third party vendor> <Organization name>

A full Checklist of Third-party vendors goes below. 

- [Codepad]

> site: codepad.co "Organization name"

Codepad is an online compiler/Interpreter, you could find hard coded credentials here sometimes. You could look for critical Keys, Passwords, access keys, uuids, special URLs, etc.

- [Gitlab]

> inurl: gitlab "Organization name"

Gitlab, just like github is used to store source code. You could often find internal source code and other sensitive information here.

- [Scribd]

> site: scribd.com "Organization name"

Scribd generally contains books and E-books but you could sometimes expect internal files uploaded by employees that contains passwords or keys.

- [Atlassian]

> site: * .atlassian.net "Organization name"

This dork can be used to find confluence, Jira, and other products that can contain sensitive information.


