build:
		docker build \
		--cache-from python:3.9-bookworm \
		-t my-python-image \
		-f Dockerfile \
		. \

clean:  
	docker rmi -f my-python-image  