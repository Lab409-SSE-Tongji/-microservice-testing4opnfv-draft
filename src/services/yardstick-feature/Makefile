TAG ?= dev
# docker

run-wheel-builder:
	docker run --rm \
		-v "$$(pwd)":/application -v "$$(pwd)"/wheelhouse:/wheelhouse \
		microservice-benchmarker-builder;

build-image:
	docker build -t chunchill/benchmarker-feature:$(TAG) .;

push-image:
	docker push chunchill/benchmarker-feature:$(TAG)
