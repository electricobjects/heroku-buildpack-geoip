Heroku buildpack: GeoIP (Legacy)
=======================

This is a [Heroku buildpack](http://devcenter.heroku.com/articles/buildpacks) for installing [MaxMind's GeoIP](http://dev.maxmind.com/geoip/legacy/downloadable/) Legacy C library.

Usage
-----

Example usage:

```
# to create a new heroku app with this buildpack
$ heroku create --stack cedar --buildpack https://github.com/electricobjects/heroku-buildpack-geoip.git

# or if your app is already created
$ heroku config:add BUILDPACK_URL=https://github.com/electricobjects/heroku-buildpack-geoip.git
$ git push heroku master
```

You may need to enable Multiple Buildpacks.  See more information [here](https://devcenter.heroku.com/articles/using-multiple-buildpacks-for-an-app).
