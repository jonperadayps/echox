+++
title = "WebSocket Recipe"
description = "WebSocket recipe for Echo"
[menu.main]
  name = "WebSocket"
  parent = "cookbook"
+++

## Using `net` WebSocket

### Server

`server.go`

{{< embed "websocket/net/server.go" >}}

## Using `gorilla` WebSocket

### Server

`server.go`

{{< embed "websocket/gorilla/server.go" >}}

## Client

`index.html`

{{< embed "websocket/public/index.html" >}}

## Output

`Client`

```sh
Hello, Client!
Hello, Client!
Hello, Client!
Hello, Client!
Hello, Client!
```

`Server`

```sh
Hello, Server!
Hello, Server!
Hello, Server!
Hello, Server!
Hello, Server!
```

## Source Code

[See]({{< source "websocket" >}})

