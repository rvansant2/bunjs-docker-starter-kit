# bunjs-docker-starter
Bunjs Docker Starter Kit

## Bunjs Features
- From [Bunjs Documentation](https://bun.sh/)
Web APIs like `fetch`, `WebSocket`, and `ReadableStream` are built-in
- `node_modules` bun implements Node.js' module resolution algorithm, so you can use `npm` packages in Bun. `ESM` and `CommonJS` are supported, but Bun internally uses `ESM`
- In Bun, every file is transpiled. `TypeScript` & `JSX` just work
- Bun supports "paths", "jsxImportSource"and more from `tsconfig.json` files
- Bun.Transpiler Bun's `JSX` & `TypeScript` transpiler is available as an API in Bun
- use the fastest system calls available with Bun.write to write, copy, pipe, send and clone files
- Bun automatically loads environment variables from `.env` files. No more require("dotenv").config()
- Bun ships with a fast `SQLite3` client built-in `bun:sqlite`
- Node-API Bun implements most of Node-API (N-API). Many Node.js native modules just work
- `bun:ffi` call native code from JavaScript with Bun's low-overhead foreign function interface
- `node:fs` node:path Bun natively supports a growing list of Node.js core modules along with globals like Buffer and process

## Required
- Docker desktop

## Run
- Clone the repo and run `cd bunjs-docker-starter`.
- Run the following command: `docker compose up --build, and optionally add `-d` to run as a daemon.
- Go to [http://localhost:3000](http://localhost:3000) to view the server response `Welcome to Bun!`.

## Note on the Dockerfiles
- In the `server` directory, there are 2 versions of the `Dockerfile`: `Dockerfile` and `Dockerfile.custom`.
  - `Dockerfile.custom` uses the latest stable version of Ubuntu and custom builds the packages, roles needed to run bunjs.
  - To use this `Dockerfile.custom`, just update the `docker-compose.yml` file to use this file by replacing as follows: `dockerfile: Dockerfile.custom`.
  
