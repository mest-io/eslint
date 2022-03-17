## ESLint for MEST team

This is the eslint configuration used by Organization MEST.

## Usage
### JavaScript

1. Install: `yarn add @mest-fe/eslint-config -D`
2. Add the following code to the in-configuration file (`.eslintrc`):

    ```
    { "extends": "@mest-fe/eslint-config" }
    ```

### TypeScript

We always recommend that you use `@typescript-eslint` instead of `tslint`, as `tslint` is now out of maintenance,
please at least make sure that you have the following dependencies installed:

  - `eslint > 5.0`

For more information on this please read the following links:

  - [Roadmap: TSLint -> ESLint](https://github.com/palantir/tslint/issues/4534) (TSLint: Stop accepting any PRs at December 1st, 2020)
  - [TSLint in 2019](https://medium.com/palantir/tslint-in-2019-1a144c2317a9)
  - [Getting Started - Linting your TypeScript Codebase](https://github.com/typescript-eslint/typescript-eslint/blob/master/docs/getting-started/linting/README.md)
  - [typescript-eslint repo](https://github.com/typescript-eslint/typescript-eslint)

So naturally, we need to install dependencies before we begin:

1. Install: `yarn add @mest-fe/eslint-config-ts -D`
2. Adding configuration to the `.eslintrc` file:

    ```json
    "extends": ["@mest-fe/eslint-config-ts"],
    "parserOptions": {
      "project": "./tsconfig.json"
    }
    ```

### React 

```json
{
  "extends": [
    "@mest-fe/eslint-config-ts",
    "@mest-fe/eslint-config-react"
  ],
  "parserOptions": {
    "project": "./tsconfig.json"
  }
}
```

<br/>

## LICENSE

[MIT](https://github.com/@mest/eslint/blob/master/LICENSE)
