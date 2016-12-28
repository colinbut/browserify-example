# Browserify Example

#### What is Browserify?

By the definition goes by in the official Browserify website: http://browserify.org/


> Browserify lets you require('modules') in the browser by bundling up all of your dependencies.

In other words what seems to me is a tool that can combine multiple "resources/assets/files" into one single
file as a "bundle" which then allowing you to serve up in a single `<script>` tag.

An alternative to webpack?

#### Installation

```
npm install -g browserify
```

#### Bundle up a module

Apparently bundling a module is quite simple. Running Browserify to bundle multiple 'modules' into a 'bundle'.
For example, bundle multiple js files into one single js files.

1. Code up your required modules - (they might be using require method from nodejs, browsers don't have this method)
2. (remember to install the dependencies i.e. `npm install [dependency module]`)
3. run the following Browserify command:

assuming you have a javascript file called `main.js` ...

```
browserify main.js -o bundle.js
```

4. attach this output bundle into the html file using `<script></script>` tags.

above will bundle that into an output bundle called `bundle.js`
