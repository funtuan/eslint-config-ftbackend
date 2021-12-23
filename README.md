## Installation

```
npm install --save-dev eslint eslint-config-google eslint-config-ftbackend
```

## Usage

Once the `eslint-config-ftbackend` package is installed, you can use it by specifying `ftbackend` in the [`extends`](http://eslint.org/docs/user-guide/configuring#extending-configuration-files) section of your [ESLint configuration](http://eslint.org/docs/user-guide/configuring).

```js
{
  "extends": "ftbackend",
  "rules": {
    // Additional, per-project rules...
  }
}
```

### Using the `ftbackend` config with `eslint:recommended`

There are several rules in the [`eslint:recommended` ruleset](http://eslint.org/docs/rules/) that Google style is not opinionated about that you might want to enforce in your project.

To use Google style in conjunction with ESLint's recommended rule set, extend them both, making sure to list `ftbackend` last:

```js
{
  "extends": ["eslint:recommended", "ftbackend"],
  "rules": {
    // Additional, per-project rules...
  }
}
```

To see how the `ftbackend` config compares with `eslint:recommended`, refer to the [source code of `index.js`](https://github.com/google/eslint-config-google/blob/master/index.js), which lists every ESLint rule along with whether (and how) it is enforced by the `ftbackend` config.

## License

Apache-2 © Google
