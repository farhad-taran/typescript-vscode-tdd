# Debugging TypeScript in VS Code Without Compiling (using `ts-node`)

This repo contains a sample TypeScript project with a Visual Studio Code `launch.json` that
allows you run TypeScript code and Mocha tests without a separate build step and is configured to work with the Mocha Test Explorer extension.

## Usage

```
git clone this repo
npm install
```

## VS Code Debug Tasks

This repo contains the following VS Code Debug tasks (accessible via the debug button on the left):

**Current TS File** - allows you to debug the currently open TypeScript file. Try it with `src/index.ts`:

![image](https://raw.githubusercontent.com/farhad-taran/typescript-vscode-tdd/master/screenshots/ts-file-debugging.png)

**Current TS Tests File** - allows you to debug the currently open Mocha unit tests file. Try it with `src/__tests__/person.tests.ts`:

![image](https://raw.githubusercontent.com/farhad-taran/typescript-vscode-tdd/master/screenshots/mocha-debugging.png)

These tasks should allow you to hit breakpoints in your code, without needing to compile first.

**Setting up Test Explorer** - to allow the test explorer extension to find your tests you need to add the appropriate settings:

![image](https://raw.githubusercontent.com/farhad-taran/typescript-vscode-tdd/master/screenshots/test-explorer.png)

