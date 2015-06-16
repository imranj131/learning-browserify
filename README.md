# What is Browserify?
Check out:
* http://browserify.org/
* https://www.npmjs.com/package/browserify
* https://github.com/substack/browserify-handbook
* http://blakeembrey.com/articles/2013/09/introduction-to-browserify/

## Getting Started

Getting started with the browserify command-line tool requires node.js and npm installed.

        npm install browserify -g

As we have written a couple of modules that require each other, we can run browserify and generate the file for use in the browser:

        browserify index.js -o bundle.js

Now that we have a bundle.js file that bundled the three modules we wrote, we can add a single script tag reference to it into our html page and it'll execute in the browser automatically resolving require calls. 

        <script src="bundle.js"></script> 

and we should see 'Hello World!' logged to the JavaScript console of your browser.

