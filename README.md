# GoFinances

This is an app manager for financial transactions. 

There is a Node server, which connects to a Postgres database and the React APP sends the requests and deal with the responses.

### Knowledge and skills gained

* Typing with Typescript
* Routing with Express.js
* Object modeling with TypeORM
* File upload with Multer
* Postgres and Docker
* EditorConfig and ESLint

### Main functionalities

* CRUD for Transactions
* CSV file upload and importation of its data into the database

## How to start the server

1. Create a Postgres database named _gostack_desafio06_, with Docker:

```
docker run -e POSTGRES_DB=gostack_desafio06 --name gostack_desafio06 -e POSTGRES_PASSWORD=docker -p 5432:5432 -d postgres
```

2. Go to the `backend` folder and initialize `node_modules`:

```
cd backend/
yarn install
```

3. Start the server with the following command

```
yarn dev:server
```

## How to start the React APP

1. Go to the `frontend` folder and initialize `node_modules`:

```
cd frontend/
yarn install
```

2. Start the app with the following command

```
yarn start
```

## How to run tests

1. Create a Postgres database named _gostack_desafio06_tests_, with Docker:

```
docker run -e POSTGRES_DB=_gostack_desafio06_tests_ --name _gostack_desafio06_tests_ -e POSTGRES_PASSWORD=docker -p 5432:5432 -d postgres
```

3. Go to the `backend` or `frontend` folder and run tests:

```
yarn test
```
