Typescript seems to generate relative paths for references, when I would expect a module name.

`yarn install` from the root to install deps

See `packages/b/dist/index.d.ts`

created with `./node_modules/.bin/tsc --pretty` in `packages/b`

The reference generated is `/// <reference path="../../a/index.d.ts" />` when I would expect `/// <reference path="@ts-bug/a" />`
