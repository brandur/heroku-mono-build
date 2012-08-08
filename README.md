heroku-buildpack-mono-build
===========================

Builds the Heroku Mono buildpack via Anvil.

Store your secrets to the environment of a Heroku app:

    heroku create heroku-buildpack-mono-build --buildpack https://github.com/kennethreitz/buildpack-null.git
    heroku config:add AWS_ID="..." AWS_SECRET="..." -a heroku-buildpack-mono-build

Now shell in and kick off a build:

    heroku run -a heroku-buildpack-mono-build bash
    bin/build
