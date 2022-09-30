## WTF is this?

Template repository I use with [`degit`](https://www.npmjs.com/package/tiged) to kick-start minimal, stand-alone [Typescript](https://www.typescriptlang.org) enabled projects. It's a companion to my [altcmdio/workspace](https://github.com/altcmdio/workspace) repo that can be used to quickly generate new _component_ projects inside of a [Yarn workspace](https://yarnpkg.com/features/workspaces).

## Quick start

### Standalone package

```sh
# globally install `degit` command, if not already installed
# npm install -g tiged

degit altcmdio/package my-package
cd my-package
yarn
code -n .
```

### Workspace package

```sh
# globally install `degit` command, if not already installed
# npm install -g tiged

# where `my-project` is a workspace generated from `altcmdio/workspace`
degit altcmdio/package my-project/packages/my-package
cd my-project
code -n .

# `altcmdio/workspace` creates a devcontainer environment; run things like `yarn install` from within the devcontainer itself
```
