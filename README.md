# node-sass-pug

A simple starter project to help you get started with [Node](https://nodejs.org/), [Sass](http://sass-lang.com/), and [Pug](https://pugjs.org/). It does the following for you:

- Uses the `node-sass` and `pug-cli` modules to compile your Sass into CSS and your Pug into HTML, respectively.
- Uses the `live-server` module to run a simple local server that can live-reload on file changes.
- Uses the `postcss-cli` to post-process generated CSS to produce a production build (using the `autoprefixer` plugin to add prefixes and the `cssnano` plugin to optimize and minify).

All input files (`*.scss` and `*.pug`) live in the `src` directory, and all generated files (`*.css` and `*.html`) will end up in the `dist` directory. When running the commands below, everything in the `dist` directory will be wiped out and regenerated, so **be careful not to add files or make changes in the `dist` directory. Only work in the `src` directory.**

## Getting Started

First, make sure you've installed [npm](https://www.npmjs.com/get-npm). You can also use Yarn instead of npm, but the instructions below were written for npm (the Yarn equivalents are similar).

Next, clone this repo and install the Node dependencies:

```bash
git clone https://github.com/reid47/node-sass-pug.git some-directory

cd some-directory

npm i
```

## Developing

While developing, run the following to start up a local server at `localhost:8080` that will live-compile the `*.pug` and `*.scss` files in your `src` directory and live-reload your pages upon changes:

```bash
npm run watch
```

*NOTE: When you have added a new file, you will probably need to quit this process and restart it to pick up the new file.*

## Building for Production

When you're ready, run the following to produce a final set of compiled HTML and CSS files in the `dist` directory, with the CSS prefixed, optimized and minified:

```bash
npm run build
```
