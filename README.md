# eslint-config-lintification

A suite of battle-tested linting rules for any modern Node.js application, with full support for the most common TypeScript rules.



## Table of Contents
- [eslint-config-lintification](#eslint-config-lintification)
  - [Table of Contents](#table-of-contents)
  - [Usage](#usage)
    - [Installation](#installation)
    - [Extend the Configuration](#extend-the-configuration)
  - [License](#license)



## Usage

### Installation
`npm install -D eslint-config-lintification`

If you have an existing `eslint.config.js` file, add this to your list of plugins as defined [here](https://eslint.org/docs/latest/extend/shareable-configs#using-a-shareable-config) in the eslint documentation.

If you do not have a pre-existing configuration file, you can simply add the configuration to your `package.json` via the `eslintConfig` property:
```json
{
    "eslintConfig": {
        "extends": "lintification"
    }
}
```

Finally, ensure you have a valid linting script added to your `package.json`, like so:
```json
{
    "scripts": {
        "lint": "eslint --cache --ext js --ext ts ./",
        "lint:fix": "eslint --cache --fix --ext js --ext ts ./"
    }
}
```

Then, just run `npm run lint` to run the linter, and run `npm run lint:fix` to fix any issues that can automatically be fixed by the linter.

### Extend the Configuration
You can easily add new or overwrite existing rules by updating your configuration file or in the `eslintConfig` property of your `package.json`.
If you have a pre-existing `eslint.config.js` file, see [this page](https://eslint.org/docs/latest/extend/shareable-configs#overriding-settings-from-shareable-configs) from the eslint documentation on extending shared configurations.
If you don't use a traditional configuration file, you can still extend the configuration by including them in the `rules` property of the `eslintConfig` object in your `package.json`.
```json
{
    "eslintConfig": {
        "extends": "lintification",
        "rules": {
            "object-curly-spacing": "off"
        }
    }
}
```



## License
[MIT](https://choosealicense.com/licenses/mit/)
