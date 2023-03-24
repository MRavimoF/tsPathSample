# Test project for TS import path issue

It compiles fine
`npm run build`

But fails on running
`npm run start`

```
> start
> node build/index.js

node:internal/modules/cjs/loader:988
  throw err;
  ^

Error: Cannot find module 'suba/subFileA'
Require stack:
- /build/subb/subFileB.js
- /build/index.js
```
