# es-di

`es-di` is a dependency injection library for standard ECMAScript decorators.

## Status

The repository is currently in bootstrap mode. The package, TypeScript, lint, and open source scaffolding are in place so the runtime API can land on a stable foundation.

## Project goals

- Target TC39 Stage 3 decorators instead of legacy decorator metadata.
- Keep the authoring experience close to lightweight DI tools such as TypeDI.
- Use Bun for local development while publishing a package that runs in plain Node.js.
- Ship TypeScript declarations and clean ESM exports for npm consumers.

## Tooling

- Runtime target: Node.js 18.18+
- Development workflow: Bun
- Publish target: npm
- Type checking and builds: TypeScript 5
- Lint and format: oxlint and oxfmt

## Development

```sh
bun install
bun run hooks:validate
bun run hooks:run:pre-commit
bun run lint
bun run fmt:check
bun run typecheck
bun run build
```

`bun install` also installs the local Git hooks through Lefthook. If you need to reinstall them manually, run `bun run hooks:install`.

## Community

- Contributing guide: [CONTRIBUTING.md](./CONTRIBUTING.md)
- Code of Conduct: [CODE_OF_CONDUCT.md](./CODE_OF_CONDUCT.md)
- Security policy: [SECURITY.md](./SECURITY.md)
