---
layout: post
title:  "Popular Hello World Examples"
date:   2019-02-25 22:50:26 +0000
categories: programming stackoverflow popular example
---
Have you ever had the motivation to do something but didn’t know where to start?  This post came out of that same mental state.  Below is the starting place for the top 10 most popular languages in <a href="https://insights.stackoverflow.com/survey/2018/#most-popular-technologies">Stackoverflow’s annual survey</a> which had over 100,000 participants!  

<h2>Hello World in the {{ site.data.helloWorld | size }} most Popular Languages</h2>

{% for language in site.data.helloWorld %}

<a name="{{language.language_jekyll}}" href="#{{language.language_jekyll}}">{{language.language_pretty}}</a>
<p>{{language.blurb}}</p>
```{{language.language_jekyll}}
{{language.code}}
```
<h6>{{language.output}}</h6>

<br>
{% endfor %}