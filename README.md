# Reason to Rock '26

This project contains a 2026 refresh of the website ReasonToRock.com. 

The project contains both original content as well as finished HTML pages. 

The Mac app [Notenik](https://notenik.app) is used to merge the content into one or more templates, producing the final `.html` files that will be seen on the Web. 

This refresh project is still very much a work-in-progress. 

The refresh has the following goals:

+ Convert all remaining textile content to Markdown;
+ Convert all metadata from Excel spreadsheets to Notenik;
+ Modernize the look and feel and coding of the website itself;
+ Convert underscores in filenames to hyphens. 

The primary project folder structure is as follows. 

+ `content` — containing the various Notenik projects contributing content to the site. 
+ `factory` — containing various types of Notenik files used to generate finished web pages from the content. 
	- `includes` — chunks of text pulled into templates, to prevent repetitive coding in the templates
	- `scripts` — script files used by Notenik to combine selected content with selected template(s)
	- `templates` — Notenik merge templates
+ `import` — tab- or comma-delimited files containing data to be imported into various content collections
+ `step-by-step` — Step-by-step notes on how I'm creating the refreshed site
+ `web` — The actual files that make up the finished website

Copyright (c) 2001-2026 by Herb Bowie except where otherwise noted.
