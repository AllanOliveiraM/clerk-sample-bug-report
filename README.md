# Clerk Sample - Build Error

This is a [Next.js](https://nextjs.org) project bootstrapped with [`create-next-app`](https://nextjs.org/docs/pages/api-reference/create-next-app) created for Clerk Bug Report.

How to reproduce:

- Install deps

```sh
yarn install
```

- Run build

```sh
yarn install
```

You will see the following error:

**Funny that this error does not prevent the build.**

```log
./node_modules/next/dist/esm/client/components/navigation.js
Attempted import error: 'useContext' is not exported from 'react' (imported as 'useContext').

Import trace for requested module:
./node_modules/next/dist/esm/client/components/navigation.js
./node_modules/next/dist/esm/api/navigation.js
./node_modules/@clerk/nextjs/dist/esm/app-router/server/auth.js
./node_modules/@clerk/nextjs/dist/esm/server/index.js

./node_modules/next/dist/esm/client/components/navigation.js
Attempted import error: 'useContext' is not exported from 'react' (imported as 'useContext').

Import trace for requested module:
./node_modules/next/dist/esm/client/components/navigation.js
./node_modules/next/dist/esm/api/navigation.js
./node_modules/@clerk/nextjs/dist/esm/app-router/server/auth.js
./node_modules/@clerk/nextjs/dist/esm/server/index.js
```
