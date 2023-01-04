help : # help here
	@echo "post : post your new post"
	@echo "clean: clears recursively the directory dist"

post: #new post
	hugo new posts/${POST_NAME}.md
	sed -i '/title/c\title: "${POST_TITLE}"' content/posts/${POST_NAME}.md

clean: # clear the directory 
	rm -fr dist

build: # create a site
	hugo > /dev/null 2>&1