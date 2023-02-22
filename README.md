## Introduction

This is a server boilerplate using GraphQL and MongoDB. Support subscriptions using GraphQL Yoga. 

## Getting started

1. Clone this repo using
```
https://github.com/aliraxa-hub/GraphQL-MongoDB.git
```
2. Move to the appropriate directory: 
```
cd GraphQL-MongoDB
``` 
3. Install dependencies using.
```
yarn install 
or 
npm install
```
4. Set `.env` file with your mongoURI and past the database connection link from mongodb atlas.
5. Run 
```
npm start
``` 
6. See the example app at 
```
http://localhost:4000/playground
```

## Commands

```
npm start
```
start the playground at 
```
http://localhost:4000/playground
```

## Query

### Mutation Query
Used to create update and delete here is the create methpd

```
mutation CreateUser($user: CreateUserInput!) {
  createUser(user: $user) {
    name
    email
    age
  }
}
```

### Query Veriable
```
{
  "user": {
    "name": "John Doe",
    "email": "doe@example.com",
    "age": 30
  }
}
```
