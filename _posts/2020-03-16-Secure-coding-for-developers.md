---
date: 2020-03-16 14:55:45
layout: post
title: Secure Coding for Developers
subtitle: Cyber Security for Developers in a nutshell
description: Secure coding principles for Developers to reduce vulnerabilities before their inception. This post speaks of robust
image: https://raw.githubusercontent.com/ujwalpro/ujwalpro.github.io/master/assets/img/blog/securecoding.jpg
optimized_image: https://raw.githubusercontent.com/ujwalpro/ujwalpro.github.io/master/assets/img/blog/securecoding.jpg
category: Security
tags:
  - cyber security
  - coding
  - secure coding
author: Ujwal kumar
---

While there are new Platforms, Applications and Softwares coming up every single day, Security is top-of-mind for most people working with technology. Over the years, there has been increasing awareness about data breaches, Cyber attacks and what not. Developers now don't just require to enhance their coding to obtain higher accuracy, optimization and speed, they need to work upon most crucial aspect, **Security**. It has become extremely important to have the "know-how" of Secure Coding. Through this post, I'll be covering principles by which you could enhance your secure coding skills to create more robust & Trust worthy software's in future. 

Here's a list of Rules which are highly reccommended while you code:

### 1) Input Validation of all Types of Inputs

For any Dynamic Website, it is obvious that there would be Incoming data. In the midst of it, it is important to "Not Trust any Data at all" irrespective of it's nature. The most prevalent security weakness of current applications is a failure to correctly process data that is received from external sources, particularly user input. You should always take a close look at any input to make sure it has been validated before it is used. Failing to analyze user input for possible attacks can result in data loss or exposure, elevation of privilege, or even execution of malicious code on other users' computers. Failing to validate user inputs leads to Vulnerabilities like SQL Injections, Command Injections, Cross Site scripting, etc. ( For people who don't know of these attacks, you don't need to be intimidated by the names, as developers you can easily avoid these )

**Why Do you need to validate the input?**
Suppose that you are building an interface to allow a user to create an account on your website. Our profile data includes a name, Phone number, and a nickname that we will display to everyone who visits the site. What if a new user creates a profile and enters a nickname that includes some SQL commands? For example - what if a malicious user enters something like the following excerpt:

```SQL
// This SQL Command will directly get executed in your backend if not validated

Ujwal'); DROP TABLE Users;--

```

If we blindly insert this value into a database, it could potentially alter the SQL statement to execute commands we absolutely don't want to run! This example is referred to as a "SQL Injection" attack, which is one of the many types of exploits that can potentially be done when you don't properly handle user input.

**When do you need to validate input?**
The answer is **always**. You must validate every input for your application. This Includes :
* Inputs from the user
* Data from the Database
* Data from the API
* URL Parameters
* Usage of data coming from a third party service.

Always use an "allow" list approach, which means you only accept "known good" input, instead of a deny list (where you specifically look for bad input) because it's impossible to think of a complete list of all potentially dangerous inputs. Do this work on the server side, not the client-side (or in addition to the client-side), to ensure that your defenses cannot be circumvented.

For Input validation based on frameworks, you could use:
* Regular expressions
* Whitelisting Vs Blacklisting (Former always wins)
* File Upload Validation
* Ensure that any input validation performed on the client is also performed on the server.

### 2) Output encoding Required always

Any output you present either visually or within a document should always be encoded and escaped. This can protect you in case something was missed in the sanitization pass, or the code accidentally generates something that can be used maliciously. This desigh principle will make sure that everything is displayed as output and not inadvertently interpreted as something that should be executed, which is another common attack technique that is referred to as "Cross-Site Scripting" (XSS). When you encode all outputs, it decreases the chances for attacker to find a potential vulnerability and exploit it, even if you missed out anything accidentally. Of course, Because mistakes happen by humans.

### 3) Use Parameterized Queries always.

**Never Ever Use Inline SQL Queries, Ever**
















