# Welcome to the Anythink Market repo

To start the app use Docker. It will start both frontend and backend, including all the relevant dependencies, and the db.

Please find more info about each part in the relevant Readme file ([frontend](frontend/readme.md) and [backend](backend/README.md)).

## Development

When implementing a new feature or fixing a bug, please create a new pull request against `main` from a feature/bug branch and add `@vanessa-cooper` as reviewer.

## First setup

<!-- **[TODO 05/01/2018 @vanessa-cooper]:** _It's been a while since anyone ran a fresh copy of this repo. I think it's worth documenting the steps needed to install and run the repo on a new machine?_ -->
1. Install Docker and Docker Compose (see [Docker docs](https://docs.docker.com/compose/install/))
2. Verify Docker is running by running `docker -v` and `docker-compose -v` in the terminal.
3. Clone the repo
4. Run `docker-compose up` in the terminal from the project root directory.
5. Test by going to `localhost:3000/api/ping` in the browser.
6. Check the frontend by going to `localhost:3001/register` in the browser.
7. One can use `docker exec` to run commands inside the containers. For example, to run a command inside the backend container, run `docker exec -it anythink-market_backend_1 bash` in the terminal. To run a command inside the frontend container, run `docker exec -it anythink-market_frontend_1 bash` in the terminal.
