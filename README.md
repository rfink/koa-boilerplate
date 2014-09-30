## Koa-Boilerplate
### Usage Documentation

#### Purpose
The purpose of this project is to make it easier for an engineer to get
up-and-running with a koa (node.js >= v0.11.9) server app.  It makes sense
to have a quick spin-up process to take care of most of the plumbing for you,
so you can spend more time coding your actual app.

#### Usage
If you install this globally, you will only have to install it once.  The command
to install is:

```
    npm install -g git://github.com/rfink/koa-boilerplate.git
```

Now, assuming your global node_modules is in your $PATH, you should be able to use the
command "koa-boilerplate".  There's only one parameter: "--name".  This parameter
will be the name of the application you want to create.  It will be automatically
inserted into the package.json.

```
    koa-boilerplate --name=myapp
```

That's pretty much it.  We plan on updating this repo as new versions of koa are released,
and our release tags should mirror the versioning scheme of koa and its dependencies
(i.e. a minor version bump in either would cause a minor version bump in koa-boilerplate).

#### Contents
The koa app ships with the common dependencies needed for a typical app,
such as the session middleware, body-parser, compression, envcfg, connect-redis,
passport, connect-timeout, bunyan, cookie-parser, and redis.  It also has
dev dependencies for mocha/should for testing purposes, and jshint for coding standards.

We've tried to follow, as close as possible, to
[felixge's node style guide](https://github.com/felixge/node-style-guide) for the server app.

#### Contributing
If you want to contribute, please fork the repo, create a feature or bugfix branch,
commit your change, and submit a pull request with an appropriate description.
