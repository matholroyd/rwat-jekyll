---
layout: default
categories: ruby
---

Below is bunch of notes and links to get you started with Ruby.

## Checking if you have Ruby installed

### Mac

If you bought a Mac in the last couple of years, chances are you already have Ruby installed. To check, open up a terminal (go to Spotlight and search for `terminal`. Alternatively in the **Applications** folder there should be a **Utilities** folder, and in that is the **Termainal** app). Once the terminal is open, type in `ruby --version`. If you see something like `ruby 1.8.7` then you're good to go.  Note if you have an older version of Ruby, e.g. 1.8.6, note that recent versions of Rails no longer support Ruby 1.8.6 or earlier. Since we will be using VirtualBox to run the workshop, you don't need to worry about this for now, just keep it in mind. 

### Linux

There's a chance Ruby is installed already. Open up a terminal and type `ruby --version` to check. If you get something back like `ruby 1.8.7` you are good to go.

### Windows

Windows does not come with Ruby, so it will need to be installed.


## Installing Ruby

There are a bunch of guides for Mac, Linux and Windows at [www.ruby-lang.org/en/downloads/](http://www.ruby-lang.org/en/downloads/). Rather then repeating them, you should just go there.

A word of warning though- if you are thinking of using RVM to install Ruby, note that I have had trouble getting RVM to setup Ruby properly on Linux. I have run into the problem several times where a *phatom* version of Ruby is still lurking on the system, and RVM has some how failed to update existing references to the old version of Ruby.  Other people swear by RVM though, and I actually use it on my Mac despite the trouble I have with it on Linux.

For Linux I prefer manually compiling it myself, and then manually updating the binary references (e.g. `/usr/bin/ruby`) myself if need be.




