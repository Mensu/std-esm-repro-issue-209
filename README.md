# How to reproduce

with ``"cjs": { "vars": true }`` turned on

```
npm i
node -r @std/esm index.js
```

- expected behavior: prints ``work`` before exiting
- actual behavior: throws ``TypeError: Cannot redefine property: debugMode``

```
npm i @std/esm@0.18.0
node -r @std/esm index.js
```

- the behavior would be normal: prints ``work``
