heroku-buildpack-mono-build
===========================

Clone the build repository:

    git clone https://github.com/brandur/heroku-buildpack-mono-build.git
    cd heroku-buildpack-mono-build.git

Create a Heroku app and store your secrets there:

    heroku create heroku-buildpack-mono-build --buildpack https://github.com/kennethreitz/buildpack-null.git
    heroku config:add AWS_ID="..." AWS_SECRET="..."

Now shell into your new app and kick off a build:

    heroku run bash
    bin/build
