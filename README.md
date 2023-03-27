# TS absolute import paths issue demonstration

On `subFileB` we use absolute path for import `import {subA} from "suba/subFileA"`.

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
