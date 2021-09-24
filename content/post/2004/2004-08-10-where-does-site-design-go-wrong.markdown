---
authors: ["Bill Hennessy"]
date: 2004-08-10 13:45:22+00:00
draft: false
title: Where Does Site Design Go Wrong?
layout: blog
url: /2004/08/10/where-does-site-design-go-wrong/
categories:
- Latest
---

I am simultaneously juggling four new websites, all built on the DotNetNuke portal framework with massive customization. The biggest challenge so far has been deciding





  * What goes into the site?
  * What main tabs?
  * What sub tabs?
  * What security roles?
  * What can each security role see and do?


In other words, basic site design and flow. 




In almost every site I've designed, I've begun down the wrong path. I don't get far, mind you, but I always start off the wrong way. I have worked with a lot of designers who have this problem, and a few who don't. Over the years, I've learned something from the latter: Don't do more than you have to.




You'd think that someone who preaches simplicity of design, simplicity of architecture, simplicity of code would understand simplicity of web design out of the box. But the array of options available to the site designer seems overwhelming sometimes. So here's how I approach site design now, in order to limit my choices on the first round:





  * Create Main Menu items for each major user group. For a school application, those are Students, Parents, Teachers, and Alumni.
  * Create Main Menu items for each major general activity area. Using the school motif, those might be Sports, Clubs, Curriculum, and School Store. 
  * Create a Utility area for subject matter administrators (as opposed to site administrators). This will hold master calendars, lunch menus, etc.


That's it. Now, let the customer flesh these areas out. Build the skeleton site using only the navigation bar. Start with the things a Student would want to see. Ask if Teachers or Parents or Alumni might also want access to the information? If the answer is yes, create a central admin tool under the Utilities area and shadow the controls in each area that needs them. Continue this process through each of the major User Groups, then each of the major Activity Groups, until the site is complete.




Remember, this is only a start and only one way of designing a functional web site. But its the method I've seen repeated successfully by site designers who seem always to get it right the first time.




{{< figure src="https://blog.billhennessy.com/aggbug.aspx?PostID=647" >}}

