# NPM Solo

A build system just using NPM. No Gulp or Grunt etc.

---

**I'm not sure whether this is a ideal build config for larger projects. Maybe that's when *Gulp* is better**

---

## Things I want this build config to do

**Some of these have been completed now as can be seen in the `package.json` file**.

1. Templating language into HTML - (Handlebars, Nunjucks, Liquid...?)
2. SCSS compiling
3. CSS pre- or postprocessor
4. JavaScript Linting and Testing
5. ES6 transpiler
6. Dependency Management
7. JS Uglification
8. File watcher
9. Image minification

## Helpful NPM tips

Used these articles as a starter for ten:

* [gablaxian.com/blog/using-npm-as-a-build-tool](https://gablaxian.com/blog/using-npm-as-a-build-tool)
* [css-tricks.com/why-npm-scripts](https://css-tricks.com/why-npm-scripts/)

---

Thanks to Bret Cameron for this article - [13 npm Tricks for Faster JavaScript Development](https://medium.com/@bretcameron/13-npm-tricks-for-faster-javascript-development-4fe2a83f87a2). It's primary targeted at JS development but there are definitely some take-aways if JS isn't necessarily your focus.

Here are a few tips I've gleaned from his article that I found particularly helpful. For my needs anyhow:

* `npm install -g json` - (**Edit package.json from the Command Line**)
  * Then you can use it for in-place editing with -I . For example, to add a new script “foo” with the value “bar”, type: `json -I -f package.json -e 'this.scripts.foo="bar"'`
* `npm i -D cross-env` - (**Make Scripts Cross-Platform Compatible eg. for Windows users**)
* `npm i -D npm-run-all` - (**Run Scripts in Parallel**)
* `npm i -g ntl` - (**List and Select Available Scripts**)
  * Then run the `ntl` command in the project folder. You’ll get a list of available scripts, with the option of selecting one of them to run.

## Keeping NPM packages & dependencies up to date

[scotch.io/bar-talk/3-tools-to-keep-npm-packages-updated](https://scotch.io/bar-talk/3-tools-to-keep-npm-packages-updated)

* If you use VS Code, install the [Version Lens](https://marketplace.visualstudio.com/items?itemName=pflannery.vscode-versionlens) extension
* Install the [npm-check-updates](https://www.npmjs.com/package/npm-check-updates) CLI tool like this...  
  * `npm i -g npm-check-updates`
  * To use / run it, `ncu`
  * To update all the packages, `ncu -u`
  * To update a *specific* package, `ncu node-sass`

## Some interesting NPM packages

* `npm i -g pwainit` - [PWAinit](https://www.npmjs.com/package/pwainit)
