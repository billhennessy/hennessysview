---
authors: ["Bill Hennessy"]
date: 2007-03-06 04:14:53+00:00
draft: false
title: Have We Taken Metadata Too Far
layout: blog
url: /2007/03/05/have-we-taken-metadata-too-far/
categories:
- Latest
---

Recently, I’ve had the task of explaining to clients why it’s more difficult and error-prone to change their web applications’ configuration metadata than to change code. They don’t take my story well. After all, the whole idea of many web applications is _configurability_. By that I mean that a non-programmer can change, add, or remove values that cause either business rules, workflows, navigation flows, or content of a web site to change.




Once upon a time, we hard coded everything, save for _transactional data_, the stuff that the web site captures through user interaction (name, address, phone number, buy a book, etc.), or the data that arrives in files or through web services for display on the web site. Whenever a client wanted to change, say, the color of the GO button, a programmer coded the change, a tester tested, and someone released the code to production.




The idea behind configurability was to eliminate all this programming so that the customer could make the change and be done with it.




Then came security, process, and compliance.




Between Sarbanes-Oxley, SAS70, PCI DSS, and CMMi, the practice of making system configuration change directly to production went the way of 8.25 inch floppies. Metadata changes must be treated like code: defined, approved, developed, tested, staged and tested again, then released. But data are not code. Data are values arranged in columns and rows, usually identified by a sequential, unique number. Even if you solve the unique number problem with GUIDs, you still have to create crude SQL scripts, apply them to an environment and test. If the client wants changes or finds defects, you have to refresh the database (blowing away any test case data created), change the script, and re-apply it to the test environment. And so on.




This whole process would actually be easier were these metadata hard coded into tiny artifacts.




I think my next design will contain such artifacts. Perhaps they will leverage the Windows Workflow Foundation. Instead of changing data, I’ll simply reorder the artifacts or tweak a rule and move the changes through the testing assembly line. Less risk, faster code (since there are no database round trips), and I don’t have to train clients how highly structured, mature processes work.

