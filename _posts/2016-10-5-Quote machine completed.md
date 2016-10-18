---
layout: post
title: Quote Machine Completed!

---

![quote-machine]({{ site.baseurl }}/images/quote-machine.png)

So this is the first project I have been working on for about a week based on Freecodecamp's Intermediate challenges, and it involved retrieving JSON objects (really JSONP to bypass origin problems) from an API, and using dot notation to access the object's keys and values to display quotes on the page. 

I did this using Jquery's getJSON method, and manipulated the API's query parameters to format the quotes into english and into JSON format (because the API can put it Russian and in HTML, XML, etc.). Furthermore, quotes can be tweeted when clicking the "tweet it!" button, with the quote in quotes, and the author of the quote being hashtaged. This was done by manipulating Twitter's url query parameters to show text and the author of the quote. 

The only improvements I do want to implement in the future (other than cleaning up my ugly js code) is to figure out why semicolons stop the completion mid-sentence when tweeted. For example, if a quote said "For those that are weary, be especially careful; they are not really weary at all...", when clicking the "tweet it!" button, the quote would only display "For those that are weary, be especially careful" in Twitter's text box. 

You can check it out by clicking right [here](http://yasirsoulong.me/quote-machine/).