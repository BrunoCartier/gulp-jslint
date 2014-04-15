# gulp-jslint [![Build Status](https://travis-ci.org/karimsa/gulp-jslint.svg?branch=master)](https://travis-ci.org/karimsa/gulp-jslint)
It's JSLint for Gulp.js.

[![NPM](https://nodei.co/npm/gulp-jslint.png?downloads=true&stars=true)](https://nodei.co/npm/gulp-jslint/)

## Usage

To install with npm, simply do:

```
$ npm install gulp-jslint
```

Sample Gulpfile.js:

```
var gulp = require('gulp');
var jslint = require('gulp-jslint');
var uglify = require('gulp-uglify');

gulp.task('default', function () {
    return gulp.src(['my_files.js'])
            .pipe(jslint(/* pass all directives as an object here */))
            .pipe(uglify())
            .pipe(gulp.dest('built'));
});
```

## Custom Install
To build from source, simply do the following:

```
$ git clone https://github.com/karimsa/gulp-jslint.git
.. clones gulp-jslint ..
$ cd gulp-jslint
$ npm install
.. installs dependencies ..
$ gulp
.. builds gulp-jslint into gulp.jslint.min.js ..
```

## Support
Please use the official issues section in GitHub to post issues.
All forks and helpful comments are much appreciated. :D