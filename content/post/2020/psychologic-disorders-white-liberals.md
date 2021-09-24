---
title: "White Liberals Twice as Likely to be Diagnosed with Psychological Problems"
date: 2020-10-10T13:38:01-05:00
url: psychologic-disorders-white-liberals
authors: ["Bill Hennessy"]
images: ["/images/mental-illness.jpg"]
categories: ["Politics", "Living"]
tags: ["Psychology"]
draft: false
---

Liberals of all ages and races are twice as likely to suffer from mental illness than conservatives, but white liberals are particularly prone to psychological and psychiatric problems. 

Researchers have identified a strong correlation between liberalism and mental illness.The correlation is so powerful that almost **one in two young white liberals have been diagnosed with mental health disorders** according to Pew American Trends research. 


{{< figure src="/images/pew-psyc.JPG" caption="Crosstab analysis of Pew March 2020 American Trends survey data by Zach Goldberg @ZachG932" >}}

We have identified four major takeaways from this research, conducted earlier this year:

1. Nearly 1 in 2 (45.9%) of white liberals have been diagnosed with mental health disorders.
2. White liberals of all ages are more than twice as likely as conservatives of any age to suffer from mental health disorders.
3. White liberals are almost twice as likely as non-white liberals to be diagnosed with mental health problems. 
4. Among conservatives of all ages, there is very little difference in the rates of mental disorders between whites and non-whites.

Liberals will, of course, throw out a flurry of excuses and say we're reading these number wrong. They'll say that liberals are more likely than conservatives to seek help for mental disorders. (There's no evidence of that, but they'll say it.)

They'll also say that non-whites lack access to mental health services. This is racist, of course. It's the same as saying, "non-white liberals are just as crazy as white liberals; they just haven't been diagnosed."

The fact remains that white liberals are twice as likely to have mental problems that conservatives. But we don't know the cause/effect relationship. 

Does mental illness lead people to become liberals, or does liberalism cause mental illness?

---
UPDATE: The comments by two readers expose a basic ignorance of how datasets work. Todd and Kathy were confused when they read Pew's narratives and did not find mention of these statistics. So I'll explain.

The statistics on the correlation between age, ideology, and race where created by a PhD student, Zach Goldberg, using Pew's Wave 64 datasets. Because Pew (and many other research firrms) publish their raw datasets for independent analysis, we can mine their data for insights that Pew did not produce.  You can [see Zach's excellent work here](https://threadreaderapp.com/thread/1248823584111439872.html). 

Researchers like Zach are a great boon to our knowledge base, and he's not alone. Much of our knowledge of medicine comes from anaysis done by independent researchers mining data from previous published reports. For example, about ten years ago, researchers discovered a strong correlation between regular aspirin use and exceptionally low incidence of skin, liver, and kidney cancer. The studies that produced the data for this research had nothing to do with either aspirin or cancer. Instead, those original studies simply collected data about the habits of subjects. 

The Pew study was focused on mental health effects of the COVID pandemic. It included a question about whether or not respondents had ever been diagnosed with mental illnes. Pew likely used this response to weight its statistics on COVID's effects. You would expect people with diagnosed mental illness to be emotionally more affected by a pandemic than people without mental illness.

Zach used Pew's quality data in a different way. He looked at the correlations between age, politicaly ideology, and race with respondents' histories of mental illness and produced new insights from existing data. Very efficient.

I replicated and confirmed Zach's findings using IBM's SPSS analytics software. You can, too, if you'd like and if you have some understanding of setting up crosstab analyses in a tool like SPSS. The [Pew datasets are available with a free account at this link](https://www.pewsocialtrends.org/dataset/covid-19-late-march-2020/). The data are in the file `ATP W64.sav`

A simple crosstab query to get started: 

```
CROSSTABS 
  /TABLES=F_AGECAT F_SEX BY F_IDEO BY COVID_MENTAL_W64 
  /FORMAT=AVALUE TABLES 
  /CELLS=COUNT 
  /COUNT ROUND CELL.
```

Have fun!