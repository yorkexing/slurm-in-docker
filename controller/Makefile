
SLURM_VERSION = 23.02.1
IMAGE = harbor.cqxyy.net/wict/slurm.controller

.PHONY: all build clean test


all: build

build:
	docker build -t $(IMAGE):$(SLURM_VERSION) .

clean:
	@[ -z $(docker images -q $(IMAGE):$(SLURM_VERSION)) ] || docker rmi $(IMAGE):$(SLURM_VERSION)
