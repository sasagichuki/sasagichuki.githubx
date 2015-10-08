---
layout: post
title: How moving to Jekyll saved me $140
date: 2015-10-09T00:00:00.000Z
last_modified_at: 2015-10-09T00:00:00.000Z
excerpt: How moving to Github pages and Jekyll saved me $140 in hosting costs.
categories: tech
tags: jekyll
image: 
  feature: jekyll.jpg
  topPosition: "-100px"
bgContrast: dark
bgGradientOpacity: darker
syntaxHighlighter: "no"
published: false
---



Who pays $140 to host a website, i did. I signed up for a Bluehost account millenia ago and diligently paid for my annual renewal every year (it seems that they dropped prices but kept charging me the same $11 per month ).

Most of the stuff i had on the server was experiemts, my portfolio, and a couple of clients

Stuff rarely changed and i was using only like 10% of my 10GB box (its now infinity). Every year i paid mostly because my personal page and blog were hosted there.

There was some real inertia, i did need to move... that is until my box got hacked, likely through my wordpress install or through my SSH access (very likely my fault ), i spent a weekend trying to clean it up but eventually i was very frustrated and just decided to close my Bluehost account for good (although i still had a whole year paid up)

It made a lot of sense anyway, my domain wasn't registered on Bluehost anyway

Wordpress is really difficult to use... it is so big, so detailed, i had really gotten tired of trying to figure out stuff, once i had even bought a theme but after mucking around trying to make it look exactly how i wanted... i gave up.

Then i met Ghost... i immediatley loved Ghost's cleaner user interface, simple templating and styling and Node JS geekyness... that why i used it at Ongair's Blog

Still to run Ghost you need a server that can run NODE, BlueHost can't.. technically it can (link) but it would take a lot of wrangling to get it working it did not meet my criteria. i Did not want to pay $20 a month just to write a blog.

You can use Digital Ocean... pay $20 or use AWS and host for free

I had played around with Jekyll and Github pages but i did not consider them as serious options.. until i tried

It's really easy to set up and there is a ton of good looking themes at (link)

After wrangling around with a few problems and other gotchas i was up and running

Also the templating language is easy to understand

Once my domain name propagated my hosting costs were $0

####Jekyll has a couple of advantages;

1. You use markdown to write you articles, no more struggling with databases and clucnky editors, you can write markdown straight into Github, you can also use Sublime text with a Markdown extension or something like Prose.io (i use all of them ) Markdown is easy to use, here is a detailed guide to the Syntax

2. Host for free on Github

3. If you like Git, then you will love working with Jekyll + Github Pages

4. Problems are easy to fix, no more fighting with Mamp or XXampp

5. 

I have a whole post on how i did the setup here (setting up Jekyll + GitHub pages)

I moved everything else to EAC directory, in my opinion a very good quality hosting company.

Jekyll rocks.