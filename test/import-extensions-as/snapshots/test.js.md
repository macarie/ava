# Snapshot report for `test/import-extensions-as/test.js`

The actual snapshot is saved in `test.js.snap`.

Generated by [AVA](https://avajs.dev).

## cannot configure how js, cjs, and mjs extensions should be loaded

> js not set as true

    {
      exitCode: 1,
      failed: true,
      'stats.failed': [],
      'stats.passed': [],
    }

> cjs not set as true

    {
      exitCode: 1,
      failed: true,
      'stats.failed': [],
      'stats.passed': [],
    }

> mjs not set as true

    {
      exitCode: 1,
      failed: true,
      'stats.failed': [],
      'stats.passed': [],
    }

## load custom extension as commonjs

> ts extension

    {
      exitCode: 0,
      failed: false,
      'stats.failed': [],
      'stats.passed': [
        {
          file: 'test-cjs-syntax.ts',
          title: 'always passing test',
        },
        {
          file: 'test-esm-syntax.ts',
          title: 'always passing test',
        },
        {
          file: 'test.js',
          title: 'always passing test',
        },
      ],
    }

## load js, cjs, and mjs extensions when set to true

> standard node extensions

    {
      exitCode: 0,
      failed: false,
      'stats.failed': [],
      'stats.passed': [
        {
          file: 'test.cjs',
          title: 'always passing test',
        },
        {
          file: 'test.js',
          title: 'always passing test',
        },
        {
          file: 'test.mjs',
          title: 'always passing test',
        },
      ],
    }

## cannot load custom extension when not set to "commonjs" or "module"

> ts not set as ("commonjs" | "module")

    {
      exitCode: 1,
      failed: true,
      'stats.failed': [],
      'stats.passed': [],
    }