# Example Typscript package development environment

This library has two environment one named "dev" and the other "package". This is to be used as a boiler plate for creating new packages.

Before you can start developing your package create two terminal instances and cd into both dev and package.
- Run `npm install` in both.
- In the package terminal run  `npm link`
- In the dev terminal run  `npm link package-name`

This will create a linked folder in your dev environment node_modules that you can use to reference the package locally without having to publish anything.

## Dev Scripts

The main script you will want to use in this environment is bellow. This will spin up a local server with webpack with hot refresh and watch.

```
npm run serve
```

## Package Scripts

This environment has two script that are self explanatory.

```
npm run build
```
```
npm run dev
```