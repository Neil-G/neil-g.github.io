---
layout:     post
title:      "Scrollable Tables"
subtitle:   "I made a reusable component maybe..."
date:       2016-01-17 12:00:00
author:     " "
comments:   true
header-img: "img/post-bg-05.jpg"
---
<link rel="stylesheet" href="{{ "/css/skeleton.css" | prepend: site.baseurl }}">

<h2>Motivation</h2>
<p>Sometimes you have a table with a lot of items- more items than can fit on the screen or page vertically.  In this case, you have to create some type of scrollable table.<p>

<h2> Too Long </h2>
<table>
		<thead>
			<tr> <th>number</th><th>heading 1</th><th>heading 2</th><th>heading 3</th> </tr>
		</thead>
		<tbody>
			<tr> <td>1</td><td>column 1</td><td>column 2</td><td>column 3</td> </tr>	
			<tr> <td>2</td><td>column 1</td><td>column 2</td><td>column 3</td> </tr>	
			<tr> <td>3</td><td>column 1</td><td>column 2</td><td>column 3</td> </tr>	
			<tr> <td>4</td><td>column 1</td><td>column 2</td><td>column 3</td> </tr>	
			<tr> <td>5</td><td>column 1</td><td>column 2</td><td>column 3</td> </tr>	
			<tr> <td>6</td><td>column 1</td><td>column 2</td><td>column 3</td> </tr>	
			<tr> <td>7</td><td>column 1</td><td>column 2</td><td>column 3</td> </tr>	
			<tr> <td>8</td><td>column 1</td><td>column 2</td><td>column 3</td> </tr>	
			<tr> <td>9</td><td>column 1</td><td>column 2</td><td>column 3</td> </tr>	
			<tr> <td>10</td><td>column 1</td><td>column 2</td><td>column 3</td> </tr>	
			<tr> <td>11</td><td>column 1</td><td>column 2</td><td>column 3</td> </tr>	
			<tr> <td>12</td><td>column 1</td><td>column 2</td><td>column 3</td> </tr>	
			<tr> <td>13</td><td>column 1</td><td>column 2</td><td>column 3</td> </tr>	
			<tr> <td>14</td><td>column 1</td><td>column 2</td><td>column 3</td> </tr>	
			<tr> <td>15</td><td>column 1</td><td>column 2</td><td>column 3</td> </tr>	
			<tr> <td>16</td><td>column 1</td><td>column 2</td><td>column 3</td> </tr>	
			<tr> <td>17</td><td>column 1</td><td>column 2</td><td>column 3</td> </tr>	
			<tr> <td>18</td><td>column 1</td><td>column 2</td><td>column 3</td> </tr>	
			<tr> <td>19</td><td>column 1</td><td>column 2</td><td>column 3</td> </tr>	
			<tr> <td>20</td><td>column 1</td><td>column 2</td><td>column 3</td> </tr>	
		</tbody>
</table>
</hr>
<h3> headers and data are not aligned</h3>



<h2> Scrollable, but the Heading Disappears </h2>
<div class="header-disappear">
	<table>
			<thead>
				<tr> <th>number</th><th>heading 1</th><th>heading 2</th><th>heading 3</th> </tr>
			</thead>
			<tbody>
				<tr> <td>1</td><td>column 1</td><td>column 2</td><td>column 3</td> </tr>	
				<tr> <td>2</td><td>column 1</td><td>column 2</td><td>column 3</td> </tr>	
				<tr> <td>3</td><td>column 1</td><td>column 2</td><td>column 3</td> </tr>	
				<tr> <td>4</td><td>column 1</td><td>column 2</td><td>column 3</td> </tr>	
				<tr> <td>5</td><td>column 1</td><td>column 2</td><td>column 3</td> </tr>	
				<tr> <td>6</td><td>column 1</td><td>column 2</td><td>column 3</td> </tr>	
				<tr> <td>7</td><td>column 1</td><td>column 2</td><td>column 3</td> </tr>	
				<tr> <td>8</td><td>column 1</td><td>column 2</td><td>column 3</td> </tr>	
				<tr> <td>9</td><td>column 1</td><td>column 2</td><td>column 3</td> </tr>	
				<tr> <td>10</td><td>column 1</td><td>column 2</td><td>column 3</td> </tr>	
				<tr> <td>11</td><td>column 1</td><td>column 2</td><td>column 3</td> </tr>	
				<tr> <td>12</td><td>column 1</td><td>column 2</td><td>column 3</td> </tr>	
				<tr> <td>13</td><td>column 1</td><td>column 2</td><td>column 3</td> </tr>	
				<tr> <td>14</td><td>column 1</td><td>column 2</td><td>column 3</td> </tr>	
				<tr> <td>15</td><td>column 1</td><td>column 2</td><td>column 3</td> </tr>	
				<tr> <td>16</td><td>column 1</td><td>column 2</td><td>column 3</td> </tr>	
				<tr> <td>17</td><td>column 1</td><td>column 2</td><td>column 3</td> </tr>	
				<tr> <td>18</td><td>column 1</td><td>column 2</td><td>column 3</td> </tr>	
				<tr> <td>19</td><td>column 1</td><td>column 2</td><td>column 3</td> </tr>	
				<tr> <td>20</td><td>column 1</td><td>column 2</td><td>column 3</td> </tr>		
			</tbody>
	</table>
</div>


<h2> Solution 1: sticky headers </h2>

