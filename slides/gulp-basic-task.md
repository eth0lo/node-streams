## Basic task

		gulp.task('scripts', function() {
	    return gulp.src('./src/**/*.js')
	        .pipe(uglify())
	        .pipe(concat('all.min.js'))
	        .pipe(gulp.dest('build/'));
		});