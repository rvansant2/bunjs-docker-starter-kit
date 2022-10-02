# bunjs-docker-starter
Bunjs Docker Starter Kit

## Required
- Docker desktop

## Run
- Clone the repo and run `cd bunjs-docker-starter`.
- Run the following command: `docker compose up --build, and optionally add `-d` to run as a daemon.
- Go to [http://localhost:3000](http://localhost:3000) to view the server response `Welcome to Bun!`.

## Note on the Dockerfiles
- In the `server` directory, there are 2 versions of the `Dockerfile`: `Dockerfile` and `Dockerfile.custom`.
  - `Dockerfile.custom` uses the latest stable version of Ubuntu and custom builds the packages, roles needed to run bunjs.
  - To use this `Dockerfile.custom`, just update the `docker-compose.yml` file to use this file by replacing as follows: `dockerfile: Dockerfile.custom`
  
