Sketchfab API allow users to publish, search and embed 3D content without any plugins.

example:

`apis.sketchfab.embed('7irY67vcquhR4DCmPAUsSyxZWoC');`

or

<pre class="prettyprint">var data = apis.sketchfab.search('vader').result;
for (var i = 0; i < data.length; i++)
   apis.sketchfab.embed(data[i]);</pre>

Search
======

You can search 3D models on Sketchfab using `apis.sketchfab.search(params);`

<table class="table">
	<head>
		<th>Param</th>
		<th>Description</th>
		<th>Exemple</th>
	</thead>
	<tbody>
		<tr>
			<td>q</td>
			<td>the `q` parameter is the query with your keywords. if `params` is a string, this string is your query `q`. The query is <strong>not</strong> optionnal</td>
			<td><code>apis.sketchfab.search('iphone');</code></td>
		</tr>
		<tr>
			<td>count</td>
			<td>the number of search result you want. This parameter is optionnal</td>
			<td><code>apis.sketchfab.search({q: 'iphone', count: 2});</code></td>
		</tr>
		<tr>
			<td>detail</td>
			<td>By default, you don't have any detail about the model in the search result. You can set it to `full` </td>
			<td><code>apis.sketchfab.search({q: 'iphone', count: 2, detail: 'full'});</code></td>
		</tr>
	</tbody>
</table><br />

Embed
=====

You can easily embed Sketchfab's model into any page easily :

`apis.sketchfab.embed('7irY67vcquhR4DCmPAUsSyxZWoC');`

<table class="table">
	<head>
		<th>Param</th>
		<th>Description</th>
		<th>Exemple</th>
	</thead>
	<tbody>
		<tr>
			<td>id</td>
			<td>the `q` parameter is the query with your keywords. if `params` is a string, this string is your query `q`. The query is <strong>not</strong> optionnal</td>
			<td><code>apis.sketchfab.embed('7irY67vcquhR4DCmPAUsSyxZWoC');</code></td>
		</tr>
		<tr>
			<td>width</td>
			<td>The width of the iframe</td>
			<td><code>apis.sketchfab.embed({id: '7irY67vcquhR4DCmPAUsSyxZWoC', width: 650});</code></td>
		</tr>
		<tr>
			<td>height</td>
			<td>the height of the iframe</td>
			<td><code>apis.sketchfab.embed({id: '7irY67vcquhR4DCmPAUsSyxZWoC', width: 650, height: 300});</code></td>
		</tr>
	</tbody>
</table>
##Licence
Webshell APIs
Copyright (C) 2013 Webshell SAS

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
any later version.\n\n This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program. If not, see <http://www.gnu.org/licenses/>.

