# Files

`lib.ts`, `foo.ts` - Library I'm planning to package as ESM.

`dist` - Generated JS file by TSC.

`index.html`, `index.ts` - Code that demoes the library.

# How to run

`yarn tsc` -- works

`yarn parcel index.html` -- doesn't work

```
Server running at http://localhost:40363
🚨 Build failed.

@parcel/core: Failed to resolve 'foo.js' from './lib.ts'

  /home/farseen/Projects/97.Temp/repro-parcel-ts/lib.ts:1:8
  > 1 | import "foo.js"
  >   |        ^^^^^^^^
    2 |
```
