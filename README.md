# Bootstrap 3 Boilerplate

Yet another boilerplate project for front end applications. Forked from [bootstrap-4-boilerplate](https://github.com/cwchentw/bootstrap-4-boilerplate).

## Note

This boilerplate project intends for tiny static sites with few pages. If you want to build a content website, see [Lightweight CMS](https://lightweightcms.org) instead.

## Technology Stacks

Main tools used during development:

* [Gulp](https://gulpjs.com/)
* [Nunjucks](https://mozilla.github.io/nunjucks/)
* [Sass](https://sass-lang.com/)
* [Autoprefixer](https://github.com/postcss/autoprefixer)
* [stylelint](https://stylelint.io/)
* [Babel](https://babeljs.io/)
* [Flow](https://flow.org/en/)
* [ESLint](https://eslint.org/)

Libraries used in the output:

* [Bootstrap 3](https://getbootstrap.com/docs/3.4/) and [Bootstrap.Native](http://thednp.github.io/bootstrap.native/)
* [Polyfill.io](https://polyfill.io/v3/)
* [HTML5 Shiv](https://github.com/aFarkas/html5shiv/)

## Usage

### Start a New Project

Clone this repo and install all tools:

```
$ git clone https://github.com/cwchentw/bootstrap-3-boilerplate.git
$ mv html-frontend-boilerplate myapp
$ cd myapp
$ npm install
```

After editing *myapp*, update the remote URL to save it to a new remote repo:

```
$ git remote set-url origin path/to/remote/repo
```

### Build a Project

Invoke this command to build a project:

```
$ npm run dev
```

The output will be in *public* directory. During development phase, all assets will keep pretty format.

### Live Code a Project

Invoke this command:

```
$ npm run watch
```

Visit the output at http://localhost:3000/ . While ediing the project. the output will be updated automatically.

### Publish a Project

Invoke this command to build a project for production environment:

```
$ npm run prod
```

The output will be in *public* directory. During production phase, all assets will be minified to save bandwidth.

Upload the content in *public* directory to a remote web server to publish this project.

## Note for Web Developers

You should **NOT** use the builtin error pages provided by your web server. Such pages usually reveal too many technical details. Instead, you should set redirecting rules and custom error pages for erroreous HTTP status codes.

In this boilerplate project, we provide a custom HTTP 404 error page. Nevertheless, the page works only on our development environment. You still need to set your own redirecting rules and custom error pages on your production environment.

## Note for Bootstrap.Native Users

The version `2.0.27` is the last version of Bootstrap.Native that supports Bootstrap 3. The project only supports Bootstrap 4 since the version `3.x`.

## See Also

This boilerplate project is largely inspired by [tonik/html-frontend-boilerplate](https://github.com/tonik/html-frontend-boilerplate).

Why re-inventing the wheel? That project didn't migrate to Gulp 4 yet as this repo was built. In addition, the project used [Rollup](https://rollupjs.org/guide/en/) as its bundler, which doesn't support multiple JavaScript files when combined with Gulp. Hence, I updated to Gulp 4, dropping Rollup to support multiple scripts in this repo.

## Copyright

Copyright 2020-2021, Michelle Chen. This repo itself is under [MIT license](http://opensource.org/licenses/MIT). Nevertheless, you may adopt it in your own project with any license you prefer.
