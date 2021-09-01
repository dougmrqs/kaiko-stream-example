# Node SDK

## Requirements

You will need to have Node.js runtime installed on your machine
Installation can be done here (<https://nodejs.or>g) or through third-party tools like NVM (<https://github.com/nvm-sh/nvm>).

The Node SDK offers both support for Node and Typescript/Node.

## Build the example (Typescript/Node)

- Install:

```bash
npm install
```

- Run

```bash
npm start
```

Note that for this particular step, you will need to setup an environment variable `KAIKO_API_KEY` with a valid Kaiko API key, otherwise you will get an error such as `PERMISSION_DENIED: not authorized`.

## Points to observe

- This script, differs from the example (<https://github.com/challengerdeep/kaiko-sdk-examples/blob/master/examples/node/index.ts#L160-L189>).

- The objective of this is to observe memory leaks and discuss an implementation to multiple requests upon a single stream client.

- Few logs are presented, like the logs when a connection is RESET.

- No handling was added to reconnect a missing connection in this example.
