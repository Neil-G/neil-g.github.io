---
layout:     post
title:      "ThinkQuick! blog post"
subtitle:   "instructions, thoughts, sketches"
date:       2015-10-31 12:00:00
author:     "Neil Gordon"
header-img: "img/post-bg-04.jpg"
---

<h2 class="section-heading">ThinkQuick! Basics</h2>

<p>ThinkQuick! gives you 5 simple arithmetic problems to solve at any given time. Each problem has three numbers and an operation.  If the operation is "ADD", then add the three numbers together, enter the answer in the top-right input box, and press "answer" button.  If the operation is "MULTIPLY," then multiply the numbers instead. If your submitted answer is correct -AND- you are the first to answer correctly, your username (or unknown if you are not logged in) gets added to the Winners column, and the solved problem gets reset.</p>

<h2 class="section-heading">It's a Race!</h2>
<p>This app is real time!  You are racing against anyone else trying to solve problems, and if they get the answer before you, they get the win.  And you get nada- but you can always get the next one.</p>

<h2 class="section-heading">SignUp, LogIn, and No Refreshes</h2>
<p>The page contains everything on a single page- what you see is what you get.  Even for logging in and signing up.  To SignUp or Login, enter a username and password.  If the username exists, the app will try to log you in.  If the username doesn't exist, the app will create the user and then log you in.  You can also just play as unknown (default username when you're not logged in), but then you won't get your props in the Winners column- boo.</p>

<h2 class="section-heading">Test it Out</h2>
<p>The App is best with 2 to 5 people playing simultaneously, but you can try out the real-time nature yourself by opening it up in two windows (or open one on your window and another on a mobile device) and playing against yourself.  You'll see both windows stay in sync as questions are answered in either one. </p>

<h2 class="section-heading">Closing Thoughts</h2>
<p>I freestyled this app over a weekend based on quizzes my first grade teacher used to give our class.  Of course the app didn't resemble those quizzes by the time it was done. My ideas were changing rapidly enough to make PropTypes and Testing impediments and far from being helpful.</p>
<p>I found making the app usable on mobile to be the hardest part by far. And not just the styling, but the functionality.  For example, on mobile, clicking on an input focuses, zooms in, and brings up a keyboard, which is just a clunky and not a fun way to use the app. Luckily since it's built with React, making a React Native mobile version might be a fun and viable solution.  The best solution, however, is to find better ways to make different kinds of apps responsive. </p>
<p>	In conclusion, I could tinker with this app forever, and in under a minute I could think of countless style changes and feature additions to improve it, but I think I'm going to leave this as is and focus on creating other (maybe similar) things, building on what I learned from ThinkQuick!. I'd definitely be open to making a tutorial if anyone is interested, so let me know! </p>


<p>The github repo for the React part of this project can be found at <a href="http://spaceipsum.com/">Space Ipsum</a>.</p>