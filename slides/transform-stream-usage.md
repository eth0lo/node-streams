## Transform Stream Usage


		// Pipe the streams
		process.stdin
			.pipe(parser)
			.pipe(process.stdout);

		// Some programs like `head` send an error on stdout
		// when they don't want any more data
		process.stdout.on('error', process.exit);