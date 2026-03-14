start:
	docker compose up -d --no-recreate --remove-orphans

stop:
	docker compose stop

down:
	docker compose down

recreate:
	docker compose up -d --force-recreate

build:
	docker compose build

clear:
	docker system prune
	docker builder prune

up:
	docker compose up -d
	
stop-all:
	docker stop $$(docker ps -aq)
	
enter:
	docker compose exec php bash

create-project:
	docker compose exec php composer create-project symfony/skeleton:8.0.* .

restart: stop start