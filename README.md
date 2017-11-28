# nyc spawn wrap

* To reproduce the issue, clone the repo

```bash
    $ npm install
    $ npm test
```

```js

    > nyc ./node_modules/.bin/mocha "./lib/**/*.spec.js" --opts "./mocha.opts"

    /git/nyc-spawn-wrap-issue-test/node_modules/nyc/node_modules/spawn-wrap/index.js:30
    shebang = '#!'
            ^
    ReferenceError: shebang is not defined
        at Object.<anonymous> (/git/nyc-spawn-wrap-issue-test/node_modules/nyc/node_modules/spawn-wrap/index.js:30:11)
        at Module._compile (module.js:635:30)
        at Object.Module._extensions..js (module.js:646:10)
        at Module.load (module.js:554:32)
        at tryModuleLoad (module.js:497:12)
        at Function.Module._load (module.js:489:3)
        at Module.require (module.js:579:17)
        at require (internal/module.js:11:18)
        at /.node-spawn-wrap-56825-9752b13600c7/node:167:17
        at Object.<anonymous> (/.node-spawn-wrap-56825-9752b13600c7/node:181:3)
```
