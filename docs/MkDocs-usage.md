## MkDocs使用

> Installing

		pip install mkdocs

> Check Version

		mkdocs --version

> Commands

		mkdocs new [dir-name] # Create a new project.
		mkdocs serve  		  # Start local server.
		mkdocs build		  # Build document site.
		mkdocs gh-deploy      # Deploy HTML in gh-pages

> Layout

		mkdocs.yml    # The configuration file.
		docs/
		index.md  # The documentation homepage.
		...       # Other markdown pages, images and other files.

> yml settings

		site_name: [title]
		site_url: [url]
		site_author: Crash
		site_favicon: favicon.ico
		theme: readthedocs
		copyright: Copyright© 2020 ASR-Crash
		nav:
		- [entry1]: [file.md /'url']
