---
layout:     project
title:      "ThinkQuick! "
subtitle:   "Free-for-all real-time problem solving"
author:     "Neil Gordon"
date:       2016-02-01 12:00:00
---



<style>
	div.game-container {
	  width: 100%;
	}

	.show-small {display: inline;}

	.float-left-on-small { right: 0px; }

	.login-box {float: right; padding: 8px;}

	.show-border {border: 1px solid tomato; box-sizing: border-box;}


	/* Larger than mobile */
	@media (min-width: 400px) {
	  
	}

	/* Larger than phablet (also point when grid becomes active) */
	@media (min-width: 550px) {

	  .show-small {display: none;}
	}

	/* Larger than tablet */
	@media (min-width: 750px) {
	  div.game-container {
	    width: 100%;
	  }
	}

	/* Larger than desktop */
	@media (min-width: 1000px) {}

	/* Larger than Desktop HD */
	@media (min-width: 1200px) {}


	/* Smaller than mobile */
	@media (max-width: 400px) {}

	/* Smaller than phablet (also point when grid becomes active) */
	@media (max-width: 550px) {
	  .login-box { float: left; padding: 18px 8px 0px;}
	  .hide-small {display: none; }
	}

	/* Smaller than tablet */
	@media (max-width: 750px) {
	  .float-left-on-small { float: left; }
	}

	/* Smaller than desktop */
	@media (max-width: 1000px) {
	  .hide-mobile {
	    background: blue;
	    display: none;
	  }

	  .hide-medium {
	    display: none;
	  }
	  .show-medium { display: inline; }
	}

	/* Smaller than Desktop HD */
	@media (max-width: 1350px) {
	  .hide-large {display: none;}
	}
</style>
<div id='root'></div>
<script src="{{ "/js/thinkQuickBundle.js " | prepend: site.baseurl }}"></script>
