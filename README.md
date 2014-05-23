dokku-bower-install
===================

Dokku pluging to install bower dependecies.

*NOTE*: it's developed and tested on the latest `progrium/buildstep` which uses the latest `heroku-buildpack-nodejs`.

To install the lastest build step, you should remove the existing one and run,

```
$ docker build -t progrium/buildstep github.com/progrium/buildstep
```

## Description

This plugin will inject the `/app/.bower` shell script that's going to be executed on the `pre-deploy` stage. If the root of the application contains a `bower.json` file, then bower and all dependencies are installed.

## Usage

```
git clone https://github.com/timsuchanek/dokku-bower-gulp-install.git /var/lib/dokku/plugins
sudo dokku plugins-install
```

Push your app.

# License

MIT
