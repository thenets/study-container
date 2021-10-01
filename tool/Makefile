build:
	docker build \
		-t test-tools \
		.

inspect:
	docker inspect test-tools | jq ".[0]"

run:
	docker run -it --rm \
		test-tools
