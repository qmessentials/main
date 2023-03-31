# 6. Use separate repos in a single organization rather than a monorepo

Date: 2023-03-31

## Status

Accepted

Expands on [5. Use main repo for docs and for main docker compose](0005-use-main-repo-for-docs-and-for-main-docker-compose.md)

## Context

The various QMEssentials components are closely related but they also tend to evolve in very different directions, so a decision was needed as to whether to store them all in a monorepo or in separate repos

## Decision

Use separate repos under a single GitHub organization

## Consequences

Modifying and even replacing individual components will be easier, but there's added complexity around running the while system
