help:	## Show help for each of the Makefile recipes.
	@fgrep -h "##" $(MAKEFILE_LIST) | fgrep -v fgrep | sed -e 's/\\$$//' | sed -e 's/##//'
	
post: #new post
	hugo new posts/${POST_NAME}.md
	sed -i '/title/c\title: "${POST_TITLE}"' content/posts/${POST_NAME}.md

clean: # clear the directory 
	rm -fr dist

build: # create a site
	hugo > /dev/null 2>&1