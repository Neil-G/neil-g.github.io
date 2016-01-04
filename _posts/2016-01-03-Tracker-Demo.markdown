---
layout:     project
title:      "Tracker Demo"
subtitle:   "Demo"
author:     "Neil Gordon"
date:       2016-01-03 12:00:00
---

<style type="text/css">
  .vis-item.vis-background.test {
    background-color: rgba(0, 200, 0, 0.2);
    background: linear-gradient(to right, rgba(0, 200, 0, 0.6), rgba(0, 200, 0, 0.4) 25%,rgba(0, 200, 0, 0.1))
  }
  div.bootstrap-datetimepicker.dropdown-menu.bottom.pull-right {
    position: fixed;
  }
</style>

<link rel="stylesheet" href="{{ "/css/vis.min.css" | prepend: site.baseurl }}">
<link rel="stylesheet" href="{{ "/css/bootstrap-datetimepicker.css" | prepend: site.baseurl }}">
<link rel="stylesheet" href="{{ "/css/skeleton.css" | prepend: site.baseurl }}">

<div id='root'></div>

<script src="{{ "/js/trackerBundle.js " | prepend: site.baseurl }}"></script>

<style>
	@media (max-width: 550px) {
	  .center-text {
	    text-align: center;
	  }
	}
</style>