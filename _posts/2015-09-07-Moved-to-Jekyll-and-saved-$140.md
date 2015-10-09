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

##Bluehost
First, Who pays $140 to host a website ? I did. I signed up for a Bluehost account in 2007, a millenia ago and diligently paid for my annual renewal every year (it seems that they dropped prices but kept charging me the same $9 per month ).

Most of the stuff i had on the server was experiemts, my portfolio, and a couple of sites i did for clients.

Stuff rarely changed or grew and i was using only like 10% of my 10GB box (which they now upgraded to infinity). I kepy it running mostly because my personal site and blog were hosted there.

I really had no reason to move... everything worked sort of okay, i got my emails, clicked around my cpanel and uploaded stuff with Filezilla... that is until my box got hacked, likely through my wordpress install or through my SSH access (very likely my fault ), I spent a weekend trying to clean it up but eventually i was very frustrated and just decided to close my Bluehost account for good (although i still had a whole year paid up).

##Wordpress is powerful

I was begin to dislike how really Heavy weight Wordpress is, sometime you just want to write a story but then you find yourself swimming through a sea of plugins and configuration options you know... Jetpack, Akismet bla bla bla... it is so so big, The WYSIWYG editor can really spit out bloated HTML. Once i had even bought a theme but after much mucking around trying to make it look exactly how i wanted... i gave up.

Luckily did not feel like moving with any of the stuff i had written so far, i just wanted a clean slate " You Know Nothing Chaos "

Wordpress keeps all your content in this opaque database that only a machine can read with very granular columns (Jekyll has a really neat meta section at the top... that's it )

##Tried a Ghost

Then i met Ghost... i immediatley loved Ghost's cleaner user interface, simple templating and styling and Node JS geekyness... that why i used it on [Ongair's Blog](http://blog.ongair.im/)

Still to run Ghost you need a server that can run NODE, BlueHost can't.. technically it can (link) but it would take a lot of wrangling to get it working it did not meet my criteria. i Did not want to pay $20 a month just to write a blog.

You can use Digital Ocean... pay $20 or use AWS and host for free but AWS is not free forever

##Enter the Octocat

![octocat and jekyll]({{site.baseurl}}/_posts/octo_cat.jpg)

I had played around with Jekyll and Github pages but i did not consider them as serious options.. until i tried

It's really easy to set up and there is a ton of good looking themes at (link)

After wrangling around with a few problems and other gotchas i was up and running

Also the templating language is easy to understand

Once my domain name propagated my hosting costs were $0

They are a couple of quick themes to get you started with Jekyll popular ones are Poole, Hyde and  by @mdo but there is a whole list of them over at (link)

More on how to get started here

There are some easy tools to help you migrate your current blog over to Jekyll, there are list here 

[Jekyll Importers](http://import.jekyllrb.com/docs/home/ "Jekyll Importers")

####Jekyll has a couple of advantages;

1. You use markdown to write you articles, no more struggling with databases and clucnky editors, you can write markdown straight into Github, you can also use Sublime text with a Markdown extension or something like Prose.io (i use all of them ) Markdown is easy to use, here is a detailed guide to the Syntax

2. Host for free on Github, you dont have to deal with any hosting

3. If you like Git, then you will love working with Jekyll + Github Pages, in case you fat finger something you can always go back to your commit do a

    git diff
    
and find out what you fudged.

4. Problems are easy to fix, no more fighting with Mamp or XXampp

5. No more databases, comment moderation, or pesky updates to install—just your content. Makes your site a lot faster as there are no database calls to make, you make very few calls since you are mostly serving up static files

6. No CMS to deal with ... Simplicity, Simple backups, Simple clear syntax... simple, there is no funny plugin in the background doing something that you do not understand to 1 of you 200 .php files

I'll do a more detailed post on how i did the whole setup.

I moved everything else to EAC directory, in my opinion a very good quality hosting company.

I have to admit Jekyll is not for everyone, it's [Blogging for Hackers Ethos](http://tom.preston-werner.com/2008/11/17/blogging-like-a-hacker.html) might make it a steep climb for most people but it's advatages far outweigh the ccost, it's not the famous 5 minutes deploy for Wordpress but Jekyll rocks.

Jekyll is not a microframework either, you can build large websites on top of it, like Obama care [healthcare.gov/](https://www.healthcare.gov/)
