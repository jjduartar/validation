build: ##
	hugo -D > /dev/null 2>&1

.PHONY: clean
clean: ##
	rm -rf ./dist/ > /dev/null 2>&1

post: ##
	hugo new posts/$(POST_NAME).md
	echo '---\ntitle: "$(POST_TITLE)"draft: false\n---' > ./content/posts/$(POST_NAME).md  	
     
help: ##
	grep '##' ./Makefile  | sed 's/ ##/ /' |  head -n -1
