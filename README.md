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

1. Sign up and create an app on Webshell
By creating an app, you generate API Key for the Webshell API. You can configure hosts, and attach to this app some API Key for the API you are using.

2. Install the Javascript SDK
Insert this line in your HTML

    <script type="text/javascript" src="http://api.webshell.io/sdk/js?key={key}"></script>
     
3. Hello world app
In your Javascript you can now use the wsh object

    wsh.exec({
        code: function() {
            //Some javascript which have to be executed by Webshell
            apis.tts('hello world');
        },
        process: function(data, meta) {
            $('body').append(meta.view);
        }
    });
    
You can just call the Text to Speech API for, say, "Hello World". You can call lots of APIs like that and script them together directly in your JavaScript. Take a minute to visit our API Explorer to discover them!

4. Webshell Cloud Editor
To try and create your APIs directly in your browser to use them in the Webshell API. Go to the [API Editor](http://webshell.io/editor)

5. More
For more information on what you can do with Webshell, check the [Documentation](http://webshell.io/docs) and the [FAQ](http://webshell.io/docs/faq)
