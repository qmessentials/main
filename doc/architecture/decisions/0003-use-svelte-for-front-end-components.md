# 3. Use Svelte for front-end components

Date: 2022-10-25

## Status

Superceded by [4. Use NextJS instead of Svelte](0004-use-nextjs-instead-of-svelte.md)

## Context

The original plan was to use React for the front-end components, either with Create React App or with Next.js.
At the outset, other reasonable options would've been Vue or Angular. Vue would still be a reasonable choice,
but Angular seems to be in clear decline. In the meantime, Svelte has emerged as a real option for serious
application development, and has developed a good community.

On the React side, the community seems to be coalescing around server-side rendering (SSR) tools such as 
Next.js rather than fully-client applications. Learning Next.js would be worthwhile, and might prove to be the 
best choice, but it also seems to be kind of a heavy solution for what is really not an extremely large or 
complex user interface.

## Decision

Proceed with Svelte for the front end components

## Consequences

There will be a bit of a learning curve, but there would've been some of that with Next.js anyway. Hopefully
the expected productivity gains from working with a simpler but still feature-complete framework will offset
that learning curve.

It's possible that I might end up running into unexpected challenges or limitations with Svelte that could 
cause me to switch to using React. But Svelte seems to be mature enough to handle what I'm doing here.

Svelte is also definitely the more bleeding-edge approach, but since this is an open-source project with no
specific client to create risk for, this seems like a reasonable bet on a promising technology.
