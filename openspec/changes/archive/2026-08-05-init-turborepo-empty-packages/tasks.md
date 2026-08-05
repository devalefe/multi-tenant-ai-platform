# Tasks

## Setup root monorepo tooling

- [ ] Create `package.json` with `pnpm` workspace settings, Turborepo dependency, and shared scripts.
- [ ] Create `pnpm-workspace.yaml` including only `packages/*`.
- [ ] Add `tsconfig.base.json` for shared TypeScript compiler settings.
- [ ] Add `.gitignore` with standard Node and monorepo ignores.

## Configure package scaffolding

- [ ] Create `packages/README.md` or package placeholder documentation for the initial workspace.
- [ ] Add shared workspace package config templates if needed for package standards.
- [ ] Ensure no apps or `apps/` workspaces exist.

## Validate the initial workspace

- [ ] Confirm root workspace files exist and the monorepo can resolve workspaces.
- [ ] Confirm the repo remains app-free and ready for library/package expansion.
