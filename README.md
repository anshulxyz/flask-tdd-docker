# flask-tdd-docker

This is a project for reference. This is built from steps shown in https://testdriven.io/courses/tdd-flask/

## dependencies

1. docker
2. docker-compose

## run

```bash
# build and start docker image
$ docker-compose up -d --build

# run the tests
$ docker-compose exec api python -m pytest "src/tests"

# seed data
docker-compose exec api python manage.py seed_db
```

After seeding data, visit http://localhost:5004/users
