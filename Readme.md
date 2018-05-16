# Heroku Buildpack for OpenCV (with Ruby/Bundler Multipack Flow)

This is a Notarize-flavored [Heroku Buildpack](http://devcenter.heroku.com/articles/buildpacks) for OpenCV, with an addition for the Bundler gemset manager used in the [heroku-buildpack-ruby flow](https://github.com/heroku/heroku-buildpack-ruby#flow).

Overall, this buildpack should help you use the [ruby-opencv](https://github.com/ruby-opencv/ruby-opencv) gem. If so, you should
- be using heroku multipacks
- use a CMake buildpack at some point, or modify this buildpack to also install CMake
- use a ruby/rails/bundler buildpack **_after_** this buildpack at some point

If you'd like to use OpenCV for other purposes, you should fork this buildpack and export any other path variables needed for other libraries to access OpenCV.
