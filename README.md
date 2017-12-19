# node-sass-pug

A repo to get started with Node, Sass, and Pug. It does the following for you:

- Uses the `node-sass` and `pug-cli` modules to compile your Sass into CSS and your Pug into HTML, respectively.
- Uses the `live-server` module to run a simple local server that can live-reload on file changes.
- Uses the `postcss-cli` to post-process generated CSS to produce a production build (using the `autoprefixer` plugin to add prefixes and the `cssnano` plugin to optimize and minify).

All input files (`*.scss` and `*.pug`) should live in the `src` directory, and all generated files (`*.css` and `*.html`) will end up in the `dist` directory.

## Developing

1. Make sure you've installed Node and either npm or Yarn.

2. Clone this repo:

```bash
git clone https://github.com/reid47/node-sass-pug.git some-directory

cd some-directory
```

3. Install Node dependencies:

If using npm:
```bash
npm i
```

If using Yarn:
```bash
yarn
```

4. While developing, run the following to start up a local server at `localhost:8080` that will live-compile the `*.pug` and `*.scss` files in your `src` directory and live-reload your pages upon changes:

If using npm:

```bash
npm run watch
```

If using Yarn:

```bash
yarn run watch
```

5. When you're ready, run the following to produce a final set of compiled HTML and CSS files in the `dist` directory, with the CSS prefixed, optimized and minified:

If using npm:

```bash
npm run build
```

If using Yarn:

```bash
yarn run build
```

## Publishing/distributing

