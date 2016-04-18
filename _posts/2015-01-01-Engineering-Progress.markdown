---
layout:     project
title:      "Engineering Progress"
subtitle:   "Engineering"
author:     "Neil Gordon"
date:       2015-01-01 12:00:00
---



<link rel="stylesheet" href="{{ "/css/skeleton.css" | prepend: site.baseurl }}">

<div id='root'></div>

<script src="{{ "/js/engineeringProgressBundle.js " | prepend: site.baseurl }}"></script>

<style>
	@media (max-width: 550px) {
	  .center-text {
	    text-align: center;
	  }
	}

	.full-screen {
	  position: fixed;
	  top: 0;
	  right: 0;
	  bottom: 0;
	  left: 0;
	}

	.header {
	  position: fixed;
	  top: 0;
	  right: 0;
	  left: 0;
	  height: 80px;
	}

	.main-body {
	  position: fixed;
	  top: 88px;
	  right: 0;
	  bottom: 0;
	  left: 0;
	  /*padding-top: 12px;*/
	}

	.entry:nth-child(even) {
	  background-color: #f2f2f2;
	}


	tr:nth-child(even) {
	  background-color: #f2f2f2;
	}

	td:first-child { padding-left: 6px; }
</style>