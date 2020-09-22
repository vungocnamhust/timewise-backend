# Timewise
This is backend of timewise application for saling watches

## Feature
- CRUD

## Module

- User (Account)
- Product + Category
- Order (Shopping Cart)
- Search
- Statics 

## Directory structure

```bash
|
|____timewise-backend
|    |
|    |____configs
|    |    |____configs.go
|    |
|    |____api
|    |    |____notes.go
|    |    |____users.go
|    |
|    |____users
|    |    |____store.go
|    |    |____cache.go
|    |    |____users.go
|    |    |____users_test.go
|    |
|    |____notes
|    |    |____notes.go
|    |
|    |____platform
|    |    |____stringutils
|    |    |____datastore
|    |    |     |____datastore.go
|    |    |____cachestore
|    |    |    |____cachestore.go
|    |    |____logger
|    |         |____logger.go
|    |
|    |____server
|         |____http
|         |    |____web
|         |    |    |____templates
|         |    |         |____index.html
|         |    |____handlers_notes.go
|         |    |____handlers_users.go
|         |    |____http.go
|         |
|         |____grpc
|
|____lib
|    |____notes
|         |____notes.go
|
|____vendor
|
|____docker
|    |____Dockerfile # obviously your 'default' dockerfile
|
|____go.mod
|____go.sum
|
|____ciconfig.yml # depends on the CI/CD system you're using. e.g. .travis.yml
|____README.md
|____main.go
|
```

## cmd

- Store all the code run firstly in project
- Can store all version of `main.go`

## db

- Connect to Postgres 

## log

- Store log method to store data into log.files
- When a problem will be happended, log will get errors then write to log.files 

## log.files

- Store errors of system

## model

- Store object 

## repository

- Managing logic working with db

## router

- Define API 

## security

- All algorithms for security

## validator

- Validate all data 
