Sketchfab API allow users to publish, search and embed 3D content without any plugins.

example:

`apis.sketchfab.embed('7irY67vcquhR4DCmPAUsSyxZWoC');`

or

<pre class="prettyprint">var data = apis.sketchfab.search('vader').result;
for (var i = 0; i < data.length; i++)
   apis.sketchfab.embed(data[i]);</pre>