wp-zurb-boilerplate
===================

worpress site boilerplate with [zurb foundation 4](http://foundation.zurb.com/) sprinkled in

this is based on [this](https://github.com/inverse-paradox/boilerplate) repo, which is referenced in [John’s Windows WordPress Theme Development Workflow (now with SASS!)](http://www.inverseparadox.com/2013/05/johns-windows-wordpress-theme-development-workflow-now-with-sass/).

besides being on a mac, my development process would be similar, but a little different though. i would:

* start with this repo and make a new github repo for the project
* set up a local dev environment using:
  * [livereload](http://livereload.com/)
  * [compass](http://compass-style.org/) running in a terminal window to compile the scss. this implies Ruby so i have included a Gemfile so you can use [bundler](http://gembundler.com/). i also use [rvm](http://rvm.io/) and might even be using a [gemset](http://rvm.io/gemsets), but that's just me.
  * wordpress running locally via Apache ([this](http://rzen.net/development/local-develoment-in-osx/) is not exactly how i'd do it . . but it's close)
* generally work things out in the index.html
* convert to the index.php and other files
* set up a production server and deploy the site to it from github


install wordpress locally, then link your local theme working directory under the wordpress install's theme directory

```
$ ln -s ~/wrk/personal/wp-zurb-boilerplate ~/wrk/personal/wordpress/wp-content/themes/wp-zurb-boilerplate
```


apache virtual host config:

```
<VirtualHost *:80>
    ServerAdmin bobo@example.com
    DocumentRoot "/Users/bobo/wrk/wordpress"
    ServerName staengl.dev
    ServerAlias *.staengl.dev
    ErrorLog "/private/var/log/apache2/bobo-error_log"
    CustomLog "/private/var/log/apache2/bobo-access_log" common
    <Directory "/Users/bobo/wrk/wordpress">
       AllowOverride All
       Options FollowSymlinks Indexes MultiViews
       Order allow,deny
       Allow from 127.0.0.1
    </Directory>
</VirtualHost>
```


TODO:

* style index.php
* add screenshot.png
* style 404 with zurb layout css? or is that the same as notfound.php?