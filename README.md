Node.js layer for APIs
======================

JavaScript has long been the de facto standard for client-side APIs and mashups with Googlemaps, Youtube etc... While nearly all client API code is written in JavaScript, server-side APIs like Twitter or Facebook can be called in PHP, Python, Ruby, Java, and numerous other languages. Life as a web and mobile developer would be much simpler if a single language was used everywhere.

Because JavaScript dominates APIs in the browser , it makes sense to use it for server side APIs as well.

In the same way Node.js made Javascript the unique language to execute code server-side and client-side, Webshell, built on Node.js too, lets you call APIs with a single language : Javascript.

APIs
====

All APIs implemented in Webshell are here in Javascript.

Usage
=====

in [Webshell](http://webshell.io/prototype), you can try all these APIs online in really few lines of code :

`apis.google.maps();`

This command will search in google folder, pick the last version and execute maps/maps file. 

If you have an account on [Webshell](http://webshell.io/), you can setup your API Key by creating an apps in your [Dashboard](http://webshell.io/dashboard). All settings needed are specified in the `conf.json` file which allow us to generate a form to let you set your API Keys.

Note
====

Some builtins are used in their APIs are not describe on Webshell.io yet... We work on it ;)