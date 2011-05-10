The Cajoleit API Server provides an easy to use HTTP API for transforming  
raw JavaScript and CoffeeScript into "cajoled" code via [Google Caja]. See  
the docs for more info: [http://ampify.it/cajoleit.html]

**Installing Your Own Instance**

* Create a new application with [Google App Engine].

* Update `appengine.xml` with the application ID.

* Run `./install-deps` to grab the various dependencies.

* Run `ant runserver` to test that everything works in your local instance.

* Run `.appengine_java_sdk/bin/appcfg.sh update war` to deploy to a  
  production instance at App Engine.

**Upgrading The Dependencies**

To upgrade the downloaded dependencies, first remove the existing versions  
by running:

    ./install-deps --clean

And then just re-run `./install-deps`.

**Known Issues**

The situation with Java on OS X is pretty messed up. On older systems you  
might want to alias `ant` to force a specific `$JAVA_HOME`, e.g.

    JAVA_HOME=/System/Library/Frameworks/JavaVM.framework/Versions/1.6.0/Home ant

**Contribute**

To contribute any patches simply fork this repository using GitHub and send  
a pull request to me <<https://github.com/tav>>, thanks!

**License**

All of the Cajoleit code has been released into the [Public Domain]. Do with  
it as you please.

—  
Enjoy, tav <<tav@espians.com>>



[http://ampify.it/cajoleit.html]: http://ampify.it/cajoleit.html
[Google App Engine]: http://code.google.com/appengine/
[Google Caja]: http://code.google.com/p/google-caja/
[Public Domain]: https://github.com/tav/cajoleit/raw/master/UNLICENSE