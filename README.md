wp-zurb-boilerplate
===================

worpress site boilerplate with [zurb foundation 4](http://foundation.zurb.com/) sprinkled in

this is based on [this](https://github.com/inverse-paradox/boilerplate) repo, which is referenced in [John’s Windows WordPress Theme Development Workflow (now with SASS!)](http://www.inverseparadox.com/2013/05/johns-windows-wordpress-theme-development-workflow-now-with-sass/).

besides being on a mac, my development process would be similar, but a little different though. i would:

* start with this repo and make a new github repo for the project
* set up a local dev environment using:
  * [livereload](http://livereload.com/)
  * [compass](http://compass-style.org/) running in a terminal window to compile the scss
  * wordpress running locally via Apache
* generally work things out in the index.html
* convert to the index.php and other files
* set up a production server and deploy the site to it from github
