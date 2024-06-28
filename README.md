# savim-local-bun

A simple library to save file with Savim in local (Bun version)

## Usage

```typescript
import { Savim } from 'savim';
import { SavimLocalProviderConfig, SavimLocalProvider } from 'savim-local-bun';

const savim = new Savim();

await savim.addProvider<SavimLocalProviderConfig>(
  SavimLocalProvider,
  { rootFolderPath: __dirname },
);

await savim.uploadFile('test.txt', 'thisisatest');
```

## Tests

To execute jest tests (all errors, type integrity test)

```
bun test
```

## Maintain

This package use [TSdx](https://github.com/jaredpalmer/tsdx). Please check documentation to update this package.
