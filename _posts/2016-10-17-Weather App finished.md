---
layout: post
title: Weather Web App finished!

---

![Weather Web App]({{ site.baseurl }}/images/weatherapp.jpg)

So this is the second of Freecodecamp's intermediate projects and more or less uses the same concepts used to create the [quote machine](http://yasirsoulong.me/quote-machine/). The only different concept to be introduced was the use of a geolocation API. Now with this being said, Chrome's geolocation API is only accessible over an https connection as of [12PM PST April 20 2016](https://developers.google.com/web/updates/2016/04/geolocation-on-secure-contexts-only). This didn't apply to firefox, safari, and internet explorer, as API data can still be manipulated on those browsers. 

So to get around this and to make it compatible with all browsers, I (as well as many other campers) used an API that tracks down the location of the client's IP address. This then returns back a longitude and latitude that can be used with an actual weather API to find the current weather in your area. 

Some improvements that can be implemented to this project as of right now is to obtain a more accurate longitude and latitude. I have a gripe with Chrome's new policy as it forces me to use locations of IP addresses, which is undoubtedly unreliable giving me an incorrect longitude and latitude. This in turn gives me the wrong city the client is in, although it usually isn't far off. Here is an [article](https://www.techdirt.com/articles/20160413/12012834171/how-bad-are-geolocation-tools-really-really-bad.shtml) on how bad geolocation by IP is. 

Secondly, I want to load my button "Convert to Celcius!" at the same time all the data is retrieved from the weather api. Sometimes, the button will load before any information is displayed. This is due to me just using the jquery method .delay() and .show() and timing them as best as I can to be synced with data being displayed. 

To check out the project, click [here](http://yasirsoulong.me/weatherapp/).



