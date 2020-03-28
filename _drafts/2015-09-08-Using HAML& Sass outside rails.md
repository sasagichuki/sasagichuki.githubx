---
published: false
layout: post
date: 2015-10-09T00:00:00.000Z
last_modified_at: 2015-10-09T00:00:00.000Z
excerpt: Example excerpt.
categories: tech
tags: jekyll
image:
  feature: jekyll.jpg
  topPosition: '-100px'
bgContrast: dark
bgGradientOpacity: darker
syntaxHighlighter: 'no'
---

## HAML & SASS

HAML, CoffeeScript, & Sass are 3 wonderful tools that make the life of your neighborhood front-end developer much easier. Think of them as shorthand mark-up for HTML, Javascript, & CSS respectively. Since this post isn’t about the pros and cons of each, I won’t dive into their syntax. However here’s a comparison for demonstration purposes:

HAML


!!! 5
              %html{lang: 'en'}
                %head
                  %title Demo Page
                %body
                  %h1 Why should I use HAML?
                  %ol
                    %li It's much easier on the eyes.
                    %li You'll type less.
                    %li You can embed Ruby and/or Rails commands.
HTML


<!DOCTYPE html>
              <html lang='en'>
                <head>
                  <title>Demo Page</title>
                </head>
                <body>
                  <h1>Why should I use HAML?</h1>
                  <ol>
                    <li>It's much easier on the eyes.</li>
                    <li>You'll type less.</li>
                    <li>You can embed Ruby and/or Rails commands.</li>
                  </ol>
                </body>
              </html>
How do I use them?

(Note: do not include the brackets “[]” in your code, they're for demonstration purposes only)

Deploying any of the 3 in Rails is fantastically easy, assuming you are using OSX, and can be done in 3 steps.

Open "Gemfile" and add "gem [name of gem, ex. 'haml']" (note: Sass is included by default)
In terminal, while inside of the rails app directory, type 'bundle' & hit 'return'
Add .haml, .scss, or .coffee to the end of the file extension (e.g. index.html.haml)
Start using the language you choose
How to use them without creating a Rails application.

The easiest of the 3 to get running seems to be CoffeeScript. If you install Node.js, you're also given the ability to compile it to Javascript on demand. To do so, run "coffee –compile [filename]" in Terminal. If you'd rather CoffeeScript compiled every time you saved the document, use "coffee –watch [filename]" to do so.

That takes care of CoffeeScript, on to Sass.

Sass has a bit of a different syntax than HAML. To use it, you’ll need to install the Sass Gem by running “gem install sass” in Terminal. Run “sass –update [input-filename.scss]:[output-filename.css]” to compile a single file. If you'd like to watch a file or directory and automatically compile just run “sass –watch [name of file or directory]” to have sass update everything automatically.

This seems too easy. How about Haml?

Unfortunately HAML doesn't have the same "watch" compiling feature that CoffeeScript enjoys by default (as of version 3.1.6 "Separated Sally"). However, if you can compile a single file.

To run HAML from the command line, you'll need to have the HAML Ruby Gem installed. To do so run "gem install haml" from the command line. You can compile a file in Terminal by running "haml [input-filename.haml] [output-filename.html]" to output the single file.

Isn't there an easier way to do this?

Yes. In fact, I recommend buying CodeKit for 20 bucks and letting it do all of the hard work. It will compile all 3 formats (and more), then refresh your browser window every time an update happens.


There is another tool, called LiveReload, that has a very similar set of features. However, I would advise caution before putting down the $10 for this app. The commentors in Apple's App Store have pointed out that the current version (2.2.2) is buggy. PowrDev2000 may have said it best, "I like the software when its working, it's great but it crashes way to often to be useful now …"
