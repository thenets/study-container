build:
	docker build \
		-t test-dev \
		.

inspect:
	docker inspect test-dev | jq ".[0].RootFS"

run:
	docker run -it --rm \
		-p 9000:5000 \
		test-dev
