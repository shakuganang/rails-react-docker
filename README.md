# Rails-React-TypeScript-Docker Example ![backend_test](https://github.com/ohbarye/rails-react-typescript-docker-example/actions/workflows/backend_test.yml/badge.svg) ![frontend_test](https://github.com/ohbarye/rails-react-typescript-docker-example/actions/workflows/frontend_test.yml/badge.svg)

## TL;DR

**Here is an example application with the following modern web technology stacks. With this boilerplate, you can easily start to build your own app.**

- [Ruby](https://www.ruby-lang.org/en/) 3.0.0
- [Rails](https://rubyonrails.org/) 6.1.4
- [React.js](https://reactjs.org/) 17.0.1
- [TypeScript](https://www.typescriptlang.org/) 4.3.5
- [Docker](https://docs.docker.com/)
- [PostgreSQL](https://www.postgresql.org/) 11
- [GitHub Actions](https://github.com/features/actions)

## Usage

```shell
# Setup
$ docker-compose run frontend yarn
$ docker-compose run backend bin/rails db:create db:migrate

# Start
$ docker-compose up -d

# Open frontend
$ open http://localhost:3000 # You'll see angshana page, then click any app

# Check backend API
$ curl -H 'Host: backend.localhost' http://localhost/greetings/hello
```

## Motivation

Nowadays, I feel like **we need a wide range acknowledgment on web development even if we call ourselves "backend developer" or "frontend developer".**

### Backend

The combination, Rails + PostgreSQL + Docker Compose, is just a result of using: [Docker Compose's official instruction](https://docs.docker.com/compose/rails/).

### Frontend

It consist of very thin webpack settings, TypeScript config, and Jest.
