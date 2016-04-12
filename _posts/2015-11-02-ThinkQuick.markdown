---
layout:     project
title:      "ThinkQuick! "
subtitle:   "free-for-all real-time problem solving"
author:     "Neil Gordon"
date:       2015-11-02 12:00:00
---



<style>
	div.game-container {
	  width: 100%;
	}

	.show-small {display: inline;}

	.float-left-on-small { right: 0px; }


	/* Larger than mobile */
	@media (min-width: 400px) {
	  
	}

	/* Larger than phablet (also point when grid becomes active) */
	@media (min-width: 550px) {

	}

	/* Larger than tablet */
	@media (min-width: 750px) {
	  div.game-container {
	    width: 80%;
	  }
	  .show-small {display: none;}
	}

	/* Larger than desktop */
	@media (min-width: 1000px) {}

	/* Larger than Desktop HD */
	@media (min-width: 1200px) {}


	/* Smaller than mobile */
	@media (max-width: 400px) {}

	/* Smaller than phablet (also point when grid becomes active) */
	@media (max-width: 550px) {}

	/* Smaller than tablet */
	@media (max-width: 750px) {
	  .hide-small {
	    display: none;
	  }
	  .float-left-on-small { left: 4px; }
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
