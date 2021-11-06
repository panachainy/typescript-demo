# Typescript-demo

## Prerequisite

- Node.js v14.17.6

## Setup

Setup script follow below

```sh
# init project node
yarn init -y

# add dependency
yarn add --dev ts-node typescript

# init typescript config
./node_modules/.bin/tsc -init
# or in global way
# yarn global add typescript
# tsc -init
```

Create file `src/index.ts` and `.env`

Result

```txt
.
├── node_modules/
├── .env
├── index.ts
├── package.json
├── readme.md
├── tsconfig.json
└── yarn.lock
```

## Implement little project

Add dotenv dependency for load config from .env file

```sh
yarn add dotenv
yarn add --dev @types/node
```

Update file `src/index.ts`

```ts
import "dotenv/config";

const EXAMPLE_CONFIG = process.env.EXAMPLE_CONFIG;
console.log("EXAMPLE_CONFIG: ", EXAMPLE_CONFIG);
```

Try to Run

```sh
yarn ts-node ./src/index.ts
```
