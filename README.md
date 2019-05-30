# eslint-config-titanium

> ESLint [shareable config](http://eslint.org/docs/developer-guide/shareable-configs.html) for internal projects at Titanium


## Installation

```
$ npm install --save-dev eslint eslint-config-airbnb eslint-config-prettier eslint-plugin-jest eslint-plugin-react eslint-config-titanium
```


## Usage

Once the `eslint-config-titanium` package is installed, you can use it by specifying `titanium` in the [`extends`](http://eslint.org/docs/user-guide/configuring#extending-configuration-files) section of your [ESLint configuration](http://eslint.org/docs/user-guide/configuring).

```js
{
  "extends": "titanium",
  "rules": {
    // Additional, per-project rules...
  }
}
```

### Using the `titanium` config with `eslint:recommended`

To use Titanium style in conjunction with ESLint's recommended rule set, extend them both, making sure to list `titanium` last:

```js
{
  "extends": ["eslint:recommended", "titanium"],
  "rules": {
    // Additional, per-project rules...
  }
}
```

To see how the `titanium` config compares with `eslint:recommended`, refer to the [source code of `index.js`](https://gitlab.titanium.codes/nicolai.voronin/eslint-config-titanium/blob/master/index.js), which lists every ESLint rule along with whether (and how) it is enforced by the `titanium` config.


##### Heavily inspired by [eslint-config-google](https://github.com/google/eslint-config-google)


