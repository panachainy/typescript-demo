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

Create file index.ts and .env

```sh
touch index.ts
touch .env
```

Result

```txt
.
├── node_modules/
├── index.ts
├── package.json
├── readme.md
├── tsconfig.json
└── yarn.lock
```
