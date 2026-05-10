# demo

Demo monorepo for testing [npmgraph](https://npmgraph.js.org). It contains packages that demonstrate the full range of dependency types and edge cases that npmgraph needs to handle.

## Releasing

Run the **Release** workflow manually from the Actions tab. It publishes all workspace packages to npm with [provenance](https://docs.npmjs.com/generating-provenance-statements) (trusted publishing).

The version is bumped automatically.
