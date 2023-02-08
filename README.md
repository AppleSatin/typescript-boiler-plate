<div align="center">
<h1 align="center"> Project Error Logo because this belows to them </h1>
    <img href="https://projecterror.dev" width="150" src="https://i.tasoagc.dev/c1pD" alt="Material-UI logo" />
</div>
<h1 align="center">FiveM TypeScript Resource Boilerplate</h1>

<div align="center">
This is a simple boilerplate for getting started with TypeScript game-scripts, in FiveM.
</div>

<div align="center">

This repository is a basic boilerplate for getting started
with TypeScript resources in FiveM. This boilerplate only comes with
development dependencies needed for FiveM-centered TypeScript transpilation, the rest
is up to you.

## Foreword

This boilerplate was originally based off a previous popular TypeScript boilerplate,
made by [d0p3t](https://github.com/d0p3t/fivem-ts-boilerplate). He heartbeakingly passed
in 2021, leaving the original unmaintained. This boilerplate was an up-to-date alternative.

Since then, this boilerplate has been updated to take advantage of tooling progress made
in the greater NPM ecosystem.

## Requirements
* Node > v16
* Yarn

## Getting Started

First clone the repository or use the template option
and place it within your `resources` folder

**Install Dependencies**

Navigate into the newly cloned folder and then into the project folder and execute
the following command, to install dependencies.

```sh
npm i
```

## Development

### Hot Building

While developing your resource, this boilerplate offers
a `watch` script that will automatically hot rebuild on any
change within the `client` or `server` directories.

```sh
npm run watch
```
*This script still requires you restart the resource for the
changes to be reflected in-game*

### Entry Points
**Client** - `./client/client.ts`

**Server** - `./server/server.ts`

## Production Build
Once you have completed the development phase of your resource,
you must create an optimized & minimized production build, using
the `build` script.

```sh
npm run build
```

## Version < 2.0.0

Version 2.0.0 introduced ESBuild as the primary bundler, removing
the option for automatic builds through the embedded FXServer webpack builder.

This documentation is preserved for legacy purposes.

### Automatic Builds (Optional)

*This is not recommended as the embedded version of yarn is
ocassionally prone to performance and environment problems. We
highly recomend, you manually run the build script*

If desired, the `fxmanifest.lua` can be setup to allow for
FXServer to automatically build on resource start. This utilizes
the embedded `yarn` & `webpack` default resources.

To enable this, add the following to your `fxmanifest.lua`

```lua
dependency {
    'yarn',
    'webpack'
}

webpack_config 'webpack.config.js'
```

### Additional Notes

This is not my boiler plate I DID NOT MAKE THIS this is just my edited version of the boiler plate to my needs if anyone has any issues with this being public you are more than welcome to write a comment and ill make it private

https://github.com/project-error/fivem-typescript-boilerplate
