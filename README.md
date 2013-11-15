
# angular-seed-more — a seed for AngularFire apps

This project is a derivative application skeleton for an [AngularFire](http://angularfire.com/) web app.
It is a fork of the original angular-seed repo with some extra libs and
functionality that I commonly use in developing apps.
This library allows you to quickly bootstrap real-time apps using [Firebase](http://www.firebase.com) and [AngularJS](http://www.angularjs.org).

The seed contains AngularJS libraries, test libraries and a bunch of scripts all preconfigured for
instant web development gratification.  Additionally, Bootstrap is included and pre-wired in views.
Just clone the repo (or download the zip/tarball), start up our (or yours) webserver and you are ready to develop and test your application.

The seed app doesn't do much, just shows how to wire two controllers and views together. You can
check it out by opening app/index.html in your browser (might not work file `file://` scheme in
certain browsers, see note below).

_Note: While angular, angularFire, and Firebase can be used client-side-only, and it's possible to create
apps that don't require a backend server at all, we recommend hosting the project files using a local
webserver during development to avoid issues with security restrictions (sandbox) in browsers. The
sandbox implementation varies between browsers, but quite often prevents things like cookies, xhr,
etc to function properly when an html page is opened via `file://` scheme instead of `http://`._


## How to use this repo

 1. Clone the angularFire-seed repository
 1. Open app/js/config.js and add your Firebase URL
 1. Start hacking...


### Running the app during development

You can pick one of these options:

* serve this repository with your webserver
* install node.js and run `scripts/web-server.js`

Then navigate your browser to `http://localhost:<port>/app/index.html` to see the app running in
your browser.


### Running unit tests

We recommend using [jasmine](http://pivotal.github.com/jasmine/) and
[Karma](http://karma-runner.github.io) for your unit tests/specs, but you are free
to use whatever works for you.

Requires [node.js](http://nodejs.org/), Karma (`sudo npm install -g karma`) and a local
or remote browser.

* start `scripts/test.sh` (on windows: `scripts\test.bat`)
  * a browser will start and connect to the Karma server (Chrome is default browser, others can be captured by loading the same url as the one in Chrome or by changing the `config/karma.conf.js` file)
* to run or re-run tests just change any of your source or test javascript files


### End to end testing

Angular ships with a baked-in end-to-end test runner that understands angular, your app and allows
you to write your tests with jasmine-like BDD syntax.

Requires a webserver, node.js + `./scripts/web-server.js` or your backend server that hosts the angular static files.

Check out the
[end-to-end runner's documentation](http://docs.angularjs.org/guide/dev_guide.e2e-testing) for more
info.

* create your end-to-end tests in `test/e2e/scenarios.js`
* serve your project directory with your http/backend server or node.js + `scripts/web-server.js`
* to run do one of:
  * open `http://localhost:port/test/e2e/runner.html` in your browser
  * run the tests from console with [Karma](http://karma-runner.github.io) via
    `scripts/e2e-test.sh` or `script/e2e-test.bat`


## References

More information on AngularJS: http://angularjs.org/
More information on Firebase: http://firebase.com/
More information on AngularFire: http://angularfire.com/
More information on Bootstrap: http://getbootstrap.com/
