# @npmgraph/demo-b

Supporting demo package for [@npmgraph/demo](../demo). Published to npm so npmgraph can resolve it as a dependency.

## What it demonstrates

| Feature | How |
|---|---|
| `dependencies` | `chalk` |
| `peerDependencies` (met) | `react >=18` — satisfied by `@npmgraph/demo` which lists `react ^18` |
| `peerDependencies` (unmet, optional) | `vue >=3` — not present anywhere in `@npmgraph/demo`'s tree |
