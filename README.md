# Project-template

A template for an easy start on new projects.

## Installing dependencies

Here are all the dependencies you should install for each project to create a good working environment for your project.

### es-lint

Installing:

```
npm install eslint --save-dev
```

Setting up:

```
npx eslint --init
```

### Prettier

```
npm install --save-dev prettier
```

### Creating pre-commit hooks

```
npx mrm@2 lint-staged
```

Configure package.json with this after running the command over

```
"lint-staged": {
  "*.js": [
    "eslint --fix",
    "prettier --write"
  ],
  "*.html": [
    "prettier --write"
  ],
  "*.scss": [
    "prettier --write"
  ]
}
```

### Jest

```
npm i -D jest@29.2.0
```

Configure the environment for Jest

```
npx eslint --init
```

Setting up Jest plugin

```
npm i -D eslint-plugin-jest
```

Setting up babel to work with Jest

```
npm -D install @babel/core@7.19.3 @babel/preset-env@7.19.4
```

### Cypress for end-to-end testing

```
npm install cypress --save-dev
```

Setting up cypress plugin for eslint

```
npm i -D cypress@10.7.0 eslint-plugin-cypress@2.12.1
```