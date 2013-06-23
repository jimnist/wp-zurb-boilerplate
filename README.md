wp-zurb-boilerplate
===================

NOTE - this is in-progress and might not work just right yet

TODO:
*  move contents of app.css to global.css or vice-versa

worpress site boilerplate with [zurb foundation 4](http://foundation.zurb.com/) sprinkled in

this is based on [this](https://github.com/inverse-paradox/boilerplate) repo, which is referenced in [John’s Windows WordPress Theme Development Workflow (now with SASS!)](http://www.inverseparadox.com/2013/05/johns-windows-wordpress-theme-development-workflow-now-with-sass/).

besides being on a mac, my development process would be similar, but a little different though. i would:

* start with this repo and make a new github repo for the project
* set up a local dev environment using:
  * [livereload](http://livereload.com/)
  * [compass](http://compass-style.org/) running in a terminal window to compile the scss. this implies Ruby so i have included a Gemfile so you can use [bundler](http://gembundler.com/). i also use [rvm](http://rvm.io/) and might even be using a [gemset](http://rvm.io/gemsets), but that's just me.
  * wordpress running locally via Apache
* generally work things out in the index.html
* convert to the index.php and other files
* set up a production server and deploy the site to it from github

from zurb install
====

*********************************************************************
Congratulations! Your compass project has been created.

You may now add and edit sass stylesheets in the sass subdirectory of your project.

Sass files beginning with an underscore are called partials and won't be
compiled to CSS, but they can be imported into other sass stylesheets.

You can configure your project by editing the config.rb configuration file.

You must compile your sass stylesheets into CSS when they change.
This can be done in one of the following ways:
  1. To compile on demand:
     compass compile [path/to/project]
  2. To monitor your project for changes and automatically recompile:
     compass watch [path/to/project]

More Resources:
  * Website: http://compass-style.org/
  * Sass: http://sass-lang.com
  * Community: http://groups.google.com/group/compass-users/



w00t! You're using ZURB Foundation, now go forth and rock 'n roll!


To import your new stylesheets add the following lines of HTML (or equivalent) to your webpage:
<head>
  <link href="/stylesheets/_normalize.css" rel="stylesheet" type="text/css" />
  <link href="/stylesheets/app.css" media="screen, projector, print" rel="stylesheet" type="text/css" />
<head>


