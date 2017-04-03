# eslint-config-ndustrial
Common eslint configuration for all of ndustrial.io's node applications

## Installation
You can install this module through the regular NPM repository by using the snippet below:
```
npm install --save-dev eslint-config-ndustrial
```

or by adding this line to `devDependencies` in your `package.json` file.
```
  "eslint-config-ndustrial": "^1.0.0",
```

Once that is installed, create an `.eslintrc.json` file in your root directory and add the following line:

```
{ "extends": "ndustrial"}
```

From there, you can run eslint in your terminal with the command `eslint **/*.js`, or add that line to your package.json scripts as shown below:

```
"scripts": {
    "start": "./node_modules/.bin/nodemon server.js",
    "test": "npm run lint",
    "lint": "eslint **/*.js"
  }
```

Once it is added to your `package.json` file, you can just run `npm run lint`.