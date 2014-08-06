## Understanding the package.json file

		{
		  "name": "<project-name>",
		  "version": "0.0.0",
		  "description": "<project-description>",
		  "main": "index.js", //Entrypoint of the project
		  "scripts": {
			"start": "node index.js"
		    "test": "gulp test"
		  },
		  "author": "<your-name>",
		  "license": "MIT"
		}

More details on what can be specified on the files are in npm's [documentation](https://github.com/npm/npm/blob/master/doc/files/package.json.md "documentation")