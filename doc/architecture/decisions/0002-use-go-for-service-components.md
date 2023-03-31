# 2. Use Go for service components

Date: 2022-10-25

## Status

Accepted

## Context

There were several options for the service components:
 - Go
 - Node
 - .NET
 - Ruby/Python/PHP, etc.
 - Different tools for different components

I was always planning to use Go for the more performance-critical components. But I considered using Node or .NET 
for the components that were basically just doing CRUD operations, such as configuration, because those might be
simpler to develop and maintain.

## Decision

Use Go for all service components

## Consequences

Overall the maintenance burden should be easier for me and for anybody who uses the tool because there's only
one language and set of skills to be good with. Go has excellent library and community support for all of the
types of things we're doing. And it should be possible to achieve very high levels of performance with Go.
