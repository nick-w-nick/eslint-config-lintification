# eslint-config-lintification

A suite of battle-tested linting rules for any modern Node.js application, with full support for the most common TypeScript rules.



## Table of Contents
- [eslint-config-lintification](#eslint-config-lintification)
  - [Table of Contents](#table-of-contents)
  - [Usage](#usage)
    - [Install](#install)
    - [Extend the Configuration](#extend-the-configuration)
  - [License](#license)



## Usage

### Install
```bash
$ npm install -D eslint-config-lintification eslint @stylistic/eslint-plugin@2.10.1 @typescript-eslint/eslint-plugin@6.7.4 eslint-plugin-file-progress@1.3.0 eslint-plugin-import@2.28.1 eslint-plugin-import-newlines@1.3.4 eslint-plugin-jest@27.4.2 eslint-plugin-newline-destructuring@1.2.2 eslint-plugin-simple-import-sort@10.0.0 eslint-import-resolver-typescript@3.6.1
```

### Extend the Configuration

Either add `"extends": "lintification"` to your linting configuration or add the below to your package.json to use the rules with no modifications:
```json
{
    "eslintConfig": {
        "extends": "lintification"
    }
}
```



## License
[MIT](https://choosealicense.com/licenses/mit/)
