# demo

Demo monorepo for testing [npmgraph](https://npmgraph.js.org). It contains packages that demonstrate the full range of dependency types and edge cases that npmgraph needs to handle.

## Releasing

Run the **Release** workflow manually from the Actions tab. It publishes all workspace packages to npm with [provenance](https://docs.npmjs.com/generating-provenance-statements) (trusted publishing).

The version is bumped automatically.

## Publishing is optional

Most packages here don't need to be published to npm:

- npmgraph can load the main `package.json` directly from GitHub.
- Dependencies are still resolved and drawn on the graph even if they can't be found.

Publishing is only needed for exploring deep dependency substitution, etc.

## Examples

`packages/demo` covers `dependencies` (including `github:`, `npm:` aliases), `devDependencies`, `peerDependencies`, `optionalDependencies` and `overrides`. `packages/demo-b` covers `peerDependenciesMeta` (optional peers).

## CI

The **CI** workflow validates that every `package.json` is valid JSON.
