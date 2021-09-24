---
authors: ["Bill Hennessy"]
date: 2005-01-17 04:53:00+00:00
draft: false
title: Master/Detail Dropdownlists Without Postback
layout: blog
url: /2005/01/17/masterdetail-dropdownlists-without-postback/
categories:
- Latest
---

Suppose you have three sets of data: Customers, Orders, Products.




You want to present three dropdownlists--one for each set of data. When I select a Customer from list A, list is rebuilt with Orders for that customer, the first order is selected, and list C is updated with the Products for that order, the first Product selected.




Using ASP.NET postbacks is pretty straightforward, but it's also pretty ugly. [Al Alberto ](https://www.codeproject.com/aspnet/MasterDetailDDL.asp?select=1016022&forumid=14297&df=100&msg=1016022)got us most of the way to a solution with this article on CodeProject. [I've taken his work and extended to achieve the solution descibed above](https://blog.billhennessy.com/forums/927/ShowPost.aspx).







{{< figure src="https://blog.billhennessy.com/aggbug.aspx?PostID=930" >}}

