## Compile legacy JavaScript using TypeScript

The `tsconfig.json` provided compiles older JavaScript using
the TypeScript compiler while allowing newer JavaScript
features to be used.

### Sample `tsconfig.json` to use newer JavaScript features

```json
{
  "compilerOptions": {
    "module": "commonjs",
    "lib": [
      "es6",
      "es2015"
    ],
    "target": "es3",
    "allowJs": true,
    "outDir": "dist"
  },
  "include": [
    "src"
  ],
  "exclude": [
    "node_modules"
  ]
}
```