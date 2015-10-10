---
layout: post
title: How moving to Jekyll saved me $120
date: 2015-10-09T00:00:00.000Z
last_modified_at: 2015-10-09T00:00:00.000Z
excerpt: How moving to Github pages and Jekyll saved me $120 in hosting costs.
categories: tech
tags: jekyll
image: 
  feature: jekyll.jpg
  topPosition: "-100px"
bgContrast: dark
bgGradientOpacity: darker
syntaxHighlighter: "no"
published: true
---


##Leaving Bluehost
I signed up for a Bluehost account in about 2007, a Millenia ago and diligently paid for my annual renewal every year (it seems that they dropped prices but kept charging me the same $10 per month ).

Most of the stuff I had on my box were experiments, my portfolio, and a couple of client sites. I was using only like 10% of my 10GB box (which they now upgraded to infinity).

I really had no reason to move… everything worked sort of okay, i got my emails, clicked around my cpanel and uploaded stuff with Filezilla… that is until my box got hacked, likely through my Wordpress install or through my pedestrian SSH access (very likely my fault ), I spent a weekend trying to clean it up but eventually I was so frustrated I just decided to close my Bluehost account for good (although i still had a whole year paid up).

I needed to a new home quickly, I needed a solution that would allow me to be up and running within an hour and that is how I ended up on Jekyll.

##Wordpress — the Heavy weight

I had began disliking how really Heavy weight Wordpress is, sometime you just want to write a story but then you find yourself swimming through a sea of plugins and configuration options you know… Jetpack, Akismet bla bla bla… it is so so big. Wordpress by it’s own admission is no longer a simple blogging platform, it not even a CMS…. Its a Web OS

> WordPress was first for pure blogging, then became embraced as a CMS (though some people still deny this), is seeing growth and innovation in being used as an application platform (I think we’re about a third of the way through that), and just now starting to embrace social and mobile — the fourth phase of our evolution.

–Matt Mullenweg, WordPress Founder, 2012

> I see the future of WordPress as a web operating system.

–Matt Mullenweg, WordPress Founder, 2013

Wordpress keeps all your content in an opaque database with very granular columns, just looking at your content with phpMyadmin can make your head spin. (Jekyll has a really neat meta section at the top… that’s it the rest of content is in static Markdown files)

Luckily did not feel like moving with any of the stuff i had written so far, i just wanted a clean slate “ You Know Nothing Chaos ”

I was very happy to leave Wordpress behind.

##Ghost — The Light weight

Termed the “Wordpress Killer” after the hype it’s Kickstarter campaign kicked up. I immediately loved Ghost’s cleaner user interface, simple templating and styling and Node JS geekyness… that why i used it on [Ongair’s Blog](http://blog.ongair.im/)

Still to run Ghost you need a server that can run Node.js and there not very many cheap options, BlueHost can’t.. technically it can but it would take a lot of wrangling to get it working. The fastest way to get onto Ghost is a $5/mo droplet on Digital Ocean $5 that i did not have to spend.

![envato.png]({{site.baseurl}}/_posts/envato.png)

Ghost is a very solid solution, even some big blogs have moved over to Ghost people like [Envato](http://inside.envato.com/).

##Enter the Octocat

![octocat and jekyll]({{site.baseurl}}/_posts/octo_cat.jpg)

I had played around with Jekyll and Github pages before, at the time it seemed a little Hackish and experimental, since i already had all my code on Github I decide to give Jekyll another try.

Github pages are really easy to set up

Getting started on Jekyll was not difficult, yes it’s not the famous 5 minute WP install but it is still simple enough. After wrangling around with a few problems and a couple of gotchas i was up and running.

Once my domain name propagated my hosting costs were $0

They are a couple of quick themes to get you started with Jekyll really fast, I like [Poole](http://getpoole.com/) by My Huge Nerd @mdo and there is a whole list of good looking [Jekyll themes here too](http://jekyllthemes.org/).

There are also some [easy tools](http://import.jekyllrb.com/docs/home/) to help you migrate your current blog over to Jekyll.

Jekyll is not a hobby platform either, [Obama care](https://www.healthcare.gov/) is an example of a large website built on Jekyll.

![Obama_care.png]({{site.baseurl}}/_posts/Obama_care.png)


###Jekyll has a couple of advantages;

1. You use markdown to write you articles, you can write markdown straight into Github, you can also use Sublime text with a Markdown extension or something like [Prose.io](http://prose.io/) (i use all of them ) Markdown is easy to use.

2. Host for free on Github.

3. If you like Git, then you will love working with Jekyll + Github Pages, in case you fat finger something you can always go back to your commit do a
	git diff 
and find out what you fudged, fix it and push an update.

4. No more databases, , or pesky updates to install , no just your content. Makes your site a lot faster since you are mostly serving up static files

5. Simplicity, No CMS to deal with, No Fat WYSIWYG editor to fight with. Simple backups. There is no funny plugin soup in the background doing something that you do not understand to 1 of you 200 .php files

6. Also running Jekyll on your machine is very easy, compared with all the hoops you have to jump through to get WP or Ghost running locally.

Jekyll’s [Blogging for Hackers Ethos](http://tom.preston-werner.com/2008/11/17/blogging-like-a-hacker.html) might make it a steep climb for some people but it’s advantages far outweigh the learning curve.

Jekyll rocks.

##Others
I also checked out [Harp.js](http://harpjs.com/) for 10 minutes.

##But Wait 
What about Medium 2.0, Medium is great but you have no control over your code etc. Though you can now get custom domains and an ugly logo.
***
