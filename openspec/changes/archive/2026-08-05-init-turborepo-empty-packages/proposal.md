# Init Turborepo with empty workspace and essential packages

## What

Set up the repository as a Turborepo-managed monorepo with no application packages initially and the minimum essential workspace packages and tooling required to start building libraries.

## Why

This makes the repository ready for fast polyrepo-to-monorepo evolution without committing to app-level structure too early. It provides a solid shared tooling foundation and package workspace layout while keeping the initial state small and focused.

## Goals

- Create a Turborepo root workspace configured for `pnpm` and `packages/*`.
- Add essential monorepo tooling for TypeScript, linting, formatting, and workspace orchestration.
- Reserve package workspace paths for future libraries.
- Include only library/package scaffolding; do not create application apps yet.

## Non-goals

- Do not add any app packages or `apps/` workspace apps.
- Do not implement feature-specific application logic.
- Do not adopt an opinionated UI framework or app architecture at this stage.

## Success criteria

- The repo has root Turborepo workspace configuration and package manager workspace settings.
- A minimal set of essential packages and config files exist so the monorepo can be bootstrapped and extended.
- No app workspace is present.
