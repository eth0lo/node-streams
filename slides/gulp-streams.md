## Gulp and streams

		var uglify = require('gulp-uglify'),
		    rename = require('gulp-rename');
		    
		gulp.task('bundle', function() {
		    return fs.createReadStream('app.js')
		        .pipe(uglify())
		        .pipe(rename('bundle.min.js'))
		        .pipe(gulp.dest('dist/'));
		});