# Deep playground

Deep playground is an interactive visualization of neural networks, written in TypeScript using d3.js.
We use GitHub issues for tracking new requests and bugs. Your feedback is highly appreciated!

**If you'd like to contribute, be sure to review the [contribution
guidelines](CONTRIBUTING.md).**

## Development

To run the visualization locally you just need a server to serve all the files from the `dist` directory. You can run `npm install` then `npm run serve` if you don't have one handy. To see the visualization, visit `http://localhost:8080/` on your browser.

When developing, use `npm run serve-watch`. This will start a static server and also watchers to automatically compile the TypeScript, HTML and CSS files
whenever they change.

To produce a minified JavaScript file for production, run `npm run build`.

To push to production: `git subtree push --prefix dist origin gh-pages`.

This is not an official Google product.


## Note

Inspiring packages used in this project:

* catw: concatenate file globs, watching for changes.

* concurrently: run multiple commands concurrently.
    * Cross platform (including Windows)
    * Output is easy to follow with prefixes
    * With --kill-others switch, all commands are killed if one dies
    * Spawns commands with spawn-command

* copyfiles: copyfiles [options] inFile [more files ...] outDirectory.
    * -h, --help               output usage information
    * -V, --version            output the version number
    * -u, --up [levels]        slice a path off the bottom of the paths
    * -a --all                 include files and directories whose names begin with a dot (.)
    * -f, --flat               flatten the output
    * -e, --exclude [pattern]  pattern or glob to exclude
    * -s, --soft               do not overwrite destination files if they exist

* live-server:
    * AJAX requests don't work with the file:// protocol due to security restrictions, i.e. you need a server if your site fetches content through JavaScript.
    * Having the page reload automatically after changes to files can accelerate development.

* rimraf: the UNIX command rm -rf for node.

* typings: setting in typings.json; deprecated, now use @types

* uglify-js: to minify ECMAScript 2015 or above use Babel instead

* tsify: browserify plugin for compiling TypeScript.

* watchify: watch mode for browserify builds; update any source file and your browserify bundle will be recompiled on the spot.

## Todo

* find another method to replace `typings install` in package.json, or to use es6+ and Babel to displace typings & uglify-js

