# NPM Solo
A build system just using NPM. No Gulp or Grunt etc.

## Helpful NPM tips

Thanks to Bret Cameron for this article - [13 npm Tricks for Faster JavaScript Development](https://medium.com/@bretcameron/13-npm-tricks-for-faster-javascript-development-4fe2a83f87a2). It's primary targeted at JS development but there are definitely some take aways if JS isn't your focus.

Here are a few I've gleaned from his article that I found particularly helpful. For my needs anyhow:

* `npm i -D cross-env` - (Make Scripts Cross-Platform Compatible)
* `npm i -D concurrently` - (Run Scripts in Parallel)
* `npm i -g ntl` - (List and Select Available Scripts)
    - Then run the `ntl` command in the project folder. You’ll get a list of available scripts, with the option of selecting one of them to run.
