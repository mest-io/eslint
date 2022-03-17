## ESLint for MEST team

This is the eslint configuration used by Organization MEST.

## Usage

### JavaScript

1. Install: `yarn add @mest-fe/eslint-config -D`
2. Add the following code to the in-configuration file (`.eslintrc`):

```json
{ "extends": "@mest-fe/eslint-config" }
```

### TypeScript

1. Install: `yarn add @mest-fe/eslint-config-ts -D`
2. Adding configuration to the `.eslintrc` file:

```json
{
  "extends": ["@mest-fe/eslint-config-ts"],
  "parserOptions": {
    "project": "./tsconfig.json"
  }
}
```

### React

1. Install: `yarn add @mest-fe/eslint-config-ts @mest-fe/eslint-config-react -D`
2. Add the following code to the in-configuration file (`.eslintrc`):

```json
{
  "extends": ["@mest-fe/eslint-config-ts", "@mest-fe/eslint-config-react"],
  "parserOptions": {
    "project": "./tsconfig.json"
  }
}
```

<br/>

## LICENSE

[MIT](https://github.com/@mest/eslint/blob/master/LICENSE)
