build a test image
```DOCKER_IMAGE_TAG="test-latest"  DOCKER_BUILD_ARGS="--build-arg TARGETOS=linux --build-arg TARGETARCH=amd64" make docker```

build a prod image
```DOCKER_BUILD_ARGS="--build-arg TARGETOS=linux --build-arg TARGETARCH=amd64" make docker```