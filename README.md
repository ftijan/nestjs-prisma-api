# Nest.JS, Prisma, Swagger Example API

An Example of an API built with:
- Nest.JS
- Prisma ORM
- Swagger/OpenAPI spec annotations
- `class-transformer` and `class-validator` libraries for CRUD data validation pipeline

Based on the prisma.io tutorial article [here](https://www.prisma.io/blog/nestjs-prisma-rest-api-7D056s1BmOL0), with validations and transformations examples based on the tutorial article [here](https://www.prisma.io/blog/nestjs-prisma-validation-7D056s1kOla1).

Original tutorial code examples can be found [here](https://github.com/TasinIshmam/blog-backend-rest-api-nestjs-prisma).

## Required Local Run Configuration

Requires a `.env` file with a PostgreSQL connection string in the format of:
```
DATABASE_URL="postgresql://{account_name}:{password}@localhost:5432/median-db"
```
where `{account}` and `{password}` should be replaced with a valid credential set, and `median-db` is the assumed local DB name.

## Running the app

```bash
# install npm dependencies
$ npm install

# apply DB migrations
$ npx prisma migrate dev

# development
$ npm run start

# watch mode
$ npm run start:dev

# production mode
$ npm run start:prod
```
