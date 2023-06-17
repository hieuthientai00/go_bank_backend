# A Simple Bank

![ci-test](https://github.com/samirprakash/go-bank/workflows/ci-test/badge.svg?branch=main)

### Features

- Create and manage account
  - Owner
  - Balance
  - Currency
- Record all balance changes for each account
  - Create an account entry for each change for each account
- Money transfer transaction
  - Perform money transfer between 2 accounts consistently within a transaction

### Pre-requisites

- Install `docker for desktop`
- Execute `brew install golang-migrate sqlc`
- Execute `go install github.com/golang/mock/mockgen@v1.6.0`

### Database Design

- Design DB schema using dbdiagram.io
  - Export the queries onto `/dbdiagrams.io`
- Save and share DB diagram within the team
- Generate SQL code to create database in a target database engine i.e. postgres/MySQL/SQLServer
- Connect to postgres container and execute the queries from `/dbdiagrams.io` to create the tables

### Generate CRUD Golang code from SQL

- Execute `make sqlc` to auto generate CRUD functionalities
- Execute `make mock` to generate mock DB
