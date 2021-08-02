---
date: 2021-07-31 22:04:08
layout: post
title: Gadling Report - Technicals of Bhima Koregaon Case
subtitle: Technical aspects of Bhima koregaon case
description: Bhima koregaon case and technical aspects have been covered from a security point of view in the below article.
image: ../assets/img/blog/forensics.jpg
optimized_image: ../assets/img/blog/forensics.jpg
category: music
tags:
  - Security
  - Forensics
author: Venkatesh Sharma
---

**This analysis mostly covers the technical aspects of the Bhima Koregaon case which alleges 16 activists were involved in a plot to assassinate the Prime Minister after violence broke out during the Elgar Parishad event on 1st Jan 2018.** The incriminating evidence uncovered from the laptops of the accused is the basis of their incarceration, but the reports and analysis conducted by Arsenal Consulting conclude that the documents were planted by a malicious actor and were never created or used on the devices in the first place.



As we start analyzing the report by Arsenal Consulting (June 2021), what we see right away is that the Netwire malware itself is not a custom made one, it’s a legacy malware available commercially online. It has been well known since 2012. Sophisticated actors usually build their own malicious code to bypass detection from antiviruses and firewalls.



Visual Basic (a programming language for Windows) scripts were used for the execution. The Netwire malware was obfuscated or crypted in VB to evade detection from antivirus software, which was installed on the computer.



Email attachments infected with the malware were used to spear-phish (electronic communication based attack targeted towards a specific individual, organization or business) the victim, but what we also see is how well informed the attackers were. In order to be able to successfully social-engineer other victims implicated in the Bhima Koregaon case (in order to make the victim execute the file without hesitation), they made 3 attempts with emails sent to multiple people, and succeeded in their 3rd attempt to infiltrate Mr. Gadling’s system. We can see the date difference between the emails sent on 12 Feb and 18 Feb. Mr. Gadling executed the file on 28 Feb. We can assume time was taken to stalk/cyber-stalk the victims and send them relevant email content and files that they would assume is related to their work.


## Breaking down the hack -  

1. They used VB scripts to evade antivirus scans, then zipped the actual malware files to avoid detection by Google's default attachment malware scanner.

2. The malware was fetched and executed from a javascript file with help of windows-script-host or wscript. wscript is a Windows local script executable that interprets JS/VB locally and can execute shell commands.

3. The attack is well-known as "drive-by download" and the wscript waited for the download of the executable malware and then executed once opened.

4. We also see tools like WinSCP, unRAR etc, but Netwire comes bundled with these tools as well, as its online ad and promotion listing describes on Google. What matters more is what variant was used and how it was customized.

5. They used a no-IP service (Zapto) as malware connect back / sink (Atlaswebportal.zapto.org) to avoid their personal computer’s IP address from getting logged. Services like Zapto usually keep a track of data and user logs which can be further investigated to try and identify the hacker.

The report also mentions that the other Netwire samples from the QuickHeal and VirusTotal quarantine folders connected to the same command and control server. It’s possible that there is some kind of a SAAS platform where the malware was purchased from.

As windows hides the file extension, a hacker can add a double extension to hide the real file type (for example something.doc.js), which is a commonly used trick to hide extension names for malicious files.

Since 2009 until now, there have been around 1855 exploits/vulnerabilities of Windows 7, of which 622 methods were still available at the time of the attack. It was possible to compromise a Windows 7 system at that time without going to this extent of exposing themselves.
 
Hardcoded command and control server IP, not even using base64 encoding to hide the server IP, is indication of sloppy work. It seems more of a task that was delegated to someone who was somewhat technically adept, rather than a professional hacker who would know how to hide their tracks.

The inconsistency in the finer points of action, along with differing versions of Winrar and Unzip installed on the computer and used for the delivery of incriminating evidence, and the lack of Object Identifiers in Windows NTFS that would log opening or use of the files point to an inexperienced hacker/team. The different operating procedures compared to Mr. Rona Wilson’s hack also points to a possible team that was delegated multiple tasks instead of a single actor working alone.

Looking at all the contents of the malware, it seems more like a cyber espionage kit than a sophisticated cyber attack.

Further investigating the hosting and the no-IP services, logs from ISP, the local router logs if it's logging packets, and the email logs could lead to identifying the attacker.


Venkatesh L

CISSP,OSCP,CEH

Mr. Pentester


























