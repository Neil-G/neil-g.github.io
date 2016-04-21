---
layout:     project
title:      "ThinkQuick! "
subtitle:   "Free-for-all real-time problem solving"
author:     "Neil Gordon"
date:       2016-02-01 12:00:00
---



<style>
	div.full-screen {
	  position: fixed;
	  top: 0;
	  right: 0;
	  bottom: 0;
	  left: 0;
	}

	div.game-container {
	  width: 100%;
	  background: white;
	  position: fixed;
	  top: 80px;
	  right: 0;
	  bottom: 0;
	  left: 0;
	}

	img.github-icon {
	  width: 25px;
	  height: 25px;
	  border-radius: 100px;
	  position: fixed;
	  top: 20px;
	  left: 12px;
	}

	p.instruction-box {
	  padding: 20px;
	  border: 1px solid gray;
	}

	button.play-button {
	  background: #43A047;
	  color: rgba(255,255,255, 0.85);
	  height: 60px;
	  border: 1px solid gray;
	}

	div.game-item-container {
	  width: 100%;
	  height: 20%;
	  overflow: hidden;
	  transition: all 0.5s;
	  position: relative;
	}

	.show-small {display: inline;}

	.float-left-on-small { right: 0px; }

	.login-box {
	  float: right; padding: 8px;
	  margin: 0; 
	  box-sizing: border-box; 
	  height: 100%; 
	  display: inline-block; 
	  max-width: 100%; 
	  overflow: hidden;
	}

	input.login {
	  width: 100px; 
	  box-sizing: border-box; 
	  height: 50px; 
	  border: 1px solid #CFD8DC; 
	  margin-right: 4px;
	}

	button.auth-submit {
	  border-radius: 0; 
	  background: #B9F6CA; 
	  height: 50px; 
	  border: 1px solid #CFD8DC; 
	  font-size: smaller;
	}

	button.logout {
	  margin-right: 10px; 
	  float: right; 
	  margin-top: 18px; 
	  background: tomato; 
	  color: white; 
	  border: 0px solid #E57373; 
	  font-weight: bold;
	}

	nav.nav-header {
	  border-radius: 0; 
	  margin: 0; 
	  overflow: hidden;
	  height: 80px; 
	  position: fixed; 
	  left: 0; 
	  right: 0; 
	  top: 0; 
	  padding: 0; 
	  border-bottom: 1px solid tomato; 
	  box-sizing: border-box;
	}

	.navbar-winner-toggle {
	  cursor: pointer;
	  color: gray; 
	  font-size: 80%; 
	  position: absolute; 
	  right: 8px; 
	}


	div.winners-column {
	  text-align: center; 
	  border-left: 1px solid gray; 
	  box-sizing: border-box;
	  transition: all 1s;
	  transform: scaleX(600px);
	  background: white; 
	  position: absolute; 
	  width: 40%; 
	  bottom: 0px; 
	  top: 80px;
	}

	div.winners-top-panel {
	  height: 100px; 
	  margin-top: 0; 
	  background: white; 
	  color: #EF9A9A; 
	  padding: 3%; 
	  position: absolute; 
	  width: 100%; 
	  background: #FFEBEE; 
	  border-bottom: 1px solid #CFD8DC;
	}

	.close-winners-column {
	  position: absolute; 
	  top: 2px; 
	  right: 4px;
	  color: tomato; 
	  cursor: pointer;
	}

	div.winners-column-container {
	  width: 100%; 
	  text-align: center; 
	  position: absolute; 
	  top: 100px;
	  bottom: 1px;
	  overflow-y: scroll;
	}


	table.winners-table {
	  width: 100%; 
	  text-align: center; 
	  position: absolute;
	  top: 0; 
	  bottom: 0; 
	  overflow-y: hidden;
	}


	/* Larger than mobile */
	@media (min-width: 400px) {}

	/* Larger than phablet (also point when grid becomes active) */
	@media (min-width: 550px) {

	  .navbar-winner-toggle {
	    bottom: 2px;
	  }

	  .color-swap-toggle {
	    left:0px;
	  }

	  .show-small {display: none;}
	}

	/* Larger than tablet */
	@media (min-width: 750px) {}

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
	  .navbar-winner-toggle { top: 2px; }

	  .color-swap-toggle {
	    right:0px;
	  }
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
