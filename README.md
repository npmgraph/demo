# demo

Demo monorepo for testing [npmgraph](https://npmgraph.js.org). It contains packages that demonstrate the full range of dependency types and edge cases that npmgraph needs to handle.

## Packages

| Package | Description |
|---|---|
| [`@npmgraph/demo`](packages/demo) | Main demo package with diverse dependency types |
| [`@npmgraph/demo-b`](packages/demo-b) | Supporting package used to showcase met and unmet peer dependencies |

## Releasing

Run the **Release** workflow manually from the Actions tab. It publishes all workspace packages to npm with [provenance](https://docs.npmjs.com/generating-provenance-statements) (trusted publishing).

Before triggering the workflow, bump the version in the relevant `packages/*/package.json` files.
