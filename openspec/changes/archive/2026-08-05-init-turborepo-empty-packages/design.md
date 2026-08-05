# Design

## Workspace layout

- Root repository uses Turborepo as the workspace orchestrator.
- `packages/*` is the only initial workspace area.
- No `apps/` workspace directories will be created at this stage.

## Tooling and dependencies

- Use `pnpm` workspaces with `packageManager` configured in the root `package.json`.
- Configure shared TypeScript settings in `tsconfig.base.json`.
- Add workspace-level linting and formatting configuration for consistency.
- Keep package scaffolding minimal: an empty package placeholder and shared configuration.

## Extensibility

- New packages can be added under `packages/` without changing the root workspace structure.
- App-level work may be added later once the package layout and tooling are stable.

## How

1. Configure root `package.json` with Turborepo and workspace definitions.
2. Create `pnpm-workspace.yaml` to include `packages/*`.
3. Add `tsconfig.base.json` and a minimal `.gitignore`.
4. Add shared package-level config placeholders for packages.
5. Do not create any application package directories or app-related root config.
