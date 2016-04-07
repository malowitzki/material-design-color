# Material design color

Google's Material design color palette implemented for Sass

## Install

### Bower

In your project's root directory, run `bower install material-design-color`.  Include the `--save` option if you want the package saved as a dependency in your bower.json.

### Meteor

Coming soon!

## Import

Import the partial into any of your Sass files:

```Sass
@import "path/to/root/bower_components/material-design-color/material-design-color";
```

### Helpful tip

If you're using [gulp](http://gulpjs.com/) and [gulp-sass](https://www.npmjs.com/package/gulp-sass) to compile your Sass, use the `includePaths` option to make importing the partial a little easier:

```javascript
gulp.task("sass", function() {
	return gulp.src("src/**/*.scss")
		.pipe(sass({
			includePaths: "bower_components"
		}))
		.pipe(concat("app.css"))
		.pipe(gulp.dest("dist"));
});
```

This way, your `@import` path can be shorter, and you also have easy access to Sass partials in any other bower package you're using:

```Sass
@import "material-design-color/material-design-color";
```