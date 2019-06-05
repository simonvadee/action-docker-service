PROJECT=action-shell
DOCKER_USER=simonvadee
DOCKER_IMAGE=$(DOCKER_USER)/$(PROJECT)


# == all ======================================================================
all: build

# == build ====================================================================
build: 
	docker build -t $(DOCKER_IMAGE):latest -f Dockerfile .

# == publish ====================================================================
publish: 
	docker push $(DOCKER_IMAGE):latest
