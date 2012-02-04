---
title: REST Protocol And The Web
layout: default
categories: web
---
  
What is the web? A bunch of computers and other devices connected together on the Internet, sending webpages and other data back and forth. Lovely, we're all pretty used to it using browsers every day, but to build a web app yourself, you need a little grounding on what's actually going on behind the scenes.

Lets start with opening your browser and navigating to Google, and specifically looking at http://google.com/. First the browser says to the internet, "Give me the computer or device that responds to 'google.com'."  The domain name servers out on the Internet willing to do your browsers bidding and return with an IP address, e.g. "74.125.237.145". Now your browser is knows who to talk to, but first the two computers/devices + their software need to agree how to talk to each other.  By default, browsers want to talk to web servers via HTTP, which actually gets translated to a port number. Ports are used by computers to redirect connections to specific applications (piece of software). For instance a computer could be serving web pages + have an FTP server- the port number tells which piece of software should respond to a connection. These servers can run on any port, but to make common tasks on the Internet simple, a bunch of ports are standardised to correspond to common applications. For HTTP, the port number is 80, and HTTPS is port 443.

* Try navigation to "google.com:80" and "google.com:443".

Browser and web server are all ready to talk to each other, and the language they use is HTTP. HTTP is simply the  


Now, to plagerize in 30 secs a 30 minute talk Jim Webber give at YOW Melbourne 2011, HTTP is  


