# 7. use pgx instead of gorm

Date: 2023-06-02

## Status

Accepted

## Context

GORM is highly rated as an ORM for Go, and it does support PostgreSQL, but it seems to have poor support for
array types, which is an important part of the database design. Also, GORM imposes some defaults that are messy
to change and not exactly ideal for our data model, such as integer keys and soft deletes.

## Decision

Use pgx directly instead of GORM

## Consequences

There is more boilerplate database code in the application, and more SQL directly mixed in with the Go code. But
we have complete control over the database structure and how we interact with it. And the pgx code is very
straightforward and easy to understand.

This change also necessitates that we create and maintain database migration code, which GORM was handling automatically.
But again, the migrations can be fully controlled, so adding and even changing columns is possible within the migration.
