# gulp-clear-log4js v0.0.1

## Information

<table>
    <tr> 
        <td>Package</td><td>gulp-clear-log4js</td>
    </tr>
    <tr>
        <td>Description</td>
        <td>Clear the log4js code</td>
    </tr>
    <tr>
        <td>Node Version</td>
        <td>>= 0.8</td>
    </tr>
</table>

## Install
```js
npm install gulp-clear-log4js
```

## Example usage with [Gulp](http://github.com/gulpjs/gulp)

```js
var gulp = require('gulp');
var clearLog = require('clear-log4js');

gulp.task('clear-log4js', function() {
    gulp.src('./*.*')
        .pipe(clearLog())
        .pipe(gulp.dest('./'));
});

gulp.task('default', ['clear-log4js']);

// Rerun the task when a file changes
gulp.task('watch', function () {
  gulp.watch('./*.*', ['clear-log4js']);
});
```

## Parameters