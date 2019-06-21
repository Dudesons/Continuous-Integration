test:
	docker-compose run myapp "py.test tests/"

ci:
	docker-compose -f docker-compose.yml -f docker-compose-ci.yml run myapp "py.test tests/"
