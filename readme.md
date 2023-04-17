```bash
git clone git@github.com:brillout/plugin-vue_4.2.0-beta.0_vps-reprod
cd plugin-vue_4.2.0-beta.0_vps-reprod/
pnpm install
pnpm run build
```

Same as single line (copy-paste me):

```shell
git clone git@github.com:brillout/plugin-vue_4.2.0-beta.0_vps-reprod && cd plugin-vue_4.2.0-beta.0_vps-reprod/ && pnpm install && pnpm run build
```

Observe error:

```
/tmp/plugin-vue_4.2.0-beta.0_vps-reprod (main) pnpm run build

vite v4.3.0-beta.7 building for production...
transforming (132) node_modules/.pnpm/vite-plugin-ssr@0.4.113_vite@4.3.0-beta.7/node_modules/vite-plugin-ssr/dist/esm/shared/getPageFiles/analyzePageClientSide/determiError when using sourcemap for reporting an error: Can't resolve original location of error.
✓ 147 modules transformed.                                                                                                                                                  
✓ built in 2.48s
"default" is not exported by "pages/index/index.page.vue?vue&type=script&lang.js", imported by "pages/index/index.page.vue".
file: /home/rom/tmp/plugin-vue_4.2.0-beta.0_vps-reprod/pages/index/index.page.vue:1:7
1: import _sfc_main from "/home/rom/tmp/plugin-vue_4.2.0-beta.0_vps-reprod/pages/index/index.page.vue?vue&type=script&la...
          ^
2: export * from "/home/rom/tmp/plugin-vue_4.2.0-beta.0_vps-reprod/pages/index/index.page.vue?vue&type=script&lang.js"
3: import { createElementVNode as _createElementVNode, createTextVNode as _createTextVNode, Fragment as _Fragment, openB...
error during build:
RollupError: "default" is not exported by "pages/index/index.page.vue?vue&type=script&lang.js", imported by "pages/index/index.page.vue".
    at error (file:///home/rom/tmp/plugin-vue_4.2.0-beta.0_vps-reprod/node_modules/.pnpm/rollup@3.20.4/node_modules/rollup/dist/es/shared/node-entry.js:2125:30)
    at Module.error (file:///home/rom/tmp/plugin-vue_4.2.0-beta.0_vps-reprod/node_modules/.pnpm/rollup@3.20.4/node_modules/rollup/dist/es/shared/node-entry.js:13334:16)
    at Module.traceVariable (file:///home/rom/tmp/plugin-vue_4.2.0-beta.0_vps-reprod/node_modules/.pnpm/rollup@3.20.4/node_modules/rollup/dist/es/shared/node-entry.js:13719:29)
    at ModuleScope.findVariable (file:///home/rom/tmp/plugin-vue_4.2.0-beta.0_vps-reprod/node_modules/.pnpm/rollup@3.20.4/node_modules/rollup/dist/es/shared/node-entry.js:12234:39)
    at Identifier.bind (file:///home/rom/tmp/plugin-vue_4.2.0-beta.0_vps-reprod/node_modules/.pnpm/rollup@3.20.4/node_modules/rollup/dist/es/shared/node-entry.js:8124:40)
    at CallExpression.bind (file:///home/rom/tmp/plugin-vue_4.2.0-beta.0_vps-reprod/node_modules/.pnpm/rollup@3.20.4/node_modules/rollup/dist/es/shared/node-entry.js:5743:28)
    at CallExpression.bind (file:///home/rom/tmp/plugin-vue_4.2.0-beta.0_vps-reprod/node_modules/.pnpm/rollup@3.20.4/node_modules/rollup/dist/es/shared/node-entry.js:9653:15)
    at ExportDefaultDeclaration.bind (file:///home/rom/tmp/plugin-vue_4.2.0-beta.0_vps-reprod/node_modules/.pnpm/rollup@3.20.4/node_modules/rollup/dist/es/shared/node-entry.js:5747:23)
    at Program.bind (file:///home/rom/tmp/plugin-vue_4.2.0-beta.0_vps-reprod/node_modules/.pnpm/rollup@3.20.4/node_modules/rollup/dist/es/shared/node-entry.js:5743:28)
    at Module.bindReferences (file:///home/rom/tmp/plugin-vue_4.2.0-beta.0_vps-reprod/node_modules/.pnpm/rollup@3.20.4/node_modules/rollup/dist/es/shared/node-entry.js:13330:18)
 ELIFECYCLE  Command failed with exit code 1.
```
