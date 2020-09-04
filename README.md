# Lerna monorepo for yarn workspaces

The example shows how you can manage monorepo using [Lerna](https://github.com/lerna/lerna) monorepo package managing tool.
In this example you can figure out how to:

- Setup Lerna for [Typescript](https://www.typescriptlang.org/) codebase
- Setup custom aliases on the server and the client
- Make aliases work together with [Jest](https://jestjs.io/)

The example shows how to handle all cases from above based only on the
[tsconfig-paths](https://www.npmjs.com/package/tsconfig-paths) + Lerna + symlinks
solution.

Monorepo consists of 3 packages:

- [@project/app](./packages/app)
- [@project/utils](./packages/utils)
- [@project/ui](./packages/ui)

Install it and run:

Development:

```bash
yarn
cd packages/app
yarn dev
```

Production:

```bash
yarn
yarn app:build
cd packages/app
yarn start
```
