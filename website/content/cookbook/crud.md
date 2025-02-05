+++
title = "CRUD Recipe"
description = "CRUD (Create, read, update and delete) recipe for Echo"
[menu.main]
  name = "CRUD"
  parent = "cookbook"
+++

## Server

`server.go`

{{< embed "crud/server.go" >}}

## Client

`curl`

### Create User

```sh
curl -X POST \
  -H 'Content-Type: application/json' \
  -d '{"name":"Joe Smith"}' \
  localhost:1323/users
```

*Response*

```js
{
  "id": 1,
  "name": "Joe Smith"
}
```

### Get User

```sh
curl localhost:1323/users/1
```

*Response*

```js
{
  "id": 1,
  "name": "Joe Smith"
}
```

### Update User

```sh
curl -X PUT \
  -H 'Content-Type: application/json' \
  -d '{"name":"Joe"}' \
  localhost:1323/users/1
```

*Response*

```js
{
  "id": 1,
  "name": "Joe"
}
```

### Delete User

```sh
curl -X DELETE localhost:1323/users/1
```

*Response*

`NoContent - 204`

## Source Code

[See]({{< source "crud" >}})