<table class="header-remain-fixed-1">
		<thead class="header-remain-fixed-1">
			<tr> <th>number</th><th>heading 1</th><th>heading 2</th><th>heading 3</th><th style="width:20px"></th> </tr>
		</thead>
		<tbody class="header-remain-fixed-1">
			<tr> <td>1</td><td>column 1</td><td>column 2</td><td>column 3</td> </tr>	
			<tr> <td>2</td><td>column 1</td><td>column 2</td><td>column 3</td> </tr>	
			<tr> <td>3</td><td>column 1</td><td>column 2</td><td>column 3</td> </tr>	
			<tr> <td>4</td><td>column 1</td><td>column 2</td><td>column 3</td> </tr>	
			<tr> <td>5</td><td>column 1</td><td>column 2</td><td>column 3</td> </tr>	
			<tr> <td>6</td><td>column 1</td><td>column 2</td><td>column 3</td> </tr>	
			<tr> <td>7</td><td>column 1</td><td>column 2</td><td>column 3</td> </tr>	
			<tr> <td>8</td><td>column 1</td><td>column 2</td><td>column 3</td> </tr>	
			<tr> <td>9</td><td>column 1</td><td>column 2</td><td>column 3</td> </tr>	
			<tr> <td>10</td><td>column 1</td><td>column 2</td><td>column 3</td> </tr>	
			<tr> <td>11</td><td>column 1</td><td>column 2</td><td>column 3</td> </tr>	
			<tr> <td>12</td><td>column 1</td><td>column 2</td><td>column 3</td> </tr>	
			<tr> <td>13</td><td>column 1</td><td>column 2</td><td>column 3</td> </tr>	
			<tr> <td>14</td><td>column 1</td><td>column 2</td><td>column 3</td> </tr>	
			<tr> <td>15</td><td>column 1</td><td>column 2</td><td>column 3</td> </tr>	
			<tr> <td>16</td><td>column 1</td><td>column 2</td><td>column 3</td> </tr>	
			<tr> <td>17</td><td>column 1</td><td>column 2</td><td>column 3</td> </tr>	
			<tr> <td>18</td><td>column 1</td><td>column 2</td><td>column 3</td> </tr>	
			<tr> <td>19</td><td>column 1</td><td>column 2</td><td>column 3</td> </tr>	
			<tr> <td>20</td><td>column 1</td><td>column 2</td><td>column 3</td> </tr>		
		</tbody>
</table>

<h2> Solution 2: sticky headers w/ fixed adjustments </h2>

<table class="header-remain-fixed-1">
		<thead class="header-remain-fixed-1">
			<tr> <th style="width:50px">#</th><th style="width:150px">heading 1</th><th style="width:200px"> heading 2</th><th style="width:200px">heading 3</th> </tr>
		</thead>
		<tbody class="header-remain-fixed-1">
			<tr> <td style="width:50px">1</td><td style="width:150px">column 1</td><td style="width:200px">column 2</td><td style="width:185px">column 3</td> </tr>	
			<tr> <td>2</td><td>WarrenNeil</td><td>column 2</td><td>column 3</td> </tr>	
			<tr> <td>3</td><td>column 1</td><td>column 2</td><td>column 3</td> </tr>	
			<tr> <td>4</td><td>column 1</td><td>column 2</td><td>column 3</td> </tr>	
			<tr> <td>5</td><td>column 1</td><td>column 2</td><td>column 3</td> </tr>	
			<tr> <td>6</td><td>column 1</td><td>column 2</td><td>column 3</td> </tr>	
			<tr> <td>7</td><td>column 1</td><td>column 2</td><td>column 3</td> </tr>	
			<tr> <td>8</td><td>column 1</td><td>column 2</td><td>column 3</td> </tr>	
			<tr> <td>9</td><td>column 1</td><td>column 2</td><td>column 3</td> </tr>	
			<tr> <td>10</td><td>column 1</td><td>column 2</td><td>column 3</td> </tr>	
			<tr> <td>11</td><td>column 1</td><td>column 2</td><td>column 3</td> </tr>	
			<tr> <td>12</td><td>column 1</td><td>column 2</td><td>column 3</td> </tr>	
			<tr> <td>13</td><td>column 1</td><td>column 2</td><td>column 3</td> </tr>	
			<tr> <td>14</td><td>column 1</td><td>column 2</td><td>column 3</td> </tr>	
			<tr> <td>15</td><td>column 1</td><td>column 2</td><td>column 3</td> </tr>	
			<tr> <td>16</td><td>column 1</td><td>column 2</td><td>column 3</td> </tr>	
			<tr> <td>17</td><td>column 1</td><td>column 2</td><td>column 3</td> </tr>	
			<tr> <td>18</td><td>column 1</td><td>column 2</td><td>column 3</td> </tr>	
			<tr> <td>19</td><td>column 1</td><td>column 2</td><td>column 3</td> </tr>	
			<tr> <td>20</td><td>column 1</td><td>column 2</td><td>column 3</td> </tr>		
		</tbody>
</table>




<style>
.header-disappear {
	height: 200px;
	overflow-y: scroll;
}

/* SOLUTION 1*/

table.header-remain-fixed-1 {
	width: 600px;
}

thead.header-remain-fixed-1 {
	display: block;
	background-color: black;
	color:tomato;
}

tbody.header-remain-fixed-1 {
	display: block;
	height: 300px; 
	overflow-y:scroll;
}

/* SOLUTION 2*/



</style>