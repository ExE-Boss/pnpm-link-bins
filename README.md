# @pnpm/link-bins

> Link bins to node_modules/.bin

<!--@shields('npm', 'travis')-->
[![npm version](https://img.shields.io/npm/v/@pnpm/link-bins.svg)](https://www.npmjs.com/package/@pnpm/link-bins) [![Build Status](https://img.shields.io/travis/pnpm/link-bins/master.svg)](https://travis-ci.org/pnpm/link-bins)
<!--/@-->

## Installation

```sh
npm i -S @pnpm/logger @pnpm/link-bins
```

## Usage

```ts
import linkBins, {linkBinsOfPackages} from '@pnpm/link-bins'

await linkBins('node_modules', 'node_modules/.bin')

const packages = [{manifest: packageJson, location: pathToPackage}]
await linkBinsOfPackages(packages, 'node_modules/.bin')
```

## License

[MIT](./LICENSE) © [Zoltan Kochan](https://www.kochan.io/)
