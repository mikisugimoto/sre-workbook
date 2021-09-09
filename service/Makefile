APP_CONTAINER=dotnet
BASE_COMPOSE_FILE=docker-compose.yml
DEV_COMPOSE_FILE=docker-compose.override.yml

all: up

# Build development containers
build:
	COMPOSE_DOCKER_CLI_BUILD=1 DOCKER_BUILDKIT=1 docker-compose build --progress=plain --force-rm --pull

clean:
	docker-compose down -v --remove-orphans --rmi all
	docker-compose rm -v --force --stop

cli:
	docker exec -it $(APP_CONTAINER) /bin/bash

down:
	docker-compose down

up:
	COMPOSE_DOCKER_CLI_BUILD=1 DOCKER_BUILDKIT=1 docker-compose up --force-recreate

.PHONY: all
.PHONY: clean
.PHONY: cli
.PHONY: down
.PHONY: up
