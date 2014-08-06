## Gulp and streams -Fixed-

		var uglify = require('gulp-uglify'),
		    rename = require('gulp-rename'),
		    source = require('vinyl-source-stream');
		    
		gulp.task('bundle', function() {
		    return fs.createReadStream('app.js')
		    	.pipe(source())
		        .pipe(uglify())
		        .pipe(rename('bundle.min.js'))
		        .pipe(gulp.dest('dist/'));
		});