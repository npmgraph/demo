# @npmgraph/demo

Main demo package for testing [npmgraph](https://npmgraph.js.org). Contains a variety of dependency types and edge cases.

## What it demonstrates

| Feature | Package / value |
|---|---|
| `dependencies` | `@npmgraph/demo-b`, `express`, `react`, `react-dom` |
| `devDependencies` | `typescript` |
| `peerDependencies` (unmet) | `webpack >=5` — not in the dependency tree |
| `npm:` alias | `react-compat: npm:react@^17.0.2` — resolves `react` under an alias |
| `github:user/repo` | `github-prefixed: github:fregante/webext-content-scripts` |
| `user/repo` shorthand | `github-shorthand: nicolo-ribaudo/tc39-proposal-string-prototype-left-pad` |
| 404 / non-existent package | `this-package-404: npm:@npmgraph/this-does-not-exist-404@^1.0.0` |
| `overrides` (existing dep) | overrides `debug` version inside `express`'s subtree |
| `overrides` (non-existing dep) | `@npmgraph/this-override-does-not-exist` — package not in the tree |

> **Note** — `github-prefixed`, `github-shorthand`, and `this-package-404` are listed under `optionalDependencies` so that `npm install` succeeds even if those references cannot be resolved.
