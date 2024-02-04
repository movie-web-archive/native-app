# movie-web native-app

## About

This repository uses [Turborepo](https://turborepo.org) and contains:

```text
.github
  └─ workflows
        └─ CI with pnpm cache setup
.vscode
  └─ Recommended extensions and settings for VSCode users
apps
  └─ expo
      ├─ Expo SDK 50
      ├─ React Native using React 18
      ├─ Navigation using Expo Router
      ├─ Tailwind using Nativewind
      └─ Typesafe API calls using tRPC
packages
  ├─ tmdb
  |   └─ Typesafe API calls to The Movie Database
  └─ provider-utils
      └─ Typesafe API calls to the video providers 
tooling
  ├─ eslint
  |   └─ shared, fine-grained, eslint presets
  ├─ prettier
  |   └─ shared prettier configuration
  ├─ tailwind
  |   └─ shared tailwind configuration
  └─ typescript
      └─ shared tsconfig you can extend from
```

## Getting started

### When it's time to add a new package

To add a new package, simply run `pnpm turbo gen init` in the monorepo root. This will prompt you for a package name as well as if you want to install any dependencies to the new package (of course you can also do this yourself later).

The generator sets up the `package.json`, `tsconfig.json` and a `index.ts`, as well as configures all the necessary configurations for tooling around your package such as formatting, linting and typechecking. When the package is created, you're ready to go build out the package.

### References

This app is based on [create-t3-turbo](https://github.com/t3-oss/create-t3-turbo) and [Turborepo](https://turborepo.org).
